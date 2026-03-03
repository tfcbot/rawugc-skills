---
name: ugc-supplements
description: >-
  UGC video format templates for supplement brands. Contains 15 TikTok-native,
  lofi video formats with shot-by-shot structure and AI video generation prompts.
  Use when the user wants to create supplement UGC content — morning stacks,
  ingredient education, taste tests, or wellness routines.
requires:
  env:
    - RAWUGC_API_KEY
compatibility: >-
  Use alongside the rawugc-api skill for API endpoint knowledge.
  Requires RAWUGC_API_KEY.
homepage: https://github.com/tfcbot/rawugc-skills
source: https://github.com/tfcbot/rawugc-skills
---

# Supplements UGC Video Formats

15 lofi, TikTok-native video formats for supplement brands. Raw, authentic, easy to produce. No hard CTAs — these feel like real people sharing their actual wellness routines and honest takes on what they put in their body.

## How to Use These Formats

1. Identify the user's goal (product launch, ingredient education, routine showcase, social proof).
2. Select the format below that best matches.
3. Use the **Prompt Template** to compose the `prompt` field for `POST /videos/generate`. Replace `[BRACKETED]` placeholders with details from the user.
4. Default to `aspectRatio: "portrait"` (9:16) and `nFrames: "10"` unless the format specifies otherwise.
5. Keep the tone casual, genuine, unscripted. Supplement content needs to feel trustworthy above all — no exaggerated claims, just honest experience.

---

## Formats

### 1. Morning Stack

**Vibe**: Laying out all supplements on the counter — taking them one by one with coffee.

**Structure**:
- 0-3s: Kitchen counter, coffee brewing in background, supplement bottles lined up
- 3-6s: Opening each bottle, taking one at a time — methodical, routine
- 6-8s: [PRODUCT] gets a beat longer — the main character of the stack
- 8-10s: Sipping coffee, all supplements taken, ready for the day

**Prompt Template**:
> Morning supplement routine. A kitchen counter with coffee brewing and several supplement bottles lined up. A person opens each one and takes them methodically — [SUPPLEMENT LIST]. When they reach [PRODUCT] from [BRAND], they linger a moment longer — it's the key part of the stack. They wash it all down with coffee, looking energized and ready. Calm morning energy, warm kitchen light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 2. Gym Bag Dump

**Vibe**: Emptying the gym bag — showing what supplements make the cut.

**Structure**:
- 0-3s: Gym bag being unzipped and flipped over, contents spilling out
- 3-6s: Sorting through items — shaker bottle, towel, headphones
- 6-8s: [PRODUCT] pulled out, held up — "this always comes with me"
- 8-10s: Repacking, [PRODUCT] goes back in first — essential

**Prompt Template**:
> Gym bag dump. A person unzips their gym bag and tips it over — contents spill onto a table. Among the shaker bottle, headphones, and towel: [PRODUCT] from [BRAND]. They pick it up, hold it to the camera — it always makes the cut. They repack, putting [PRODUCT] in first. It's a gym essential. Post-workout energy, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 3. Smoothie Build

**Vibe**: Making a smoothie, casually adding the supplement — blending, taste reaction.

**Structure**:
- 0-3s: Ingredients on counter — fruit, milk, ice
- 3-5s: Dropping ingredients into blender one by one
- 5-7s: Adding [PRODUCT] — a scoop or pour, the key addition
- 7-10s: Blending, pouring into glass, first sip, genuine taste reaction

**Prompt Template**:
> Smoothie making scene. A kitchen counter with [SMOOTHIE INGREDIENTS — e.g. banana, berries, almond milk, ice]. A person drops each ingredient into a blender. Then they add [PRODUCT] from [BRAND] — [FORMAT, e.g. a scoop of powder, a pour of liquid]. They blend it, pour into a glass. First sip — genuine reaction. The supplement blends in naturally, both literally and as part of the routine. Bright kitchen, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 4. What I Take and Why

**Vibe**: Pointing at each bottle, one sentence each — casual education, no lecture.

**Structure**:
- 0-2s: All supplement bottles on counter or shelf
- 2-5s: Pointing at first bottle — quick one-liner explanation
- 5-7s: Pointing at [PRODUCT] — slightly more detail, it matters most
- 7-10s: Last bottle, done — "that's my stack"

**Prompt Template**:
> A person standing in front of their supplement lineup, casually explaining each one. They point at each bottle with a one-liner — [QUICK EXPLANATIONS, e.g. "this for energy," "this for gut health"]. When they reach [PRODUCT] from [BRAND], they spend a beat longer — [WHY THIS ONE MATTERS]. They finish with a casual "that's my stack." No lecture energy — just sharing what works for them. Kitchen or bathroom counter, natural light, selfie angle, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 5. Pill Organizer ASMR

