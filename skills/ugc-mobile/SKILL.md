---
name: ugc-mobile
description: >-
  UGC video format templates for mobile app brands. Contains 15 TikTok-native,
  lofi video formats with shot-by-shot structure and AI video generation prompts.
  Use when the user wants to create mobile app UGC content — app demos, feature reveals,
  screen recordings, or app lifestyle content.
requires:
  env:
    - RAWUGC_API_KEY
compatibility: >-
  Use alongside the rawugc-api skill for API endpoint knowledge.
  Requires RAWUGC_API_KEY.
homepage: https://github.com/tfcbot/rawugc-skills
source: https://github.com/tfcbot/rawugc-skills
---

# Mobile App UGC Video Formats

15 lofi, TikTok-native video formats for mobile app brands. Raw, authentic, easy to produce. No hard CTAs — these feel like real people discovering and using apps they genuinely love.

## How to Use These Formats

1. Identify the user's goal (app launch, feature highlight, onboarding showcase, social proof).
2. Select the format below that best matches.
3. Use the **Prompt Template** to compose the `prompt` field for `POST /videos/generate`. Replace `[BRACKETED]` placeholders with details from the user.
4. Default to `aspectRatio: "portrait"` (9:16) and `nFrames: "10"` unless the format specifies otherwise.
5. Keep the tone casual, genuine, unscripted. These should feel like someone naturally discovering an app.

---

## Formats

### 1. POV You Just Downloaded

**Vibe**: Screen recording of first open — real reactions via voiceover, fresh discovery energy.

**Structure**:
- 0-3s: Phone in hand, thumb tapping the app icon for the first time
- 3-6s: App opens, first screen visible, person's face reflecting surprise/interest
- 6-8s: Scrolling through key features, natural exploration
- 8-10s: Genuine impressed reaction — raised eyebrows, slight nod

**Prompt Template**:
> POV of someone opening [APP NAME] for the first time on their phone. Their thumb taps the app icon, the app loads. The camera captures both the phone screen and their face — genuine curiosity turning into pleasant surprise as they explore [KEY FEATURE]. They scroll naturally, discovering features organically. The reaction is authentic, not performative. Bedroom or couch setting, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 2. App Made Me Do This

**Vibe**: Showing a real result/action the app enabled — casual storytime.

**Structure**:
- 0-3s: Person talking to camera, casual energy — "okay so this app…"
- 3-6s: Showing the result on their phone screen or in real life
- 6-8s: Quick flash of the app interface that made it happen
- 8-10s: Genuine pride/excitement about what they accomplished

**Prompt Template**:
> A person talking casually to the camera about something [APP NAME] helped them accomplish. They show [RESULT — e.g. a completed project, organized data, tracked goal] on their phone screen, then flash the app interface briefly. Their expression is genuinely proud and excited — this app actually changed something for them. Selfie angle, natural light, casual setting, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 3. Dark Mode Tour

**Vibe**: Late night in bed scrolling through app features — chill, intimate vibe.

**Structure**:
- 0-3s: Dim bedroom, person lying in bed, phone screen illuminating their face
- 3-6s: Slow scroll through app in dark mode, clean UI visible
- 6-8s: Tapping through different sections, exploring at night
- 8-10s: Content expression, settling deeper into pillow, still scrolling

**Prompt Template**:
> Late night scene — a person lying in bed in a dim room, the glow of their phone illuminating their face. They're slowly scrolling through [APP NAME] in dark mode. The clean, dark UI is visible as they tap through different features — [FEATURES]. They look content, relaxed, lost in the app. The vibe is late-night phone scroll before sleep. Dim lighting, vertical video, intimate. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 4. Before/After My Workflow

**Vibe**: Split showing the messy old way vs the clean new app way.

**Structure**:
- 0-3s: "Before" — chaotic scene of sticky notes, messy spreadsheet, frustrated expression
- 3-5s: Quick transition effect (swipe or cut)
- 5-8s: "After" — clean app dashboard, organized, same person looking relieved
- 8-10s: Satisfied lean back, everything handled

**Prompt Template**:
> Split before/after scene. BEFORE: a person surrounded by sticky notes, a messy spreadsheet on their laptop, looking frustrated and overwhelmed. Quick swipe transition. AFTER: the same person looking at [APP NAME] on their phone — clean, organized interface showing [KEY FEATURE]. They lean back with a relieved, satisfied expression. Everything is handled. Natural office/desk lighting, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 5. Notification Storytelling

