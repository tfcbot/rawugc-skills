# rawugc-skills

Agent skills for the [RawUGC](https://rawugc.com) Video Generation API. Install to give your AI agent procedural knowledge to generate and manage AI videos (Sora 2 and other models) via the RawUGC API.

## Installation

```bash
npx skills add <owner>/rawugc-skills
```

To install only the RawUGC video API skill (if the CLI supports it):

```bash
npx skills add <owner>/rawugc-skills --skill rawugc-video-api
```

Replace `<owner>` with your GitHub org or username (e.g. `blurware/rawugc-skills`).

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
| **rawugc-video-api** | Call the RawUGC Video Generation API: generate videos, get status, list videos. Uses `RAWUGC_API_KEY` for auth. |

## License

See [LICENSE](LICENSE).