**Vibe**: Filling a weekly pill organizer — satisfying clicking and sorting sounds.

**Structure**:
- 0-3s: Empty pill organizer open on table, bottles surrounding it
- 3-6s: Opening bottles, dropping pills/capsules into each day — satisfying clicks
- 6-8s: [PRODUCT] capsules going in — distinctive color or shape visible
- 8-10s: Closing each compartment — snap snap snap — organized and ready

**Prompt Template**:
> ASMR pill organizer video. An empty weekly pill organizer open on a clean surface, supplement bottles arranged around it. Hands open each bottle and drop pills into the daily compartments — satisfying clicking sounds as capsules hit plastic. [PRODUCT] from [BRAND] capsules are [DISTINCTIVE DETAIL — e.g. a bright green, distinctively shaped]. Each compartment snaps closed. Organized, satisfying, routine. Close-up tabletop shot, quiet room, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 6. 30-Day Check-In

**Vibe**: Talking to camera about what's changed since starting — honest, no miracle claims.

**Structure**:
- 0-3s: Face to camera — "okay so it's been 30 days on [PRODUCT]…"
- 3-6s: Honest assessment — what they've noticed, what's changed
- 6-8s: Showing the product, it has signs of regular use (half-empty bottle)
- 8-10s: Overall vibe — "I'm going to keep taking it" genuine conclusion

**Prompt Template**:
> 30-day supplement check-in. A person talking to camera — honest, casual tone. "It's been a month on [PRODUCT] from [BRAND]." They share what they've noticed — [HONEST OBSERVATIONS, e.g. "my energy in the afternoon is more consistent," "my skin has been better," "I sleep deeper"]. They show the bottle — it's half-used, clearly been part of daily life. No miracle claims, just honest experience. "I'm going to keep taking it." Natural light, selfie angle, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 7. Taste Test No Filter

**Vibe**: Trying it for the first time on camera — genuine face reaction, uncut.

**Structure**:
- 0-3s: Holding [PRODUCT], reading the flavor/label, curious expression
- 3-5s: Opening, smelling it first (if applicable)
- 5-8s: First taste/sip — genuine reaction, uncut, whatever happens happens
- 8-10s: Verdict — nodding approval, surprised, or honest "it's different" take

**Prompt Template**:
> First-time taste test of [PRODUCT] from [BRAND]. A person holds the [FORMAT — e.g. packet, bottle, scoop] and reads the flavor — [FLAVOR]. They open it, smell it. First taste — their face tells the whole story. Genuine, uncut reaction — [EXPECTED REACTION]. No second takes, no edits. Whatever the face does is the content. Real, honest, trustworthy. Close-up, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 8. The One I Actually Notice

**Vibe**: "I take a lot of stuff but THIS is the one I feel" — cutting through the noise.

**Structure**:
- 0-3s: Gesturing at a full shelf/counter of supplements — "I take all of these"
- 3-6s: Picking up [PRODUCT] specifically — "but this is the one I actually notice"
- 6-8s: Explaining what they feel — energy, sleep, mood, focus
- 8-10s: Setting it apart from the rest — it earned the spotlight

**Prompt Template**:
> A person gesturing at their full supplement shelf — "I take a lot of stuff." They reach past everything and pick up [PRODUCT] from [BRAND]. "But this is the one I actually feel a difference with." They explain — [WHAT THEY NOTICE, e.g. "my focus after lunch," "I actually stay asleep," "my recovery is faster"]. They set it back down, slightly in front of the others. It earned its spot. Casual, honest, selfie angle, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 9. Travel Supplement Kit

**Vibe**: Packing supplements for a trip — what makes the cut when space is limited.

**Structure**:
- 0-3s: Suitcase open, pill case or travel bag nearby
- 3-6s: Sorting through supplements, selecting the essentials for travel
- 6-8s: [PRODUCT] goes in — no debate, it always travels
- 8-10s: Travel kit packed, zipped, tossed in suitcase

**Prompt Template**:
> Packing supplements for a trip. An open suitcase, a small travel pill case or pouch. The person sorts through their supplement collection, choosing what makes the cut when space is limited. [PRODUCT] from [BRAND] goes in without hesitation — it's a travel non-negotiable. A few others join. The travel kit gets zipped and tossed in the suitcase. Not everything can come — but [PRODUCT] always does. Bedroom, natural light, packing energy, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 10. Post-Workout Ritual

**Vibe**: Immediately after gym — mixing or taking supplement while still sweaty.

**Structure**:
- 0-3s: Just finished working out — sweaty, breathing hard, gym or home gym setting
- 3-6s: Grabbing shaker bottle or [PRODUCT], mixing or taking it immediately
- 6-8s: Drinking/taking it — relief, refueling energy
- 8-10s: Leaning against wall or sitting, recovering, [PRODUCT] in hand

