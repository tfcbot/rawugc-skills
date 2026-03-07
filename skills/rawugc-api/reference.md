# RawUGC API -- Request/Response Reference

Condensed shapes for agent lookups. Base URL: `https://rawugc.com/api/v1`. Auth: `Authorization: Bearer <RAWUGC_API_KEY>`. Version: `RawUGC-Version: 2026-03-06`.

## POST /videos/generate

**Request (application/json)**

- `model` (required): `sora-2-text-to-video` | `sora-2-image-to-video` | `kling-2.6/motion-control` | `veo3` | `veo3_fast`
- `prompt` (optional, required for text-to-video/veo3): string, 1-5000 chars
- `imageUrls` (optional, required for image-to-video/kling): string[], URLs, max 10. Veo3/veo3_fast accept up to 2 optional images.
- `videoUrls` (optional, required for kling): string[], URLs, max 1
- `aspectRatio` (optional): Sora: `portrait` | `landscape`. Veo3: `16:9` | `9:16` | `Auto`
- `nFrames` (optional, Sora only): `"10"` | `"15"`
- `selectedCharacter` (optional): string
- `characterOrientation` (optional, kling only): `image` | `video`
- `mode` (optional, kling only): `720p` | `1080p`

**Response 201 (VideoGenerationResponse)**

- `videoId`: string (vid_xxx format)
- `model`: string
- `status`: `pending` | `processing` | `completed` | `failed`
- `creditsUsed`: number
- `newBalance`: number
- `estimatedCompletionTime`: string
- `createdAt`: number (ms epoch)

## GET /videos/:videoId

**Response 200 (VideoResponse)**

- `videoId`: string (vid_xxx format)
- `status`: `pending` | `processing` | `completed` | `failed`
- `model`: string
- `prompt`: string | undefined
- `creditsUsed`: number
- `url`: string (URI) | undefined -- present when status is `completed`
- `createdAt`: number (ms epoch)
- `completedAt`: number | undefined
- `failCode`: string | undefined
- `failMessage`: string | undefined
- `versions`: MediaVersion[] | undefined -- edit history, present when video has been edited

**MediaVersion**

- `videoId`: string (vid_xxx format)
- `version`: integer (1 for original, increments for edits)
- `url`: string (URI)
- `operation`: string | undefined (`captions`, `overlay`; absent for original)
- `createdAt`: number (ms epoch)

## GET /videos

**Query**

- `status` (optional): `pending` | `processing` | `completed` | `failed`
- `limit` (optional): number 1-100, default 50
- `page` (optional): number, default 1

**Response 200 (PaginatedVideosResponse)**

- `videos`: array of VideoResponse (same shape as GET /videos/:videoId)
- `pagination`: `{ total: number, page: number, pageSize: number, hasMore: boolean }`

## POST /videos/captions

**Request (application/json)**

- `videoId` (required): string (vid_xxx format)
- `language` (optional): string (e.g. `en`, `es`). Defaults to auto-detect.

**Response 200 (EditResponse)**

- `videoId`: string (vid_xxx format, new version)
- `url`: string (URI)
- `version`: integer
- `operation`: string (e.g. `caption`)
- `creditsUsed`: number (1 credit)

## POST /videos/overlay

**Request (application/json)**

- `videoId` (required): string (vid_xxx format)
- `text` (required): string, 1-500 chars
- `position` (optional): `top` | `center` | `bottom`
- `fontSize` (optional): integer, 8-200
- `topBottomMargin` (optional): integer, 0-500
- `strokeThickness` (optional): number, 0-10

**Response 200 (EditResponse)**

- `videoId`: string (vid_xxx format, new version)
- `url`: string (URI)
- `version`: integer
- `operation`: string (e.g. `overlay`)
- `creditsUsed`: number

## Error body (ApiError)

All error responses (4xx, 5xx) use RFC 7807:

- `type`: string (URI)
- `title`: string
- `status`: number (HTTP code)
- `detail`: string | undefined
- `instance`: string | undefined
- `errors`: Record<string, string[]> | undefined (validation)

**Status codes**: 400 validation, 401 auth, 402 insufficient credits, 403 insufficient scope, 404 not found, 429 rate limit, 500 server error.

## Rate limit headers

All responses include: `X-RateLimit-Limit`, `X-RateLimit-Remaining`, `X-RateLimit-Reset` (unix timestamp seconds).
