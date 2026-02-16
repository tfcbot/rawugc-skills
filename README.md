# rawugc-skills

Agent skills for the [RawUGC](https://rawugc.com) Video Generation API. Install to give your AI agent procedural knowledge to generate and manage AI videos (Sora 2 and other models) via the RawUGC API.

**Required env vars:** `RAWUGC_API_KEY` (Bearer token for the API; create in the [RawUGC dashboard](https://rawugc.com)).

## Installation

```bash
npx skills add tfcbot/rawugc-skills
```

To install only the RawUGC video API skill (if the CLI supports it):

```bash
npx skills add tfcbot/rawugc-skills --skill rawugc-api
```

## Setup

1. **API key**: Create an API key in the [RawUGC dashboard](https://rawugc.com) (Account or API Keys).
2. **Environment**: Set the key in your environment so the agent can use it:
   ```bash
   export RAWUGC_API_KEY="your-api-key-here"
   ```
   Do not commit or log the key.

## When to use

The agent will use these skills when the user:

- Asks to generate AI videos via RawUGC
- Mentions the RawUGC API or video generation
- Wants to check video status or list videos
- Works with Sora, text-to-video, or image-to-video generation

## Available skills

| Skill | Description |
|-------|-------------|
| **rawugc-api** | Call the RawUGC Video Generation API: generate videos, get status, list videos. Requires `RAWUGC_API_KEY`. |

## License

See [LICENSE](LICENSE).
