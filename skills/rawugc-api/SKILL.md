---
name: rawugc-api
description: Call the RawUGC Video Generation API to create and manage AI videos (Sora 2, Kling 2.6, Veo 3.1 and other models). Use when the user wants to generate AI videos via RawUGC, integrate RawUGC API, check video status, list videos, add captions/overlays, or work with text-to-video/image-to-video generation.
requires:
  env:
    - RAWUGC_API_KEY
compatibility: Requires RAWUGC_API_KEY (Bearer token for https://rawugc.com/api/v1). Obtain from RawUGC dashboard.
homepage: https://github.com/tfcbot/rawugc-skills
source: https://github.com/tfcbot/rawugc-skills
---

# RawUGC Video Generation API

Procedural knowledge for agents to call the RawUGC Video Generation API. All requests require an API key from the RawUGC dashboard, passed via environment variable.

## Authentication

- **Environment variable**: Read the API key from `RAWUGC_API_KEY`. The key is created in the RawUGC dashboard and must be kept secret; do not hardcode or log it.
- **Header**: Send on every request: `Authorization: Bearer <value of RAWUGC_API_KEY>`.
- If `RAWUGC_API_KEY` is missing or empty, inform the user they must set it and obtain a key from the RawUGC dashboard.

## Base URL

- **Production**: `https://rawugc.com/api/v1`
- All paths below are relative to this base.

## API Versioning

RawUGC uses date-based API versioning. The current latest version is `2026-03-06`.

- **`RawUGC-Version` request header**: Override the version per-request (recommended).
- **API key pinned version**: Set when creating the key in the dashboard.
- **Fallback**: Latest version (`2026-03-06`) if neither is set.

Always send `RawUGC-Version: 2026-03-06` in requests to ensure consistent behavior.

## Endpoints

### POST /videos/generate

Initiate video generation.

**Request body (JSON)**:

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `model` | string | Yes | One of: `sora-2-text-to-video`, `sora-2-image-to-video`, `kling-2.6/motion-control`, `veo3`, `veo3_fast` |
| `prompt` | string | For text-to-video / veo3 | Text description (1-5000 chars). Required for `sora-2-text-to-video`, `veo3`, `veo3_fast` |
| `imageUrls` | string[] | For image-to-video / kling | Array of image URLs (max 10). Required for `sora-2-image-to-video`; for `kling-2.6/motion-control` also requires `videoUrls`. Veo3/veo3_fast accept up to 2 optional images (1 image = unfold from it, 2 = first/last frame). |
| `videoUrls` | string[] | For kling | Array of video URLs (max 1). Required only for `kling-2.6/motion-control` |
| `aspectRatio` | string | No | Sora: `portrait` or `landscape`. Veo3: `16:9`, `9:16`, or `Auto` |
| `nFrames` | string | No | `"10"` or `"15"` (video length, Sora models only) |
| `selectedCharacter` | string | No | Character username (e.g. `rawugc.mia`) |
| `characterOrientation` | string | No | `image` or `video` (kling only). `image` = 10s max, `video` = 30s max |
| `mode` | string | No | `720p` or `1080p` (kling only) |

**Response (201)**: `videoId`, `model`, `status` (e.g. `pending`), `creditsUsed`, `newBalance`, `estimatedCompletionTime`, `createdAt`.

### GET /videos/:videoId

Get status of a video. Path parameter: `videoId` (vid_xxx format, from the generate response).

**Response (200)**: `videoId`, `status` (`pending` | `processing` | `completed` | `failed`), `model`, `prompt`, `creditsUsed`, `url` (when `status === 'completed'`), `createdAt`, `completedAt`, `failCode`, `failMessage`, `versions` (array of edit history when present — each entry has `videoId`, `version`, `url`, `operation`, `createdAt`).

### GET /videos

List the user's videos with optional filters and pagination.

**Query parameters**: `status` (optional: `pending` | `processing` | `completed` | `failed`), `limit` (1-100, default 50), `page` (default 1).

**Response (200)**: `videos` (array of same shape as GET /videos/:videoId), `pagination`: `total`, `page`, `pageSize`, `hasMore`.

### POST /videos/captions

Add styled captions to a completed video. Costs 1 credit.

**Request body (JSON)**:

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `videoId` | string | Yes | Video identifier (vid_xxx format) |
| `language` | string | No | Language code (e.g. `en`, `es`). Defaults to auto-detect |

**Response (200)** (EditResponse): `videoId` (new version), `url`, `version`, `operation`, `creditsUsed`.

### POST /videos/overlay

Add a text overlay to a completed video.

**Request body (JSON)**:

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `videoId` | string | Yes | Video identifier (vid_xxx format) |
| `text` | string | Yes | Text to overlay (1-500 chars) |
| `position` | string | No | `top`, `center`, or `bottom` |
| `fontSize` | integer | No | Font size in pixels (8-200) |
| `topBottomMargin` | integer | No | Margin from edge in pixels (0-500) |
| `strokeThickness` | number | No | Text stroke thickness (0-10) |

**Response (200)** (EditResponse): `videoId` (new version), `url`, `version`, `operation`, `creditsUsed`.

## Errors

Responses use RFC 7807 Problem Details (JSON): `type`, `title`, `status` (HTTP code), `detail`, optional `instance`, optional `errors` (field-specific validation messages).

| Status | Meaning |
|--------|---------|
| 400 | Validation error (invalid body or params). Surface `detail` and `errors` to the user. |
| 401 | Authentication error (missing or invalid API key). Tell user to check `RAWUGC_API_KEY`. |
| 402 | Insufficient credits. User must add credits in RawUGC dashboard. |
| 403 | Insufficient scope. API key lacks required permissions. |
| 404 | Video not found (GET /videos/:videoId). |
| 429 | Rate limit exceeded. Retry after the time indicated by `X-RateLimit-Reset` header or back off. |
| 500 | Internal server error. Suggest retry or contact support. |

## Rate Limits

- API Key: 10 requests/minute. Session: 20 requests/minute.
- Response headers: `X-RateLimit-Limit`, `X-RateLimit-Remaining`, `X-RateLimit-Reset` (unix timestamp).

## Workflow: Generate then poll

1. **Generate**: `POST /videos/generate` with the desired body and `RawUGC-Version: 2026-03-06` header. On 201, note `videoId`.
2. **Poll**: Call `GET /videos/:videoId` periodically (e.g. every 10-30 seconds). Optionally use exponential backoff.
3. **Finish**: When `status === 'completed'`, use `url` for the video. When `status === 'failed'`, surface `failCode` and `failMessage` to the user.
4. **Edit** (optional): Use `POST /videos/captions` or `POST /videos/overlay` to add captions or text overlays to completed videos.

For full request/response shapes and status codes, see [reference.md](reference.md).