**Vibe**: Phone buzzes with app notification — "wait this actually works."

**Structure**:
- 0-2s: Phone sitting on table, notification banner slides down from [APP]
- 2-5s: Hand picks up phone, reads notification, surprised expression
- 5-8s: Opens app to see the full context — it delivered on something
- 8-10s: Looking at camera with "no way" energy, genuinely impressed

**Prompt Template**:
> A phone sitting on a table buzzes with a notification from [APP NAME] — the banner shows [NOTIFICATION TEXT, e.g. "Your goal is complete" or "New result ready"]. A hand picks up the phone, the person reads it with a surprised expression. They open the app and see [RESULT]. They look up at the camera with genuine "wait, this actually works" energy. Natural setting, vertical video, candid reaction. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 6. Hidden Feature Reveal

**Vibe**: "Bet you didn't know it could do this" — screen recording energy.

**Structure**:
- 0-2s: Phone in hand, app already open, knowing smile
- 2-5s: Navigating to a non-obvious feature, tapping through menus
- 5-8s: Feature revealed — the "hidden gem" moment
- 8-10s: Impressed expression, tapping through it, mind blown energy

**Prompt Template**:
> A person holding their phone with [APP NAME] open, a knowing smile on their face like they're about to share a secret. They navigate through the app to a hidden or non-obvious feature — [HIDDEN FEATURE]. When they find it, their expression shifts to genuine excitement. They tap through it, exploring. The vibe is "I can't believe more people don't know about this." Close-up of phone and face, vertical video, natural light. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 7. 60-Second Setup

**Vibe**: Speedrun from download to first value — it's that quick.

**Structure**:
- 0-3s: App Store/Play Store, tapping "Download," progress bar
- 3-6s: Opening app, quick sign-up flow (sped up slightly)
- 6-10s: First meaningful action in the app — creating something, seeing a result
- 10-15s: Done. Leaning back, "that was it?" expression, impressed

**Prompt Template**:
> Speedrun of setting up [APP NAME]. Starting from the app store — tapping download, watching it install. Opening the app, breezing through sign-up (slightly sped up). Then the first real action — [FIRST ACTION, e.g. creating a project, setting a goal, scanning a document]. Everything happens fast and smooth. The person leans back with an impressed "that was it?" expression. The message is effortless onboarding. Screen recording energy, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "15"`

---

### 8. Day in My Life ft. App

**Vibe**: Vlog-style day where the app appears naturally at multiple touchpoints.

**Structure**:
- 0-3s: Morning — checking the app with coffee, casual glance
- 3-6s: Midday — using a feature during work/commute
- 6-9s: Evening — checking results or winding down with the app
- 9-12s: End of day, phone on nightstand, app notification visible

**Prompt Template**:
> A "day in my life" vlog where [APP NAME] appears naturally throughout. Morning: person checks the app while sipping coffee at their kitchen counter. Midday: they use [FEATURE] during a break, phone propped on desk. Evening: they review [RESULTS/STATS] on the couch. The app isn't the star — it's a natural part of their day. Vlog transitions, multiple settings, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "15"`

---

### 9. Rage Quit to Calm

**Vibe**: Frustrated with old tool, switches to app, immediate relief.

**Structure**:
- 0-3s: Visibly frustrated — typing angrily, sighing at laptop/old app
- 3-5s: Picks up phone, opens [APP NAME] with a "fine, let me try this" energy
- 5-8s: App interface loads, clean and simple, tension draining from face
- 8-10s: Relaxed smile, the thing that was hard is now easy

**Prompt Template**:
> A person visibly frustrated — sighing at their laptop, rubbing their temples, dealing with [OLD TOOL/METHOD]. They pick up their phone and open [APP NAME] with skeptical, last-resort energy. The app loads — clean, intuitive interface. Their expression softens immediately. Within seconds they've done what was frustrating them. Visible relief. The contrast between frustration and calm is the story. Desk setting, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 10. Screenshot Flex

**Vibe**: Showing screenshots of results/stats from the app — quiet pride.

**Structure**:
- 0-3s: Phone in hand, navigating to stats/results section
- 3-6s: Turning phone to show screen — impressive numbers or achievements
- 6-8s: Slight smile, nodding — letting the results speak
- 8-10s: Casually locking phone, confident energy