**Prompt Template**:
> Post-workout scene. A person just finished training — visibly sweaty, catching their breath in [SETTING — gym, garage gym, park]. They immediately grab [PRODUCT] from [BRAND] and [TAKE/MIX — e.g. scoop into shaker, drink pre-mixed, take capsules with water]. They drink it down, eyes closed for a second — refueling. They lean against a wall, recovering, [PRODUCT] in hand. Raw, real, no posing. Post-workout lighting, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 11. Reading the Label

**Vibe**: Flipping the bottle, pointing at key ingredients — "this is actually clean."

**Structure**:
- 0-3s: Holding [PRODUCT], flipping to the back — supplement facts panel
- 3-6s: Pointing at specific ingredients, reading key ones aloud
- 6-8s: Nodding at what's NOT on the label — no fillers, no junk
- 8-10s: Flipping back to front, satisfied — "this is clean"

**Prompt Template**:
> A person examining [PRODUCT] from [BRAND]. They flip the bottle to show the supplement facts panel. They point at key ingredients — [KEY INGREDIENTS] — nodding approvingly. They also note what's absent — [CLEAN LABEL NOTES, e.g. "no artificial sweeteners," "no fillers," "third-party tested"]. They flip the bottle back to the front with a satisfied expression — this passes the label test. Close-up, readable label, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 12. Nightstand Lineup

**Vibe**: Nighttime supplements on the bedside table — winding down for sleep.

**Structure**:
- 0-3s: Bedside table at night — lamp on, book, water glass, supplement bottles
- 3-6s: Picking up [PRODUCT], taking it with water
- 6-8s: Setting it back down, settling into bed
- 8-10s: Lamp clicks off, peaceful sleep energy, [PRODUCT] visible on nightstand

**Prompt Template**:
> Nighttime supplement routine. A cozy bedside table — warm lamp, a book, a glass of water, and [PRODUCT] from [BRAND] among other nighttime supplements. The person picks up [PRODUCT], takes it with water. They settle into bed, pulling covers up. The lamp clicks off. [PRODUCT] sits on the nightstand — part of the wind-down ritual. Warm, sleepy, intimate. Dim bedroom lighting, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 13. My Non-Negotiables

**Vibe**: The 3 supplements you'd never cut — explaining why, casually.

**Structure**:
- 0-3s: "If I could only take three things…" — face to camera
- 3-5s: First pick — quick explanation
- 5-7s: Second pick
- 7-10s: Third pick is [PRODUCT] — "and I'd never drop this one because…"

**Prompt Template**:
> "If I could only take three supplements" challenge. A person faces the camera. They pick their three non-negotiables from their collection. First: [PICK 1 — quick why]. Second: [PICK 2 — quick why]. Third: [PRODUCT] from [BRAND] — "and I'd never cut this because [REASON, e.g. it's the one I actually feel, it replaced three other things, nothing else does what this does]." The hierarchy is clear — [PRODUCT] is in the inner circle. Casual, opinionated, selfie angle, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 14. Fridge Door Reveal

**Vibe**: Opening the fridge to show where supplements live — organized or chaotic, both real.

**Structure**:
- 0-3s: Hand on fridge door handle, opening it
- 3-6s: Supplements visible in the fridge door or shelf — the real storage situation
- 6-8s: Grabbing [PRODUCT] from its spot — it has a home in there
- 8-10s: Taking it, closing fridge, carrying on with the day

**Prompt Template**:
> Fridge door supplement reveal. A hand opens the fridge — and there on the door shelf among the condiments sit supplement bottles. [ORGANIZED or CHAOTIC — whatever's real]. They grab [PRODUCT] from [BRAND] from its designated spot. They take it, close the fridge, and carry on. The message: this is where the supplements actually live. Real, unglamorous, authentic. Kitchen, fridge light glow, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 15. Vs My Old Brand

**Vibe**: Holding old brand and new side by side — explaining the switch honestly.

**Structure**:
- 0-3s: Holding two bottles — old brand in one hand, [PRODUCT] in the other
- 3-6s: Comparing them — label, ingredients, form factor
- 6-8s: Explaining what made them switch — better ingredients, results, value
- 8-10s: Setting old one aside, keeping [PRODUCT] — decision made

**Prompt Template**:
> Brand comparison. A person holds [OLD BRAND SUPPLEMENT] in one hand and [PRODUCT] from [BRAND] in the other. They compare — [COMPARISON POINTS, e.g. "this one has fillers, this one doesn't," "I was paying more for less with the old one," "the dosage is actually effective here"]. They explain why they switched — honest, not brand-bashing, just facts. They set the old one aside and keep [PRODUCT]. Decision made. Good lighting for label readability, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`
