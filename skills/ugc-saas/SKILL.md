---
name: ugc-saas
description: >-
  UGC video format templates for SaaS products. Contains 15 TikTok-native,
  lofi video formats with shot-by-shot structure and AI video generation prompts.
  Focused on people talking about, reacting to, and advocating for SaaS tools —
  never showing screens, dashboards, or UI. Use when the user wants to create
  SaaS UGC content — passionate recommendations, founder stories, or personal
  reactions to tools they love.
requires:
  env:
    - RAWUGC_API_KEY
compatibility: >-
  Use alongside the rawugc-api skill for API endpoint knowledge.
  Requires RAWUGC_API_KEY.
homepage: https://github.com/tfcbot/rawugc-skills
source: https://github.com/tfcbot/rawugc-skills
---

# SaaS UGC Video Formats

15 lofi, TikTok-native video formats for SaaS products. Raw, authentic, easy to produce. No hard CTAs — these feel like real professionals sharing tools they actually use. All formats focus on the PERSON — talking to camera, reacting, gesturing, celebrating — never showing actual screens, dashboards, or UI recordings. Think "founder talking about their stack" not "screen recording walkthrough."

## How to Use These Formats

1. Identify the user's goal (product demo, workflow showcase, social proof, feature education).
2. Select the format below that best matches.
3. Use the **Prompt Template** to compose the `prompt` field for `POST /videos/generate`. Replace `[BRACKETED]` placeholders with details from the user.
4. Default to `aspectRatio: "portrait"` (9:16) and `nFrames: "10"` unless the format specifies otherwise.
5. Keep the tone casual, genuine, unscripted. These should feel like a coworker showing you something cool, not a sales demo.

---

## Formats

### 1. The Tool I Won't Shut Up About

**Vibe**: Talking to camera about the one SaaS tool you keep recommending — passionate, genuine advocacy.

**Structure**:
- 0-3s: Face to camera, sitting at desk — "my coworkers are sick of me talking about this"
- 3-6s: Holding up phone/gesturing — explaining what it does in plain terms
- 6-8s: Getting more animated — the specific thing that makes it special
- 8-10s: Leaning in — "seriously just try it" — genuine conviction

**Prompt Template**:
> A person sitting at their desk, face to camera — "my [AUDIENCE, e.g. coworkers, team, friends] are genuinely sick of me talking about this." Holding up phone or gesturing while explaining what [PRODUCT] does in plain terms. Getting more animated about [KEY DIFFERENTIATOR] — the specific thing that makes it special. Leaning in with genuine conviction — "seriously just try it." Home office, natural light, vertical video, passionate recommendation energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 2. Desk Tour Namecheck

**Vibe**: Casual desk tour, namecheck each tool in the stack — the SaaS product gets the hero spot.

**Structure**:
- 0-3s: Camera panning across a clean desk setup — monitor, keyboard, coffee
- 3-6s: Hand pointing at different things casually, naming them
- 6-8s: Hand gestures toward the laptop/screen — "[PRODUCT] lives here"
- 8-10s: Leaning back in chair, hands behind head — the setup is complete

**Prompt Template**:
> Camera panning across a clean [SETTING, e.g. home office, studio] desk — monitor, keyboard, [DESK ITEMS]. Hand pointing at items casually, naming the tools in the stack. Hand gestures toward the laptop — "and [PRODUCT] basically lives here permanently." Leaning back in the chair, hands behind head — the setup is dialed. Natural light, vertical video, desk tour energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 3. The Laptop Close

**Vibe**: End of workday — closing the laptop lid with satisfaction because the tool handled everything.

**Structure**:
- 0-3s: Person at desk, typing final keystrokes, looking satisfied
- 3-6s: Leaning back, stretching, glancing at the time — done early
- 6-8s: Reaching forward and slowly closing the laptop lid — satisfying click
- 8-10s: Standing up, grabbing coffee mug, walking away — day is done

**Prompt Template**:
> A person at their desk, typing final keystrokes with a satisfied expression. Leaning back and stretching, glancing at the clock — done earlier than expected thanks to [PRODUCT] keeping everything on track. Reaching forward and slowly closing the laptop lid — satisfying click. Standing up and grabbing their [ITEM, e.g. coffee mug, jacket], heading out. [SETTING], [LIGHTING], vertical video, end-of-day satisfaction energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 4. The "Before This Tool" Rant

**Vibe**: Talking to camera about how bad things were before this SaaS tool — relatable frustration turned relief.

**Structure**:
- 0-3s: Face to camera, exasperated expression — "before I found [PRODUCT]…"
- 3-6s: Counting frustrations on fingers, animated storytelling
- 6-8s: Expression shifts to relief — "and then I found this"
- 8-10s: Relaxed, leaning back — "haven't thought about that problem since"