**Prompt Template**:
> A person holding their phone, navigating to the stats or results section of [APP NAME]. They turn the phone toward the camera to show [STATS — e.g. streak count, savings amount, project completions, fitness progress]. Their expression is quietly proud — a slight smile, a subtle nod. They let the numbers speak for themselves. No over-the-top reaction, just genuine satisfaction. Natural setting, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 11. Convince Me in 15s

**Vibe**: Fast-paced screen recording hitting every key feature — rapid fire.

**Structure**:
- 0-3s: App opens, immediately jumping into Feature 1
- 3-6s: Quick tap to Feature 2, then Feature 3
- 6-10s: Feature 4 and 5, each getting ~2 seconds
- 10-15s: Back to home screen, the whole package visible at once

**Prompt Template**:
> A rapid-fire tour of [APP NAME]. The app opens and immediately dives into [FEATURE 1], then quick-taps to [FEATURE 2], [FEATURE 3], [FEATURE 4], and [FEATURE 5] — each getting just a couple seconds. The pace is fast but not frantic, each feature clearly visible. Ends on the home screen showing the full, clean interface. The energy is "here's everything, and it all just works." Screen recording style, vertical video, slightly sped up. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "15"`

---

### 12. Widget Check

**Vibe**: Home screen widget glance throughout the day — it's always there.

**Structure**:
- 0-3s: Phone home screen visible, [APP] widget prominent among other apps
- 3-6s: Quick glance at widget info — a stat, status, or update
- 6-8s: Phone set down, going about their day
- 8-10s: Later — picking phone up again, widget shows updated info, satisfied glance

**Prompt Template**:
> A phone home screen with [APP NAME]'s widget visible among other apps. The person glances at the widget showing [WIDGET INFO — e.g. today's progress, a quick stat, upcoming task]. They set the phone down and go about their day. Later, they pick it up again — the widget has updated with new info. A quick satisfied glance. The app is passively useful, always there without demanding attention. Natural daily settings, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 13. Duo Reaction

**Vibe**: Showing a friend the app for the first time — capturing their genuine reaction.

**Structure**:
- 0-3s: Two people sitting together, one handing their phone to the other
- 3-6s: Friend looking at the app, eyebrows raising, "wait what?"
- 6-8s: Friend tapping through features, increasingly impressed
- 8-10s: Friend looking up — "where has this been?" expression

**Prompt Template**:
> Two friends sitting together on a couch. One hands their phone to the other, showing them [APP NAME]. The friend starts exploring — their eyebrows raise, they start tapping through [KEY FEATURES], getting more impressed with each screen. They look up from the phone with a "why didn't you show me this sooner" expression. Genuine reaction, natural chemistry between friends. Living room, casual setting, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 14. The Thing That Replaced

**Vibe**: "I used to use X, now I use this" — casual comparison, no drama.

**Structure**:
- 0-3s: Briefly showing old tool/app — maybe a dusty icon or closed tab
- 3-6s: Opening [APP NAME] instead, smooth transition
- 6-8s: Navigating through it naturally, doing the same task but better
- 8-10s: Small shrug — it just makes more sense now

**Prompt Template**:
> A person on their phone briefly showing [OLD APP/TOOL] — maybe scrolling past it, or closing it. Then they open [APP NAME] and do the same task — but smoother, cleaner, faster. They navigate through [KEY FEATURE] naturally. At the end, a casual shrug and slight smile — they switched and haven't looked back. No dramatic comparison, just a natural evolution. Close-up phone view, vertical video, natural light. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 15. Lock Screen Peek

**Vibe**: Notification lands on lock screen, unlocking to see what it does.

**Structure**:
- 0-2s: Phone face-up on table, lock screen visible, notification drops in
- 2-5s: Hand reaches for phone, reads the notification preview
- 5-8s: Unlocks phone, app opens to the relevant content
- 8-10s: Quick interaction — the notification was useful, satisfied

**Prompt Template**:
> A phone sitting face-up on a table. A notification from [APP NAME] slides onto the lock screen — "[NOTIFICATION PREVIEW TEXT]". A hand reaches for the phone, reads it, and unlocks to open the app. The app shows [RELEVANT CONTENT] — the notification led somewhere useful. Quick, satisfied interaction. The app is working in the background, surfacing things that matter. Clean desk or table setting, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`
