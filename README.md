<p align="center">
  <strong>rawugc-skills</strong>
  <br />
  Agent skills for <a href="https://rawugc.com">RawUGC</a> — the AI UGC generation platform
  <br />
  <sub>API integration · 150 UGC video formats · 10 industry verticals · content grading</sub>
</p>

<p align="center">
  <a href="#quickstart">Quickstart</a> ·
  <a href="#rawugc-api">API</a> ·
  <a href="#ugc-skincare">Skincare</a> ·
  <a href="#ugc-fashion">Fashion</a> ·
  <a href="#ugc-mobile">Mobile</a> ·
  <a href="#ugc-saas">SaaS</a> ·
  <a href="#ugc-dtc">DTC</a> ·
  <a href="#ugc-supplements">Supplements</a> ·
  <a href="#ugc-b2c">B2C</a> ·
  <a href="#ugc-lifestyle-broll">B-Roll</a> ·
  <a href="#ugc-content-grader">Grader</a>
</p>

---

## Overview

Give your AI agent procedural knowledge to generate TikTok-native, lofi UGC videos via the RawUGC API. Each skill is a self-contained library of video formats — shot-by-shot structures, AI prompt templates, and filled examples — ready to drop into any agent workflow.

| | Skill | Formats | Type | What it does |
|---|---|:---:|---|---|
| 🔌 | [rawugc-api](#rawugc-api) | — | API | Generate AI videos, images & music; manage content; schedule social posts; research TikTok |
| 💧 | [ugc-skincare](#ugc-skincare) | 20 | Formats | Routines, texture shots, ingredient education, shelfie tours |
| 👗 | [ugc-fashion](#ugc-fashion) | 20 | Formats | OOTDs, try-on hauls, fit checks, styling challenges |
| 📱 | [ugc-mobile](#ugc-mobile) | 15 | Formats | Phone reactions, morning rituals, couch scrolls, word-of-mouth moments |
| 💻 | [ugc-saas](#ugc-saas) | 15 | Formats | Tool advocacy, desk tours, laptop closes, coffee machine pitches |
| 📦 | [ugc-dtc](#ugc-dtc) | 15 | Formats | Unboxings, honest reviews, subscription rituals, restock reveals |
| 💊 | [ugc-supplements](#ugc-supplements) | 15 | Formats | Morning stacks, gym bag dumps, taste tests, scoop close-ups |
| 🛒 | [ugc-b2c](#ugc-b2c) | 15 | Formats | First reactions, product hacks, desk companions, nightstand essentials |
| 🗣️ | [ugc-yapper](#ugc-yapper) | 15 | Formats | Single-take, talking-head videos with high personality and no production value |
| 🎬 | [ugc-lifestyle-broll](#ugc-lifestyle-broll) | 20 | B-Roll | Ambient mood footage, golden hour, rain windows, product-in-context |
| 📊 | [ugc-content-grader](#ugc-content-grader) | 3 rubrics | Scoring | Quality, complexity, and nativeness auditing for UGC scripts |

> **Total: 150 video formats + 3 scoring rubrics across 11 skills**

---

## Quickstart

Install everything:

```bash
npx skills add tfcbot/rawugc-skills
```

Set your API key:

```bash
export RAWUGC_API_KEY="your-api-key-here"
```

That's it. Your agent now knows how to generate UGC videos, pick the right format for any industry, and score content quality before generating.

---

## Setup

1. **Get an API key** — Create one in the [RawUGC dashboard](https://rawugc.com) under Account or API Keys.
2. **Set the environment variable** — The agent reads `RAWUGC_API_KEY` at runtime. Never commit or log this value.
   ```bash
   export RAWUGC_API_KEY="your-api-key-here"
   ```
3. **Install skills** — Install all at once or pick the verticals you need (see each skill section below).

---

## When the agent activates

The agent will use these skills when the user:

- Asks to generate AI videos via RawUGC
- Mentions the RawUGC API, Sora, Veo, Kling, or text-to-video / image-to-video
- Wants to check video status or list generated videos
- Requests UGC-style video prompts for a specific industry
- Needs video format ideas, shot structures, or prompt templates
- Wants to score, grade, audit, or improve UGC video scripts
- Needs ambient b-roll footage for ads or social content

---

## Skills

---

### rawugc-api

> Call the full RawUGC API to generate AI videos, images & music, manage content, schedule social posts, and research TikTok.

```bash
npx skills add tfcbot/rawugc-skills --skill rawugc-api
```

Procedural knowledge for the full RawUGC REST API. Covers video, image, and music generation; content management (personas, products, styles, messaging, characters); social scheduling (TikTok, Instagram, YouTube); TikTok research and viral library; and file upload.

**Includes:** Full endpoint docs, request/response schemas, error handling (RFC 7807), rate limiting guidance, and authentication setup.

| File | Description |
|---|---|
| [SKILL.md](skills/rawugc-api/SKILL.md) | All endpoints, authentication, request/response schemas, workflow guidance |
| [reference.md](skills/rawugc-api/reference.md) | Condensed request/response shapes, status codes, error formats |

---

### ugc-skincare

> 20 lofi, TikTok-native video formats for skincare brands. Raw, authentic, no hard CTAs — these feel like real people sharing real routines.

```bash
npx skills add tfcbot/rawugc-skills --skill ugc-skincare
```

**20 formats with prompt templates, shot-by-shot structures, and filled examples:**

| # | Format | Vibe | Frames | Quality | Complexity | Native |
|---|---|---|:---:|:---:|:---:|:---:|
| 1 | [GRWM ASMR Routine](skills/ugc-skincare/SKILL.md#1-grwm-asmr-routine) | Silent close-up of a full skincare routine, pure ASMR | 10 | 9 | low | 9 |
| 2 | [Shelfie Tour](skills/ugc-skincare/SKILL.md#2-shelfie-tour) | POV browsing a bathroom shelf, picking up the favorite | 10 | 8 | low | 9 |
| 3 | [Texture ASMR](skills/ugc-skincare/SKILL.md#3-texture-asmr) | Extreme close-up of product texture — satisfying swatch and spread | 10 | 9 | low | 10 |
| 4 | [Product on Wet Skin](skills/ugc-skincare/SKILL.md#4-product-on-wet-skin) | Applying product on damp skin post-shower, satisfying absorption | 10 | 9 | low | 9 |
| 5 | [Night Routine Wind-Down](skills/ugc-skincare/SKILL.md#5-night-routine-wind-down) | Dimly lit, cozy vibes, ASMR bottle tapping | 10 | 9 | low | 9 |
| 6 | [Skin Check-In Vlog](skills/ugc-skincare/SKILL.md#6-skin-check-in-vlog) | Talking to camera about skin, casually holding product | 10 | 8 | low | 9 |
| 7 | [This or That](skills/ugc-skincare/SKILL.md#7-this-or-that) | Two products side by side, picking the winner | 10 | 8 | low | 8 |
| 8 | [Empty Jar Reveal](skills/ugc-skincare/SKILL.md#8-empty-jar-reveal) | Fully used-up product, showing the rebuy | 10 | 9 | low | 10 |
| 9 | [Fridge Skincare](skills/ugc-skincare/SKILL.md#9-fridge-skincare) | Opening a mini skincare fridge, pulling out the star product | 10 | 8 | low | 8 |
| 10 | [Skincare Stash Close-Up](skills/ugc-skincare/SKILL.md#10-skincare-stash-close-up) | Overhead flat-lay of curated skincare collection, hero product centered | 10 | 8 | low | 9 |
| 11 | [The Double Cleanse](skills/ugc-skincare/SKILL.md#11-the-double-cleanse) | Two-step cleansing ritual — oil dissolves, water cleanser finishes | 10 | 8 | low | 8 |
| 12 | [Sunscreen Reapply](skills/ugc-skincare/SKILL.md#12-sunscreen-reapply) | Midday reapplication, car mirror, casual PSA | 10 | 9 | low | 9 |
| 13 | [The Pat-In Technique](skills/ugc-skincare/SKILL.md#13-the-pat-in-technique) | Focused patting application technique, satisfying rhythmic tapping | 10 | 9 | low | 9 |
| 14 | [No-Makeup Makeup Prep](skills/ugc-skincare/SKILL.md#14-no-makeup-makeup-prep) | Layering skincare for glass-skin glow, no makeup needed | 10 | 8 | low | 8 |
| 15 | [Vanity Shelfie Restock](skills/ugc-skincare/SKILL.md#15-vanity-shelfie-restock) | Restocking the vanity — placing fresh product in its spot | 10 | 8 | low | 9 |
| 16 | [Travel Minis](skills/ugc-skincare/SKILL.md#16-travel-minis) | Packing a dopp kit, showing what makes the cut | 10 | 8 | low | 8 |
| 17 | [Slugging Routine](skills/ugc-skincare/SKILL.md#17-slugging-routine) | Nighttime heavy moisturizer, glistening cozy vibes | 10 | 9 | low | 9 |
| 18 | [Maskimize](skills/ugc-skincare/SKILL.md#18-maskimize) | Sheet mask on, just vibing on the couch | 10 | 8 | low | 9 |
| 19 | [Derm Said This](skills/ugc-skincare/SKILL.md#19-derm-said-this) | "My dermatologist told me…" storytime while applying | 10 | 9 | low | 9 |
| 20 | [One Product Wonder](skills/ugc-skincare/SKILL.md#20-one-product-wonder) | Entire video dedicated to one hero product | 10 | 8 | low | 7 |

**Best for:** Skincare brands, beauty brands, dermatologist-recommended products, SPF brands, clean beauty, K-beauty.

**Each format includes:** Vibe description, 4-shot structure with timestamps, prompt template with `[BRACKETED]` placeholders, recommended settings, and a filled example with a real product.

| File | Description |
|---|---|
| [SKILL.md](skills/ugc-skincare/SKILL.md) | Full format library — prompt templates, shot structures, settings |
| [examples.md](skills/ugc-skincare/examples.md) | All 20 formats filled with real products (CeraVe, Drunk Elephant, Laneige, etc.) |
| [reference.md](skills/ugc-skincare/reference.md) | Quick-lookup shot list table for all 20 formats |

---

### ugc-fashion

> 20 lofi, TikTok-native video formats for fashion and apparel brands. Outfit-focused, style-driven, real closets and real fits.

```bash
npx skills add tfcbot/rawugc-skills --skill ugc-fashion
```

**20 formats with prompt templates, shot-by-shot structures, and filled examples:**

| # | Format | Vibe | Frames | Quality | Complexity | Native |
|---|---|---|:---:|:---:|:---:|:---:|
| 1 | [Mirror OOTD](skills/ugc-fashion/SKILL.md#1-mirror-ootd) | Classic mirror selfie outfit reveal | 10 | 9 | low | 10 |
| 2 | [Try-On in Real Time](skills/ugc-fashion/SKILL.md#2-try-on-in-real-time) | Trying on a piece for the first time on camera | 10 | 8 | low | 9 |
| 3 | [Fabric Close-Up](skills/ugc-fashion/SKILL.md#3-fabric-close-up) | Extreme close-up of fabric texture, stitching, material quality | 10 | 9 | low | 10 |
| 4 | [Closet Dig](skills/ugc-fashion/SKILL.md#4-closet-dig) | Rediscovering a forgotten piece in the closet | 10 | 9 | low | 10 |
| 5 | [The Tag Check](skills/ugc-fashion/SKILL.md#5-the-tag-check) | Checking the tag — brand, size, material details | 10 | 8 | low | 9 |
| 6 | [Hanger Appeal](skills/ugc-fashion/SKILL.md#6-hanger-appeal) | Examining a piece on the hanger, front and back | 10 | 8 | low | 9 |
| 7 | [The Fold](skills/ugc-fashion/SKILL.md#7-the-fold) | Satisfying folding technique, Marie Kondo energy | 10 | 8 | low | 9 |
| 8 | [Thrift Flip Energy](skills/ugc-fashion/SKILL.md#8-thrift-flip-energy) | Styling a thrifted piece to look high-end | 10 | 9 | low | 10 |
| 9 | [Color Match](skills/ugc-fashion/SKILL.md#9-color-match) | Holding piece up to closet items, finding the perfect combo | 10 | 8 | low | 9 |
| 10 | [Size Honest](skills/ugc-fashion/SKILL.md#10-size-honest) | Showing how a piece actually fits on a real body | 10 | 9 | low | 10 |
| 11 | [Rain Day Fit](skills/ugc-fashion/SKILL.md#11-rain-day-fit) | Outfit that works in bad weather, still looks good | 10 | 8 | low | 8 |
| 12 | [The Stretch Test](skills/ugc-fashion/SKILL.md#12-the-stretch-test) | Testing fabric stretch and recovery, quality check | 10 | 8 | low | 9 |
| 13 | [The Uniform](skills/ugc-fashion/SKILL.md#13-the-uniform) | The outfit you wear on repeat, no shame | 10 | 9 | low | 10 |
| 14 | [The Hand Feel](skills/ugc-fashion/SKILL.md#14-the-hand-feel) | Running hands over fabric, feeling the quality — tactile ASMR | 10 | 9 | low | 10 |
| 15 | [Color Story](skills/ugc-fashion/SKILL.md#15-color-story) | Full outfit in one color family, monochrome energy | 10 | 8 | low | 8 |
| 16 | [Hand-Me-Up](skills/ugc-fashion/SKILL.md#16-hand-me-up) | Styling a parent's/friend's old piece, making it modern | 10 | 9 | low | 10 |
| 17 | [Get Ready With Me Silent](skills/ugc-fashion/SKILL.md#17-get-ready-with-me-silent) | Silent GRWM, outfit assembly, ASMR energy | 10 | 9 | low | 9 |
| 18 | [In My X Era](skills/ugc-fashion/SKILL.md#18-in-my-x-era) | Outfit inspired by a specific aesthetic era | 10 | 8 | low | 9 |
| 19 | [That Girl Outfit](skills/ugc-fashion/SKILL.md#19-that-girl-outfit) | Clean, aspirational, effortlessly put-together look | 10 | 8 | low | 7 |
| 20 | [The Hang](skills/ugc-fashion/SKILL.md#20-the-hang) | Hanging the piece in its closet spot — it's earned its place | 10 | 8 | low | 9 |

**Best for:** Clothing brands, shoe brands, accessory brands, athleisure, sustainable fashion, luxury, streetwear, vintage.

| File | Description |
|---|---|
| [SKILL.md](skills/ugc-fashion/SKILL.md) | Full format library — prompt templates, shot structures, settings |
| [examples.md](skills/ugc-fashion/examples.md) | All 20 formats filled with real fashion brands and pieces |
| [reference.md](skills/ugc-fashion/reference.md) | Quick-lookup shot list table for all 20 formats |

---

### ugc-mobile

> 15 lofi, TikTok-native video formats for mobile app marketing. Person-focused, reaction-driven, real phone moments — no screen content needed.

```bash
npx skills add tfcbot/rawugc-skills --skill ugc-mobile
```

**15 formats with prompt templates, shot-by-shot structures, and filled examples:**

| # | Format | Vibe | Frames | Quality | Complexity | Native |
|---|---|---|:---:|:---:|:---:|:---:|
| 1 | [Phone in Hand Reaction](skills/ugc-mobile/SKILL.md#1-phone-in-hand-reaction) | Genuine reaction to what the app just did, screen facing away | 10 | 8 | low | 9 |
| 2 | [App Made Me Do This](skills/ugc-mobile/SKILL.md#2-app-made-me-do-this) | Showing a real outcome the app enabled | 10 | 9 | low | 9 |
| 3 | [The Morning Phone Grab](skills/ugc-mobile/SKILL.md#3-the-morning-phone-grab) | First thing in the morning, reaching for the app that starts the day | 10 | 8 | low | 9 |
| 4 | [The Couch Scroll](skills/ugc-mobile/SKILL.md#4-the-couch-scroll) | Casually scrolling on the couch, genuinely engaged | 10 | 8 | low | 9 |
| 5 | [Told a Friend About It](skills/ugc-mobile/SKILL.md#5-told-a-friend-about-it) | Talking to camera about recommending the app, word-of-mouth | 10 | 9 | low | 10 |
| 6 | [The "I Forgot How I Lived Without This" Moment](skills/ugc-mobile/SKILL.md#6-the-i-forgot-how-i-lived-without-this-moment) | Life before vs after the app, no screen shown | 10 | 9 | low | 10 |
| 7 | [Phone Flat on Table](skills/ugc-mobile/SKILL.md#7-phone-flat-on-table) | Phone on table, person reacting while hands free — app works in background | 10 | 8 | low | 9 |
| 8 | [Charging Nightstand](skills/ugc-mobile/SKILL.md#8-charging-nightstand) | End of day, phone on charger, the app bookends the day | 10 | 8 | low | 10 |
| 9 | [Waiting Room Scroll](skills/ugc-mobile/SKILL.md#9-waiting-room-scroll) | Using the app while waiting, making dead time productive | 10 | 8 | low | 9 |
| 10 | [Coffee Shop Phone Moment](skills/ugc-mobile/SKILL.md#10-coffee-shop-phone-moment) | Using the app at a coffee shop, aesthetic and connected | 10 | 8 | low | 9 |
| 11 | [Convince Me in 15s](skills/ugc-mobile/SKILL.md#11-convince-me-in-15s) | Ultra-fast pitch — one killer feature, done | 10 | 8 | low | 7 |
| 12 | [The Double Tap](skills/ugc-mobile/SKILL.md#12-the-double-tap) | Quick decisive interaction — open, do the thing, close, done | 10 | 8 | low | 9 |
| 13 | [Bedtime Last App](skills/ugc-mobile/SKILL.md#13-bedtime-last-app) | In bed, phone propped on chest, the last app before sleep | 10 | 8 | low | 10 |
| 14 | [Phone Face-Down Focus](skills/ugc-mobile/SKILL.md#14-phone-face-down-focus) | Phone face-down to focus, then flip as a reward — earned the break | 10 | 8 | low | 9 |
| 15 | [The AirPod Tap](skills/ugc-mobile/SKILL.md#15-the-airpod-tap) | AirPod tap to interact, audio-first experience, hands-free | 10 | 8 | low | 9 |

**Best for:** Mobile apps, productivity tools, lifestyle apps, fintech, health and fitness apps, utility apps.

| File | Description |
|---|---|
| [SKILL.md](skills/ugc-mobile/SKILL.md) | Full format library — prompt templates, shot structures, settings |
| [examples.md](skills/ugc-mobile/examples.md) | All 15 formats filled with real apps and use cases |
| [reference.md](skills/ugc-mobile/reference.md) | Quick-lookup shot list table for all 15 formats |

---

### ugc-saas

> 15 lofi, TikTok-native video formats for SaaS and B2B software. Person-focused, desk-energy, talking about tools — no screens, dashboards, or demos needed.

```bash
npx skills add tfcbot/rawugc-skills --skill ugc-saas
```

**15 formats with prompt templates, shot-by-shot structures, and filled examples:**

| # | Format | Vibe | Frames | Quality | Complexity | Native |
|---|---|---|:---:|:---:|:---:|:---:|
| 1 | [The Tool I Won't Shut Up About](skills/ugc-saas/SKILL.md#1-the-tool-i-wont-shut-up-about) | Passionate recommendation, talking to camera about the one tool | 10 | 9 | low | 10 |
| 2 | [Desk Tour Namecheck](skills/ugc-saas/SKILL.md#2-desk-tour-namecheck) | Casual desk tour, namechecking each tool in the stack | 10 | 8 | low | 9 |
| 3 | [The Laptop Close](skills/ugc-saas/SKILL.md#3-the-laptop-close) | End of workday — closing laptop with satisfaction, tool handled everything | 10 | 8 | low | 9 |
| 4 | [The "Before This Tool" Rant](skills/ugc-saas/SKILL.md#4-the-before-this-tool-rant) | Relatable frustration turned relief, before vs after the tool | 10 | 9 | low | 10 |
| 5 | [The Stack Ranking](skills/ugc-saas/SKILL.md#5-the-stack-ranking) | Ranking your SaaS tools, this one gets top billing | 10 | 8 | low | 9 |
| 6 | [Standup Vlog](skills/ugc-saas/SKILL.md#6-standup-vlog) | Quick standup-style update featuring the tool | 10 | 8 | low | 8 |
| 7 | [Client Win Storytime](skills/ugc-saas/SKILL.md#7-client-win-storytime) | Telling the story of a win enabled by the product | 10 | 9 | low | 9 |
| 8 | [The Meeting That Could've Been](skills/ugc-saas/SKILL.md#8-the-meeting-that-couldve-been) | Time saved — the meeting/process the tool eliminated | 10 | 9 | low | 10 |
| 9 | [The Walk-Away Test](skills/ugc-saas/SKILL.md#9-the-walk-away-test) | Set it and forget it — tool works even when you're not paying attention | 10 | 8 | low | 9 |
| 10 | [The Coffee Machine Pitch](skills/ugc-saas/SKILL.md#10-the-coffee-machine-pitch) | Casually explaining the tool like a watercooler conversation | 10 | 9 | low | 10 |
| 11 | [Founder POV](skills/ugc-saas/SKILL.md#11-founder-pov) | Founder or team member sharing why they built it | 10 | 8 | low | 8 |
| 12 | [The Whiteboard Moment](skills/ugc-saas/SKILL.md#12-the-whiteboard-moment) | Scribbling before/after on a whiteboard, visual proof of impact | 10 | 8 | low | 8 |
| 13 | [Friday Wrap-Up](skills/ugc-saas/SKILL.md#13-friday-wrap-up) | End-of-week review, product in the background | 10 | 8 | low | 8 |
| 14 | [The Group Chat Moment](skills/ugc-saas/SKILL.md#14-the-group-chat-moment) | Talking about introducing the tool to the team, viral spread | 10 | 9 | low | 10 |
| 15 | [The Solo Celebration](skills/ugc-saas/SKILL.md#15-the-solo-celebration) | Small private fist pump at desk — the tool just saved the day | 10 | 8 | low | 9 |

**Best for:** SaaS products, project management tools, CRMs, automation platforms, developer tools, analytics dashboards, no-code tools.

| File | Description |
|---|---|
| [SKILL.md](skills/ugc-saas/SKILL.md) | Full format library — prompt templates, shot structures, settings |
| [examples.md](skills/ugc-saas/examples.md) | All 15 formats filled with real SaaS products and workflows |
| [reference.md](skills/ugc-saas/reference.md) | Quick-lookup shot list table for all 15 formats |

---

### ugc-dtc

> 15 lofi, TikTok-native video formats for direct-to-consumer brands. Unboxing-forward, subscription-ready, honest reviews.

```bash
npx skills add tfcbot/rawugc-skills --skill ugc-dtc
```

**15 formats with prompt templates, shot-by-shot structures, and filled examples:**

| # | Format | Vibe | Frames | Quality | Complexity | Native |
|---|---|---|:---:|:---:|:---:|:---:|
| 1 | [Unboxing Moment](skills/ugc-dtc/SKILL.md#1-unboxing-moment) | Opening a delivery, genuine first impressions | 10 | 9 | low | 10 |
| 2 | [My Honest Take](skills/ugc-dtc/SKILL.md#2-my-honest-take) | Straight-to-camera honest review, no sugar-coating | 10 | 9 | low | 9 |
| 3 | [Kitchen Counter Demo](skills/ugc-dtc/SKILL.md#3-kitchen-counter-demo) | Casual product demo on the kitchen counter | 10 | 8 | low | 8 |
| 4 | [The Ritual Spot](skills/ugc-dtc/SKILL.md#4-the-ritual-spot) | Where the product lives in your home — its permanent spot | 10 | 8 | low | 10 |
| 5 | [The Restock](skills/ugc-dtc/SKILL.md#5-the-restock) | Reordering a product you've run out of — loyalty moment | 10 | 9 | low | 10 |
| 6 | [The Repurchase Moment](skills/ugc-dtc/SKILL.md#6-the-repurchase-moment) | New one arriving as the old one runs out — loyalty loop | 10 | 9 | low | 10 |
| 7 | [Morning Ritual](skills/ugc-dtc/SKILL.md#7-morning-ritual) | Product woven into the morning routine naturally | 10 | 8 | low | 9 |
| 8 | [The Smell Test](skills/ugc-dtc/SKILL.md#8-the-smell-test) | Opening and smelling the product — genuine sensory reaction | 10 | 8 | low | 10 |
| 9 | [Counter Flat-Lay](skills/ugc-dtc/SKILL.md#9-counter-flat-lay) | Overhead shot of product in its natural habitat, styled but real | 10 | 8 | low | 9 |
| 10 | [The Texture Moment](skills/ugc-dtc/SKILL.md#10-the-texture-moment) | Close-up of product material, texture, finish — tactile discovery | 10 | 8 | low | 9 |
| 11 | [One Week Later](skills/ugc-dtc/SKILL.md#11-one-week-later) | Follow-up review after a week of use | 10 | 8 | low | 9 |
| 12 | [Why I Switched](skills/ugc-dtc/SKILL.md#12-why-i-switched) | Story of leaving an old brand for this one | 10 | 9 | low | 9 |
| 13 | [The Shelf Moment](skills/ugc-dtc/SKILL.md#13-the-shelf-moment) | Product on a styled shelf among objects — decorative and functional | 10 | 8 | low | 9 |
| 14 | [The Thing I Keep Recommending](skills/ugc-dtc/SKILL.md#14-the-thing-i-keep-recommending) | Telling friends about it, word-of-mouth energy | 10 | 9 | low | 10 |
| 15 | [The "Just One Thing" Buy](skills/ugc-dtc/SKILL.md#15-the-just-one-thing-buy) | Talking about buying just this one thing — intentional, disciplined | 10 | 9 | low | 10 |

**Best for:** DTC brands, subscription boxes, food and beverage, home goods, pet products, wellness brands, small-batch products.

| File | Description |
|---|---|
| [SKILL.md](skills/ugc-dtc/SKILL.md) | Full format library — prompt templates, shot structures, settings |
| [examples.md](skills/ugc-dtc/examples.md) | All 15 formats filled with real DTC brands and products |
| [reference.md](skills/ugc-dtc/reference.md) | Quick-lookup shot list table for all 15 formats |

---

### ugc-supplements

> 15 lofi, TikTok-native video formats for supplement and wellness brands. Stack-focused, gym-adjacent, health-conscious.

```bash
npx skills add tfcbot/rawugc-skills --skill ugc-supplements
```

**15 formats with prompt templates, shot-by-shot structures, and filled examples:**

| # | Format | Vibe | Frames | Quality | Complexity | Native |
|---|---|---|:---:|:---:|:---:|:---:|
| 1 | [Morning Stack](skills/ugc-supplements/SKILL.md#1-morning-stack) | Lining up supplements for the morning dose | 10 | 9 | low | 9 |
| 2 | [Gym Bag Dump](skills/ugc-supplements/SKILL.md#2-gym-bag-dump) | Emptying a gym bag, supplements among the essentials | 10 | 9 | low | 10 |
| 3 | [The Scoop Close-Up](skills/ugc-supplements/SKILL.md#3-the-scoop-close-up) | Satisfying close-up of scooping powder, tapping on rim | 10 | 9 | low | 10 |
| 4 | [The Cabinet Pull](skills/ugc-supplements/SKILL.md#4-the-cabinet-pull) | Opening supplement cabinet, pulling out the hero — front and center | 10 | 8 | low | 9 |
| 5 | [Pill Organizer ASMR](skills/ugc-supplements/SKILL.md#5-pill-organizer-asmr) | Filling a weekly pill organizer, satisfying clicks | 10 | 9 | low | 9 |
| 6 | [30-Day Check-In](skills/ugc-supplements/SKILL.md#6-30-day-check-in) | Honest update after a month of use | 10 | 8 | low | 9 |
| 7 | [Taste Test No Filter](skills/ugc-supplements/SKILL.md#7-taste-test-no-filter) | Real-time taste reaction, no editing | 10 | 9 | low | 10 |
| 8 | [The One I Actually Notice](skills/ugc-supplements/SKILL.md#8-the-one-i-actually-notice) | The one supplement where you feel the difference | 10 | 9 | low | 10 |
| 9 | [Travel Supplement Kit](skills/ugc-supplements/SKILL.md#9-travel-supplement-kit) | What supplements make it into the travel bag | 10 | 8 | low | 8 |
| 10 | [Post-Workout Ritual](skills/ugc-supplements/SKILL.md#10-post-workout-ritual) | Post-gym supplement routine, recovery energy | 10 | 8 | low | 8 |
| 11 | [The Palm Display](skills/ugc-supplements/SKILL.md#11-the-palm-display) | Capsules in an open palm — showing what you take, the physical ritual | 10 | 8 | low | 9 |
| 12 | [Nightstand Lineup](skills/ugc-supplements/SKILL.md#12-nightstand-lineup) | Nighttime supplements on the bedside table | 10 | 8 | low | 8 |
| 13 | [My Non-Negotiables](skills/ugc-supplements/SKILL.md#13-my-non-negotiables) | The supplements you'll never stop taking | 10 | 9 | low | 9 |
| 14 | [Fridge Door Reveal](skills/ugc-supplements/SKILL.md#14-fridge-door-reveal) | Opening the fridge, supplements organized on the door | 10 | 8 | low | 9 |
| 15 | [The Water Drop](skills/ugc-supplements/SKILL.md#15-the-water-drop) | Dropping supplement into water, watching it dissolve and swirl | 10 | 9 | low | 10 |

**Best for:** Supplement brands, protein powders, vitamins, adaptogens, gut health, sports nutrition, wellness stacks, greens powders.

| File | Description |
|---|---|
| [SKILL.md](skills/ugc-supplements/SKILL.md) | Full format library — prompt templates, shot structures, settings |
| [examples.md](skills/ugc-supplements/examples.md) | All 15 formats filled with real supplement brands |
| [reference.md](skills/ugc-supplements/reference.md) | Quick-lookup shot list table for all 15 formats |

---

### ugc-b2c

> 15 lofi, TikTok-native video formats for general B2C consumer products. Versatile, product-agnostic, works across categories.

```bash
npx skills add tfcbot/rawugc-skills --skill ugc-b2c
```

**15 formats with prompt templates, shot-by-shot structures, and filled examples:**

| # | Format | Vibe | Frames | Quality | Complexity | Native |
|---|---|---|:---:|:---:|:---:|:---:|
| 1 | [Just Got This](skills/ugc-b2c/SKILL.md#1-just-got-this) | Holding up a new product, first impressions | 10 | 9 | low | 10 |
| 2 | [The Desk Companion](skills/ugc-b2c/SKILL.md#2-the-desk-companion) | Product on your desk while you work — always there, part of the setup | 10 | 8 | low | 9 |
| 3 | [The First Touch](skills/ugc-b2c/SKILL.md#3-the-first-touch) | First time holding the product — tactile discovery, quality check | 10 | 9 | low | 10 |
| 4 | [Hack I Found](skills/ugc-b2c/SKILL.md#4-hack-i-found) | Unexpected use case or trick with the product | 10 | 9 | low | 10 |
| 5 | [Honest Pros and Cons](skills/ugc-b2c/SKILL.md#5-honest-pros-and-cons) | Balanced review listing the good and the bad | 10 | 8 | low | 8 |
| 6 | [The One Detail](skills/ugc-b2c/SKILL.md#6-the-one-detail) | Zeroing in on one design detail that makes the product special | 10 | 8 | low | 9 |
| 7 | [The Sound It Makes](skills/ugc-b2c/SKILL.md#7-the-sound-it-makes) | ASMR focus on the satisfying sounds of the product | 10 | 9 | low | 10 |
| 8 | [Would I Rebuy](skills/ugc-b2c/SKILL.md#8-would-i-rebuy) | Verdict after extended use — rebuy or no? | 10 | 9 | low | 10 |
| 9 | [The Friend Text](skills/ugc-b2c/SKILL.md#9-the-friend-text) | Talking about texting a friend to recommend this — word-of-mouth | 10 | 8 | low | 9 |
| 10 | [Car Review](skills/ugc-b2c/SKILL.md#10-car-review) | Reviewing the product from the car, casual energy | 10 | 8 | low | 9 |
| 11 | [The Thing That Fixed](skills/ugc-b2c/SKILL.md#11-the-thing-that-fixed) | The one problem this product solved | 10 | 9 | low | 10 |
| 12 | [The Restock Click](skills/ugc-b2c/SKILL.md#12-the-restock-click) | Rebuying without hesitation — loyalty confirmed, no research needed | 10 | 8 | low | 9 |
| 13 | [Gift Guide Energy](skills/ugc-b2c/SKILL.md#13-gift-guide-energy) | Positioning the product as a gift recommendation | 10 | 7 | low | 6 |
| 14 | [The Nightstand Essential](skills/ugc-b2c/SKILL.md#14-the-nightstand-essential) | Product on the nightstand — first or last thing of the day | 10 | 8 | low | 9 |
| 15 | [The Aesthetic](skills/ugc-b2c/SKILL.md#15-the-aesthetic) | Product styled beautifully, pure visual content | 10 | 8 | low | 8 |

**Best for:** Consumer electronics, home products, kitchen gadgets, outdoor gear, toys, cleaning products, general consumer goods.

| File | Description |
|---|---|
| [SKILL.md](skills/ugc-b2c/SKILL.md) | Full format library — prompt templates, shot structures, settings |
| [examples.md](skills/ugc-b2c/examples.md) | All 15 formats filled with real consumer products |
| [reference.md](skills/ugc-b2c/reference.md) | Quick-lookup shot list table for all 15 formats |

---

### ugc-yapper

> 15 lofi, TikTok-native video formats for Yapper-style ads. Raw, authentic, single-take, talking-head videos with high personality and no production value.

```bash
npx skills add tfcbot/rawugc-skills --skill ugc-yapper
```

**15 formats with prompt templates, shot-by-shot structures, and filled examples:**

| # | Format | Vibe | Frames | Quality | Complexity | Native |
|---|---|---|:---:|:---:|:---:|:---:|
| 1 | [The Car Rant](skills/ugc-yapper/SKILL.md#1-the-car-rant) | Passionate, unfiltered, and direct rant in a car. | 10 | 9 | low | 10 |
| 2 | [The Mid-Meal Monologue](skills/ugc-yapper/SKILL.md#2-the-mid-meal-monologue) | Casual, relatable, and slightly messy talk while eating. | 10 | 8 | low | 9 |
| 3 | [The Cooking Confessional](skills/ugc-yapper/SKILL.md#3-the-cooking-confessional) | Intimate, messy, and genuine story while cooking. | 10 | 8 | low | 9 |
| 4 | [The Distracted Diatribe](skills/ugc-yapper/SKILL.md#4-the-distracted-diatribe) | Chaotic, funny, and very real story with constant distractions. | 10 | 8 | low | 9 |
| 5 | [The Walking and Talking Head](skills/ugc-yapper/SKILL.md#5-the-walking-and-talking-head) | Energetic, fast-paced, and in-the-moment talk while walking. | 10 | 8 | low | 8 |
| 6 | [The Bathroom Mirror Monologue](skills/ugc-yapper/SKILL.md#6-the-bathroom-mirror-monologue) | Introspective, personal, and raw talk to one's reflection. | 10 | 9 | low | 9 |
| 7 | [The Late-Night Thoughts](skills/ugc-yapper/SKILL.md#7-the-late-night-thoughts) | Sleepy, intimate, and unfiltered talk in bed. | 10 | 9 | low | 9 |
| 8 | [The "Just Got Out of the Shower" Rant](skills/ugc-yapper/SKILL.md#8-the-just-got-out-of-the-shower-rant) | Fresh, energetic, and spontaneous rant after a shower. | 10 | 9 | low | 10 |
| 9 | [The "I'm So Over This" Complaint](skills/ugc-yapper/SKILL.md#9-the-im-so-over-this-complaint) | Relatable, funny, and a little bit dramatic complaint. | 10 | 8 | low | 9 |
| 10 | [The "I Can't Believe I'm Admitting This" Confession](skills/ugc-yapper/SKILL.md#10-the-i-cant-believe-im-admitting-this-confession) | Secretive, funny, and vulnerable confession. | 10 | 8 | low | 9 |
| 11 | [The "Hot Take" Debate](skills/ugc-yapper/SKILL.md#11-the-hot-take-debate) | Bold, opinionated, and engaging debate on a controversial topic. | 10 | 8 | low | 8 |
| 12 | [The "I'm a Genius" Hack](skills/ugc-yapper/SKILL.md#12-the-im-a-genius-hack) | Proud, excited, and helpful sharing of a clever hack. | 10 | 8 | low | 8 |
| 13 | [The "Unboxing Gone Wrong" Story](skills/ugc-yapper/SKILL.md#13-the-unboxing-gone-wrong-story) | Humorous, self-deprecating, and relatable story of a bad unboxing. | 10 | 8 | low | 9 |
| 14 | [The "I'm Obsessed" Rave Review](skills/ugc-yapper/SKILL.md#14-the-im-obsessed-rave-review) | Enthusiastic, passionate, and convincing gushing over a product. | 10 | 9 | low | 9 |
| 15 | [The "A Day in the Life" Montage](skills/ugc-yapper/SKILL.md#15-the-a-day-in-the-life-montage) | Authentic, aspirational, and lifestyle-focused montage. | 10 | 8 | low | 7 |

**Best for:** E-commerce, DTC, supplements, food/bev, and lifestyle products where authentic, personality-driven content is key.

**Each format includes:** Vibe description, 4-shot structure with timestamps, prompt template with `[BRACKETED]` placeholders, recommended settings, and a filled example with a real product.

| File | Description |
|---|---|
| [SKILL.md](skills/ugc-yapper/SKILL.md) | Full format library — prompt templates, shot structures, settings |
| [examples.md](skills/ugc-yapper/examples.md) | All 15 formats filled with real products and scenarios |
| [reference.md](skills/ugc-yapper/reference.md) | Quick-lookup shot list table for all 15 formats |

---

### ugc-lifestyle-broll

> 20 atmospheric, no-dialogue b-roll formats for any brand. Cinematic filler clips that weave product naturally into everyday moments — no talking, no CTAs, pure vibes.

```bash
npx skills add tfcbot/rawugc-skills --skill ugc-lifestyle-broll
```

**20 formats with prompt templates, shot-by-shot structures, and filled examples:**

| # | Format | Vibe | Frames | Quality | Complexity | Native |
|---|---|---|:---:|:---:|:---:|:---:|
| 1 | [Morning Light Pour](skills/ugc-lifestyle-broll/SKILL.md#1-morning-light-pour) | Golden light streaming onto product through curtains | 10 | 9 | low | 10 |
| 2 | [Coffee Table Moment](skills/ugc-lifestyle-broll/SKILL.md#2-coffee-table-moment) | Product on a coffee table, life happening in background | 10 | 9 | low | 10 |
| 3 | [Bag Dump](skills/ugc-lifestyle-broll/SKILL.md#3-bag-dump) | Bag contents spilled out, product among essentials | 10 | 8 | low | 9 |
| 4 | [Desk Drop](skills/ugc-lifestyle-broll/SKILL.md#4-desk-drop) | Product placed on desk with a satisfying drop — hero moment | 10 | 9 | low | 10 |
| 5 | [Vanity Top-Down](skills/ugc-lifestyle-broll/SKILL.md#5-vanity-top-down) | Overhead flat-lay of a curated vanity setup | 10 | 9 | low | 9 |
| 6 | [Window Sill](skills/ugc-lifestyle-broll/SKILL.md#6-window-sill) | Product on a windowsill, world going by outside | 10 | 9 | low | 10 |
| 7 | [Hands Close-Up](skills/ugc-lifestyle-broll/SKILL.md#7-hands-close-up) | Tight shot of hands opening, turning, examining product | 10 | 9 | low | 9 |
| 8 | [Towel and Steam](skills/ugc-lifestyle-broll/SKILL.md#8-towel-and-steam) | Post-shower steamy bathroom, product on the counter | 10 | 8 | low | 9 |
| 9 | [Bedside Table](skills/ugc-lifestyle-broll/SKILL.md#9-bedside-table) | Nightstand scene — lamp, phone, product, end-of-day | 10 | 9 | low | 10 |
| 10 | [Lap Blanket Cozy](skills/ugc-lifestyle-broll/SKILL.md#10-lap-blanket-cozy) | Product resting on a lap blanket — intimate, cozy, personal | 10 | 8 | low | 9 |
| 11 | [Plant Shelf](skills/ugc-lifestyle-broll/SKILL.md#11-plant-shelf) | Product nestled among plants and greenery | 10 | 9 | low | 10 |
| 12 | [Linen and Texture](skills/ugc-lifestyle-broll/SKILL.md#12-linen-and-texture) | Product lying on textured fabric — tactile, sensory | 10 | 9 | low | 10 |
| 13 | [Kitchen Counter](skills/ugc-lifestyle-broll/SKILL.md#13-kitchen-counter) | Product among breakfast items, morning routine energy | 10 | 8 | low | 9 |
| 14 | [Golden Hour Portrait](skills/ugc-lifestyle-broll/SKILL.md#14-golden-hour-portrait) | Person holding product at golden hour, dreamy backlight | 10 | 9 | low | 9 |
| 15 | [Rain Window](skills/ugc-lifestyle-broll/SKILL.md#15-rain-window) | Product near a rain-streaked window, moody and cozy | 10 | 9 | low | 10 |
| 16 | [Workout Cool-Down](skills/ugc-lifestyle-broll/SKILL.md#16-workout-cool-down) | Product pulled from a gym bag, post-workout context | 10 | 8 | low | 9 |
| 17 | [Sunset Drive](skills/ugc-lifestyle-broll/SKILL.md#17-sunset-drive) | Product in a car cupholder during a golden hour drive | 10 | 8 | low | 9 |
| 18 | [Mirror Reflection](skills/ugc-lifestyle-broll/SKILL.md#18-mirror-reflection) | Product seen through a mirror, layered composition | 10 | 9 | low | 10 |
| 19 | [Picnic Spread](skills/ugc-lifestyle-broll/SKILL.md#19-picnic-spread) | Product at an outdoor picnic, dappled sunlight | 10 | 8 | low | 9 |
| 20 | [End-of-Day Unwind](skills/ugc-lifestyle-broll/SKILL.md#20-end-of-day-unwind) | Product on a candlelit vanity, nighttime ritual | 10 | 9 | low | 10 |

**Best for:** Ad filler footage, social media aesthetic content, brand campaigns, mood-setting clips, product placement in context. Works across all industries — pair with any vertical skill for a complete content library.

| File | Description |
|---|---|
| [SKILL.md](skills/ugc-lifestyle-broll/SKILL.md) | Full format library — prompt templates, shot structures, settings |
| [examples.md](skills/ugc-lifestyle-broll/examples.md) | All 20 formats filled with real lifestyle brands (Aesop, Byredo, Le Labo, etc.) |
| [reference.md](skills/ugc-lifestyle-broll/reference.md) | Quick-lookup shot list table for all 20 formats |

---

### ugc-content-grader

> Procedural knowledge for scoring and auditing short-form UGC video ideas. Evaluates scripts, hooks, overlays, and shot lists against three rubrics.

```bash
npx skills add tfcbot/rawugc-skills --skill ugc-content-grader
```

**Three scoring dimensions:**

| Score | Scale | What it measures |
|---|---|---|
| **Quality** | 1–10 | Hook strength, overlay tightness, shot list filmability, audience fit |
| **Complexity** | low / medium / high | AI generation failure risk — screen content, walking, precise text |
| **Native** | 1–10 | Organic creator feel vs ad energy — storytime vs marketing copy |

**Quality Score breakdown:**

| Range | Label | Meaning |
|---|---|---|
| 8–10 | High | Hook stops the scroll, overlay is tight, shot list is filmable |
| 5–7 | Mid | Decent but something is off — weak hook, overlay too long |
| 1–4 | Low | Doesn't work — confusing, wrong audience, no attention hook |

**Native Score breakdown:**

| Range | Label | Meaning |
|---|---|---|
| 7–10 | Native | Feels like a real person posting — storytime, POV, rant, hot take |
| 4–6 | Mid | Mixed — decent hook but ad structure leaking through |
| 1–3 | Adsy | Reads like a marketing department wrote it — jargon, feature lists |

**Also includes:**
- **CTA distribution rules** — 1/3 of ideas should have a CTA, 2/3 should not. No "link in bio" ever. Comment-keyword CTAs only.
- **Improvement workflow** — Rewrite patterns for low-scoring content: hook rewrites, overlay cleanup, shot list simplification, tone adjustment to Gen-Z native.
- **Complexity reduction** — Common fixes for medium/high complexity: removing screen content, eliminating walking shots, simplifying prop interactions.

**Best for:** Auditing batches of UGC ideas before generation, improving script quality scores, ensuring content feels native to TikTok/Reels, QA for content pipelines.

| File | Description |
|---|---|
| [SKILL.md](skills/ugc-content-grader/SKILL.md) | Scoring rubrics, CTA rules, improvement workflow |
| [reference.md](skills/ugc-content-grader/reference.md) | Full quality rubric, native scoring flags, complexity reduction patterns |

---

## What's in each skill

Every format skill (skincare, fashion, mobile, saas, dtc, supplements, b2c, lifestyle-broll) includes three files:

| File | Contents |
|---|---|
| `SKILL.md` | Full format library with vibe descriptions, shot-by-shot structures, and prompt templates with `[BRACKETED]` placeholders |
| `examples.md` | Every format filled in with a real brand/product — copy-paste ready prompts |
| `reference.md` | Quick-lookup shot list table for all formats at a glance |

The API skill (`rawugc-api`) includes endpoint documentation, request/response schemas, error handling, and workflow guidance.

The grader skill (`ugc-content-grader`) includes scoring rubrics, red/green flag lists, rewrite patterns, and CTA rules.

---

## License

See [LICENSE](LICENSE).
