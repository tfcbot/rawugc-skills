---
name: ugc-saas
description: >-
  UGC video format templates for SaaS products. Contains 15 TikTok-native,
  lofi video formats with shot-by-shot structure and AI video generation prompts.
  Use when the user wants to create SaaS UGC content — product demos, workflow showcases,
  founder stories, or results-driven content.
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

15 lofi, TikTok-native video formats for SaaS products. Raw, authentic, easy to produce. No hard CTAs — these feel like real professionals sharing tools they actually use in their workflow.

## How to Use These Formats

1. Identify the user's goal (product demo, workflow showcase, social proof, feature education).
2. Select the format below that best matches.
3. Use the **Prompt Template** to compose the `prompt` field for `POST /videos/generate`. Replace `[BRACKETED]` placeholders with details from the user.
4. Default to `aspectRatio: "portrait"` (9:16) and `nFrames: "10"` unless the format specifies otherwise.
5. Keep the tone casual, genuine, unscripted. These should feel like a coworker showing you something cool, not a sales demo.

---

## Formats

### 1. Emotional Hook + Demo

**Vibe**: Face to camera sharing a frustration, then flipping to screen demo of the fix.

**Structure**:
- 0-3s: Close-up face, relatable frustration — "I was so tired of doing X manually"
- 3-5s: Transition to screen — opening [PRODUCT] dashboard
- 5-8s: Quick demo of the feature that solves the pain point
- 8-10s: Back to face — relieved, satisfied expression

**Prompt Template**:
> A person talking directly to camera with genuine frustration — "I was spending hours on [PAIN POINT]." Their expression is relatable and tired. Quick cut to their laptop screen showing [PRODUCT] dashboard. They click through [KEY FEATURE] — the problem gets solved in seconds. Cut back to their face — visible relief and satisfaction. The contrast between pain and solution tells the story. Desk setting, natural light, selfie angle, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 2. Desk Setup ft. Product

**Vibe**: Aesthetic desk tour — product dashboard visible on screen, soft mention.

**Structure**:
- 0-3s: Wide shot of a clean, aesthetic desk setup — monitor, keyboard, plant
- 3-6s: Camera pans across the desk, landing on the monitor
- 6-8s: [PRODUCT] dashboard is open on screen, data/charts visible
- 8-10s: Person sits down, starts working, product is just part of the setup

**Prompt Template**:
> An aesthetic desk tour. Clean workspace — monitor, mechanical keyboard, coffee, a small plant. The camera pans slowly across the setup, settling on the monitor where [PRODUCT] dashboard is open — showing [DASHBOARD CONTENT, e.g. analytics, project boards, pipelines]. A person sits down and starts working naturally. [PRODUCT] isn't the focus — it's just part of a well-curated workspace. Warm lighting, vertical video, aesthetic productivity vibes. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 3. Workflow ASMR

**Vibe**: Satisfying screen recording of clicking through a clean UI — no voiceover, pure flow.

**Structure**:
- 0-3s: Cursor moving smoothly through [PRODUCT] interface
- 3-6s: Clicking through actions — creating, organizing, completing tasks
- 6-8s: Drag-and-drop or automation triggering, satisfying visual feedback
- 8-10s: Final state — everything organized, clean, done

**Prompt Template**:
> A satisfying screen recording of [PRODUCT] in action. A cursor moves smoothly through the clean interface — clicking, dragging, organizing. [WORKFLOW — e.g. moving cards on a kanban board, triggering an automation sequence, completing a batch of tasks]. Each click is satisfying, each transition smooth. No voiceover, no music — just the zen of a well-designed tool doing its job. The final state is clean and organized. Screen recording style, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 4. The 5pm Dashboard

**Vibe**: End of day, looking at results — genuine "wow, we did that" reaction.

**Structure**:
- 0-3s: Person leaning back in chair, end-of-day energy, checking laptop
- 3-6s: [PRODUCT] dashboard showing impressive daily/weekly metrics
- 6-8s: Close-up of specific numbers or charts that stand out
- 8-10s: Satisfied expression, closing laptop, work well done

**Prompt Template**:
> End of workday. A person leans back in their desk chair, stretching, then glances at their laptop. [PRODUCT] dashboard is open showing [METRICS — e.g. deals closed, tasks completed, revenue tracked, emails sent]. The numbers are impressive. Close-up of the dashboard, key metrics highlighted. They lean back with a satisfied, quiet "we did that" expression. Closes the laptop. Natural office/home office lighting, golden hour, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 5. Before This I Was Using Spreadsheets

**Vibe**: Cringe flashback to the old way, cut to clean dashboard — instant upgrade energy.

**Structure**:
- 0-3s: Showing a messy, color-coded spreadsheet — overwhelmed expression
- 3-5s: Dramatic close of laptop or tab, "never again" energy
- 5-8s: Opens [PRODUCT] — same data but organized, visual, clean
- 8-10s: Peaceful expression, the chaos is over

**Prompt Template**:
> A person grimacing at a chaotic spreadsheet on their screen — messy rows, confusing color codes, too many tabs. They dramatically close the tab. Opens [PRODUCT] instead — the same information but clean, visual, organized. [DASHBOARD VIEW — e.g. charts, kanban boards, clean tables]. Their expression shifts from stressed to peaceful. The spreadsheet era is over. Split between laptop screen and face reactions, natural light, vertical video. [ADDITIONAL DETAILS].

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

