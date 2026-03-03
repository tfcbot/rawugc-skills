# rawugc-skills

Agent skills for [RawUGC](https://rawugc.com) — API integration and industry-specific UGC video format libraries. Install to give your AI agent procedural knowledge to generate AI videos via the RawUGC API, with TikTok-native, lofi video formats for skincare, mobile apps, SaaS, fashion, DTC, supplements, and B2C.

**Required env vars:** `RAWUGC_API_KEY` (Bearer token for the API; create in the [RawUGC dashboard](https://rawugc.com)).

## Installation

Install all skills (API + all industry segments):

```bash
npx skills add tfcbot/rawugc-skills
```

Install individual skills:

```bash
npx skills add tfcbot/rawugc-skills --skill rawugc-api       # API knowledge only
npx skills add tfcbot/rawugc-skills --skill ugc-skincare      # Skincare video formats
npx skills add tfcbot/rawugc-skills --skill ugc-mobile        # Mobile app video formats
npx skills add tfcbot/rawugc-skills --skill ugc-saas          # SaaS video formats
npx skills add tfcbot/rawugc-skills --skill ugc-fashion       # Fashion video formats
npx skills add tfcbot/rawugc-skills --skill ugc-dtc           # DTC video formats
npx skills add tfcbot/rawugc-skills --skill ugc-supplements   # Supplements video formats
npx skills add tfcbot/rawugc-skills --skill ugc-b2c           # B2C video formats
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
- Requests UGC-style video prompts for a specific industry
- Needs video format ideas, structures, or templates for marketing content

## Available skills

| Skill | Formats | Description |
|-------|---------|-------------|
| **rawugc-api** | — | Call the RawUGC Video Generation API: generate videos, get status, list videos. Requires `RAWUGC_API_KEY`. |
| **ugc-skincare** | 20 | Skincare UGC formats: GRWM ASMR, shelfie tours, texture shots, routines, ingredient education, and more. |
| **ugc-mobile** | 15 | Mobile app UGC formats: first-open POVs, dark mode tours, notification storytelling, screen recording demos, and more. |
| **ugc-saas** | 15 | SaaS UGC formats: emotional hook + demo, workflow ASMR, dashboard reactions, automation showcases, and more. |
| **ugc-fashion** | 20 | Fashion UGC formats: mirror OOTDs, try-on hauls, 3-way styling, fit check walks, era aesthetics, and more. |
| **ugc-dtc** | 15 | DTC UGC formats: unboxing moments, honest takes, restock reveals, subscription day rituals, and more. |
| **ugc-supplements** | 15 | Supplements UGC formats: morning stacks, gym bag dumps, taste tests, label reads, 30-day check-ins, and more. |
| **ugc-b2c** | 15 | General B2C UGC formats: first reactions, product hacks, durability checks, car reviews, aesthetic shots, and more. |

## License

See [LICENSE](LICENSE).