**Prompt Template**:
> A person face to camera with an exasperated expression — recounting [PAIN POINT] before [PRODUCT]. Counting frustrations on their fingers — [FRUSTRATIONS, e.g. the manual process, the errors, the wasted time]. Expression shifts to visible relief — "and then I found [PRODUCT]." Relaxed, leaning back — "haven't thought about [PROBLEM] since." Home office, natural light, vertical video, before-and-after storytelling energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 5. The Stack Ranking

**Vibe**: Casually ranking your SaaS tools — the product gets top billing.

**Structure**:
- 0-3s: Sitting at desk, talking to camera — "my top 3 tools right now"
- 3-6s: Counting: "#3 is good, #2 is great…"
- 6-8s: "#1 — and it's not even close" — naming [PRODUCT] with emphasis
- 8-10s: Nodding definitively — the ranking is final

**Prompt Template**:
> A person sitting at their desk, talking to camera — "my top [NUMBER] tools right now." Counting on fingers: "[TOOL #3] — solid. [TOOL #2] — really great." Then with emphasis — "Number one, and it's not close — [PRODUCT]." Nodding definitively, the ranking is final. Home office, natural light, vertical video, hot take energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 6. Standup Vlog

**Vibe**: Casual morning energy — "today I'm using X to tackle Y."

**Structure**:
- 0-3s: Morning setting — coffee in hand, sitting at desk, "alright, today's plan…"
- 3-6s: Quick glance at [PRODUCT] showing today's tasks or pipeline
- 6-8s: Pointing at specific items, casual prioritization
- 8-10s: Nodding, grabbing coffee, ready to work — "let's go"