### 8. Automations Running

**Vibe**: Screen recording of automations firing — satisfying domino effect.

**Structure**:
- 0-3s: Automation trigger — a form submitted, a deal moved, a task completed
- 3-6s: Chain reaction — automated actions firing in sequence
- 6-8s: Results populating — emails sent, tasks created, data synced
- 8-10s: Final state — everything updated automatically, zero manual work

**Prompt Template**:
> A satisfying screen recording of [PRODUCT]'s automation in action. It starts with a trigger — [TRIGGER, e.g. a new form submission, a deal stage change]. Then automations cascade: [CHAIN — e.g. email sends, task creates, data syncs, notification fires]. Each step happens automatically, one after another like dominoes. The final state shows everything updated — zero manual intervention. Clean, efficient, mesmerizing. Screen recording, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 9. Onboarding Speedrun

**Vibe**: Sign up to first value in under 60 seconds — it's that smooth.

**Structure**:
- 0-3s: Landing page, clicking "Sign Up" or "Get Started"
- 3-7s: Quick onboarding flow — sped up slightly, clean steps
- 7-12s: First meaningful action — creating something, seeing first data
- 12-15s: "Done" moment — leaning back, impressed by how fast that was

**Prompt Template**:
> Speedrun of [PRODUCT] onboarding. Starting from the landing page — clicking sign up. The onboarding flow is quick and clean — [ONBOARDING STEPS, e.g. name, workspace, first project]. Slightly sped up. Within moments they're doing their first real action — [FIRST VALUE MOMENT]. They lean back, genuinely impressed by how fast they went from zero to productive. Screen recording mixed with face reactions, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "15"`

---

### 10. Slack Notification Moment

**Vibe**: Integration notification pops in — genuine "oh nice" excitement.

**Structure**:
- 0-2s: Working at desk, Slack/Teams open in background
- 2-5s: Notification pops in from [PRODUCT] integration — a result, alert, or update
- 5-8s: Reading the notification, expression shifts to impressed/pleased
- 8-10s: Quick click through to [PRODUCT] to see the full detail, satisfied

**Prompt Template**:
> A person working at their desk. A Slack notification pops up from [PRODUCT] — "[NOTIFICATION — e.g. 'New deal closed: $X', 'Report ready', 'Automation complete']". They read it, eyebrows raise — genuinely impressed. They click through to [PRODUCT] to see the full detail. Satisfied nod. The integration works silently in the background and surfaces wins. Natural desk setting, screen visible, vertical video. [ADDITIONAL DETAILS].

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

### 12. Side by Side

**Vibe**: Split screen of old way vs new way — no commentary needed, the visuals speak.

**Structure**:
- 0-3s: Left/top: the old way — spreadsheet, manual process, cluttered
- 3-5s: Right/bottom: [PRODUCT] — same task, clean, visual, fast
- 5-8s: Both running simultaneously, the contrast is stark
- 8-10s: Old way still loading/processing, [PRODUCT] already done

**Prompt Template**:
> Split-screen comparison. On one side: the old way of doing [TASK] — [OLD METHOD, e.g. messy spreadsheet, manual email chains, paper files]. On the other side: [PRODUCT] handling the same task — clean interface, organized data, fast execution. The contrast speaks for itself. The old method is still processing while [PRODUCT] is already done. No voiceover needed. Clean split-screen composition, vertical video. [ADDITIONAL DETAILS].

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

### 14. The Tab I Never Close

**Vibe**: Showing browser tabs — this one's always open, casual flex.

**Structure**:
- 0-3s: Browser with multiple tabs open, cursor moving across them
- 3-6s: Landing on [PRODUCT] tab — it's pinned, always there
- 6-8s: Quick peek at what's on the dashboard right now
- 8-10s: Moving on to other work, but that tab stays open

**Prompt Template**:
> Close-up of a browser with multiple tabs open. The cursor moves across them — email, docs, calendar. Then it lands on [PRODUCT] — pinned tab, always open. Quick glance at the dashboard showing [CURRENT VIEW]. The person moves on to other work, but [PRODUCT] stays pinned. It's the tab that never closes — always running, always useful. Screen recording style with slight face cam, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 15. Team Sync Moment

**Vibe**: Quick collaboration moment showing shared workspace — natural, not staged.

**Structure**:
- 0-3s: Two people at a desk or screen, casually looking at [PRODUCT] together
- 3-6s: One pointing at something on screen, the other nodding
- 6-8s: Quick interaction in [PRODUCT] — assigning a task, leaving a comment, updating status
- 8-10s: Both nodding, aligned, moving on to execute

**Prompt Template**:
> Two coworkers casually looking at [PRODUCT] on a laptop screen together. One points at [FEATURE — e.g. a task, a pipeline stage, a report]. The other nods. A quick action — [ACTION, e.g. assigning a task, updating a status, leaving a comment]. They're aligned in seconds. The vibe is efficient collaboration, not a formal meeting. Natural office or coworking space, candid energy, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`