**Prompt Template**:
> Morning standup energy. A person sitting at their desk with coffee, talking casually to camera — "okay, here's what I'm tackling today." They glance at [PRODUCT] on their screen showing [TODAY'S VIEW — e.g. task list, pipeline, calendar]. They point at a few items, casually prioritizing. They grab their coffee and nod — ready to start. Relaxed morning energy, not corporate. Home office, natural morning light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 7. Client Win Storytime

**Vibe**: Talking to camera about a win — product is the quiet hero of the story.

**Structure**:
- 0-3s: Excited face to camera — "so I just closed this deal…" or "client just said…"
- 3-6s: Telling the story, animated gestures, genuine excitement
- 6-8s: Brief flash of [PRODUCT] screen showing the data/workflow that helped
- 8-10s: Back to face — "honestly couldn't have done it without this"

**Prompt Template**:
> A person talking excitedly to camera — telling the story of a recent win. "[CLIENT WIN STORY — e.g. closed a big deal, hit a milestone, got amazing client feedback]." Animated gestures, genuine energy. Quick flash of [PRODUCT] on their laptop screen showing [RELEVANT DATA]. Back to their face — gratitude and pride. The product helped but it's not the star — the win is. Selfie angle, natural light, casual energy, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 8. The Meeting That Could've Been

**Vibe**: Talking about time saved — the meeting/process [PRODUCT] eliminated entirely.

**Structure**:
- 0-3s: Person at desk, gesturing at an empty calendar/notebook — "we used to have a whole meeting for this"
- 3-6s: Shaking head at the absurdity, leaning forward
- 6-8s: Holding up phone — "[PRODUCT] just does it automatically now"
- 8-10s: Shrug, satisfied smile — "got an hour of my life back every week"

**Prompt Template**:
> A person at their desk, gesturing at an empty [PROP, e.g. notebook, calendar] — "we used to have a whole meeting for [TASK]." Shaking their head at the absurdity, leaning forward. Holding up their phone — "[PRODUCT] just handles it automatically now." Satisfied shrug and smile — "got [TIME SAVED] back every week." Home office, natural light, vertical video, time-saved celebration energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 9. The Walk-Away Test

**Vibe**: Talking about how the tool works even when you're not paying attention — set it and forget it.

**Structure**:
- 0-3s: Person at desk, gesturing at closed laptop — "I set this up on Monday"
- 3-6s: "Haven't touched it since" — hands up, backing away slightly
- 6-8s: "And it's been running perfectly" — impressed with their own setup
- 8-10s: Finger guns at camera — "that's how you know it's the right tool"

**Prompt Template**:
> A person at their desk, gesturing at their closed laptop — "I set this up on [TIME]." Hands up, backing away slightly — "haven't touched it since." Impressed expression — "and [PRODUCT]'s been [RUNNING TASK] perfectly." Finger guns at camera — "that's how you know it's the right tool." Home office, natural light, vertical video, set-it-and-forget-it energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 10. The Coffee Machine Pitch

**Vibe**: Casually explaining [PRODUCT] like you're pitching it to a coworker at the coffee machine — informal, persuasive.

**Structure**:
- 0-3s: Person standing, holding coffee, casual posture — "okay so basically…"
- 3-6s: Hand gestures while explaining simply — no jargon, plain language
- 6-8s: "And the best part is…" — the killer feature, delivered casually
- 8-10s: Sips coffee, shrugs — "just works"

**Prompt Template**:
> A person standing in their [SETTING, e.g. kitchen, break room] holding a coffee mug, casual posture — "okay so basically…" Hand gestures while explaining [PRODUCT] in plain terms — no jargon, just simple language. "And the best part is [KILLER FEATURE]." Sips coffee with a shrug — "just works." [SETTING], [LIGHTING], vertical video, watercooler pitch energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 11. Founder POV

**Vibe**: Building and running a business — product is a natural part of the stack.

**Structure**:
- 0-3s: "Day in my life as a founder" energy — morning routine, heading to work
- 3-6s: At desk, [PRODUCT] open among other tools — checking metrics, managing pipeline
- 6-8s: Quick action in [PRODUCT] — moving a deal, sending a follow-up, checking data
- 8-10s: Back to building — product fades into the workflow naturally

**Prompt Template**:
> A "day in the life of a founder" vibe. Morning coffee, sitting down at a busy desk. [PRODUCT] is open on the screen alongside other tools — it's part of the stack. The founder checks [METRICS/FEATURES] in [PRODUCT], takes a quick action — [ACTION]. Then moves on to other work. The product isn't highlighted — it's just there, essential but understated. Founder energy, busy but in control. Natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 12. The Whiteboard Moment

**Vibe**: Scribbling on a whiteboard/notebook about the tool's impact — visual thinking, casual.

**Structure**:
- 0-3s: Person standing at a whiteboard or holding a notebook, marker in hand
- 3-6s: Scribbling a quick before/after — rough, casual, not polished
- 6-8s: Pointing at the "after" side, tapping it — "[PRODUCT] did this"
- 8-10s: Stepping back, capping the marker — the proof is simple

**Prompt Template**:
> A person standing at a [SURFACE, e.g. small whiteboard, notebook] in their office, marker in hand. Scribbling a quick rough sketch — "before" on one side, "after" on the other showing [BEFORE/AFTER CONTRAST]. Pointing at the after side and tapping it — "[PRODUCT] did this." Stepping back and capping the marker — the proof is simple and visual. Home office, natural light, vertical video, visual thinker energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 13. Friday Wrap-Up

**Vibe**: End of week reflection — showing weekly stats, quiet satisfaction.

**Structure**:
- 0-3s: Friday afternoon energy — relaxed posture, casual outfit
- 3-6s: Opening [PRODUCT] weekly summary or dashboard
- 6-8s: Scrolling through highlights — tasks completed, goals hit, metrics up
- 8-10s: Closing laptop with satisfaction, weekend mode activated

**Prompt Template**:
> Friday afternoon. A person in casual clothes, relaxed energy, opening [PRODUCT] for a weekly wrap-up. The dashboard shows the week's highlights — [WEEKLY METRICS, e.g. tasks completed, deals progressed, goals achieved]. They scroll through with quiet pride. Numbers are up. They close the laptop with a satisfied expression — good week. Weekend energy kicks in. Home office, afternoon light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 14. The Group Chat Moment

**Vibe**: Talking about how you introduced [PRODUCT] to your team/group chat — the viral spread.

**Structure**:
- 0-3s: Face to camera, amused — "I sent this to our team Slack…"
- 3-6s: "…and within a week everyone was using it"
- 6-8s: Counting on fingers the people who switched
- 8-10s: Proud expression — "I'm basically their sales team at this point"

**Prompt Template**:
> A person face to camera, amused — "I sent [PRODUCT] to our [CHANNEL, e.g. team Slack, group chat]." Expression shifts — "within a week [ADOPTION DETAIL, e.g. every single person had switched]." Counting on fingers the converts. Proud expression — "I'm basically their sales team at this point and they're not paying me." Home office, natural light, vertical video, grassroots evangelism energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 15. The Solo Celebration

**Vibe**: Small private celebration at desk — fist pump, chair spin — because the tool just saved the day.

**Structure**:
- 0-3s: Person at desk, looking at laptop screen, tension on their face
- 3-6s: Expression shifts to relief, then excitement — it worked
- 6-8s: Small fist pump, maybe a chair spin — private celebration
- 8-10s: Composing themselves, leaning back cool — "all under control"

**Prompt Template**:
> A person at their desk, looking at their laptop with tension on their face. Expression shifts to relief, then excitement — [SUCCESS MOMENT, e.g. the deployment went through, the report generated, the campaign launched] thanks to [PRODUCT]. Small fist pump, a quick chair spin — private victory celebration. Composing themselves and leaning back cool — "all under control." Home office, natural light, vertical video, small-win celebration energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`
