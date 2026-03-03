---
name: ugc-b2c
description: >-
  UGC video format templates for general B2C products. Contains 15 TikTok-native,
  lofi video formats with shot-by-shot structure and AI video generation prompts.
  Use when the user wants to create B2C UGC content — product demos, honest reviews,
  lifestyle integrations, or comparison content for any consumer product.
requires:
  env:
    - RAWUGC_API_KEY
compatibility: >-
  Use alongside the rawugc-api skill for API endpoint knowledge.
  Requires RAWUGC_API_KEY.
homepage: https://github.com/tfcbot/rawugc-skills
source: https://github.com/tfcbot/rawugc-skills
---

# B2C UGC Video Formats

15 lofi, TikTok-native video formats for general B2C products. Raw, authentic, easy to produce. No hard CTAs — these work for any consumer product and feel like real people sharing things they genuinely use.

## How to Use These Formats

1. Identify the user's goal (product launch, social proof, comparison, lifestyle integration).
2. Select the format below that best matches.
3. Use the **Prompt Template** to compose the `prompt` field for `POST /videos/generate`. Replace `[BRACKETED]` placeholders with details from the user.
4. Default to `aspectRatio: "portrait"` (9:16) and `nFrames: "10"` unless the format specifies otherwise.
5. Keep the tone casual, genuine, unscripted. These should feel like someone sharing a real find with their group chat.

---

## Formats

### 1. Just Got This

**Vibe**: Immediate reaction to receiving or buying something — raw excitement, no prep.

**Structure**:
- 0-3s: Holding or unwrapping [PRODUCT], barely contained excitement
- 3-6s: First look — turning it over, examining quality and details
- 6-8s: First use or try — genuine "oh wow" moment
- 8-10s: Looking at camera, nodding — this was a good purchase

**Prompt Template**:
> A person just received [PRODUCT] from [BRAND]. They're holding it for the first time — excitement barely contained. They turn it over, examining the [DETAILS — e.g. build quality, design, packaging]. They use it for the first time — [FIRST USE ACTION]. Genuine impressed reaction. They look at the camera and nod — this was worth it. Unscripted, immediate, real. Living room or kitchen table, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 2. A Day With This

**Vibe**: The product follows you through a normal day — it's a background character in your life.

**Structure**:
- 0-3s: Morning — [PRODUCT] appears in morning context
- 3-6s: Midday — using it again, different setting
- 6-9s: Evening — one more touchpoint, it's always around
- 9-12s: End of day — product sitting where it lives, integrated into life

**Prompt Template**:
> A day-in-the-life featuring [PRODUCT] from [BRAND]. Morning: [MORNING USE — e.g. grabbing it on the way out, using it during breakfast]. Midday: [MIDDAY USE — e.g. at the office, during lunch, on a walk]. Evening: [EVENING USE — e.g. at home, unwinding, with friends]. The product is always there but never the focus — it's just part of a real day. Multiple settings, natural light transitions, vlog energy, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "15"`

---

### 3. The Comparison

**Vibe**: Your product vs the obvious alternative — honest, no-script take.

**Structure**:
- 0-3s: Both products side by side on a table
- 3-6s: Picking up each one, quick comparison — look, feel, build
- 6-8s: Using both — honest test, same task
- 8-10s: Verdict — [PRODUCT] wins naturally, no forced conclusion

**Prompt Template**:
> Honest product comparison. [PRODUCT] from [BRAND] next to [COMPETITOR/ALTERNATIVE]. A person examines both — [COMPARISON CRITERIA, e.g. build quality, design, feel in hand, performance]. They test both doing [SAME TASK]. The comparison is fair and honest. [PRODUCT] wins on [WINNING POINTS] — not forced, just demonstrated. Clean surface, good lighting for comparison, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 4. Hack I Found

**Vibe**: Unexpected way to use the product — "wait, try this."

**Structure**:
- 0-3s: Holding [PRODUCT], mischievous "I found something" expression
- 3-6s: Demonstrating the unexpected use or hack
- 6-8s: The hack working — satisfying result
- 8-10s: "You're welcome" energy, proud of the discovery

**Prompt Template**:
> Product hack video. A person holding [PRODUCT] from [BRAND] with a "watch this" expression. They demonstrate [UNEXPECTED USE/HACK — e.g. a secondary function, a creative way to use it, a tip that isn't obvious]. The hack works beautifully — satisfying result. They look at the camera with proud, "you're welcome" energy. The product is more versatile than people think. Close-up demonstration, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 5. Honest Pros and Cons

**Vibe**: Talking to camera, listing what you love and what's mid — full transparency.

**Structure**:
- 0-3s: "Okay here's my honest take on [PRODUCT]" — holding it up
- 3-6s: Pros — counting on fingers, genuine enthusiasm
- 6-8s: Cons — fair, minor, balanced
- 8-10s: Overall verdict — "pros way outweigh" authentic conclusion

**Prompt Template**:
> Honest pros and cons review. A person holding [PRODUCT] from [BRAND], talking directly to camera. Pros: [PROS — e.g. "the quality is insane," "it does exactly what it says," "the design is clean"]. Cons: [CONS — e.g. "wish it came in black," "took a couple days to ship," "slightly bigger than I expected"]. The cons are real but minor — the pros clearly outweigh. Transparent, trustworthy, balanced. Casual setting, selfie angle, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 6. Setup Timelapse

**Vibe**: Unbox to fully set up in a satisfying sped-up sequence.

**Structure**:
- 0-3s: Box on floor/table, opening begins
- 3-7s: Assembly/setup in progress — sped up 2-3x, satisfying progression
- 7-10s: Final product set up and in place — slows to normal speed
- 10-15s: First use, stepping back to admire, satisfied

**Prompt Template**:
> Setup timelapse of [PRODUCT] from [BRAND]. Starting with the box — opening, removing packaging. Assembly or setup sped up 2-3x — [SETUP STEPS, e.g. connecting pieces, placing components, plugging in, arranging]. When it's fully set up, the video slows to normal speed. The finished [PRODUCT] in its spot — clean, ready. First use moment. Stepping back to admire. Satisfying start-to-finish progression. Room or desk setting, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "15"`

---

### 7. The Sound It Makes

**Vibe**: ASMR focus on satisfying product sounds — clicks, zips, pours, snaps.

**Structure**:
- 0-3s: Close-up of [PRODUCT], anticipation
- 3-6s: The satisfying sound — [CLICK, ZIP, SNAP, POUR, WHIR]
- 6-8s: Repeat from different angle — same satisfying sound
- 8-10s: Final interaction, the sound is the hook

**Prompt Template**:
> ASMR product video focused on the sounds [PRODUCT] from [BRAND] makes. Close-up: [THE SOUND — e.g. the satisfying click of the lid, the zip of the case, the pour of the liquid, the snap of it locking in place]. The camera captures it from multiple angles — the sound is crisp, satisfying, oddly addictive. No talking, just the product's natural sounds. Extreme close-up, quiet room, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 8. Would I Rebuy

**Vibe**: Holding product after months of use — "here's my verdict after actually living with it."

**Structure**:
- 0-3s: Holding [PRODUCT] — it has signs of real use (wear, half-empty, etc.)
- 3-6s: Reflecting on months of use — what held up, what they love
- 6-8s: The verdict moment — "would I buy this again?"
- 8-10s: Confident yes (or honest qualification) — genuine conclusion

**Prompt Template**:
> Long-term review. A person holding [PRODUCT] from [BRAND] that's clearly been used — [SIGNS OF USE, e.g. some wear, half-empty, well-loved]. They talk about life with the product over [TIME PERIOD]. "Would I rebuy?" The verdict: [VERDICT — e.g. "absolutely, already have a backup," "yes, but I'd get the larger size next time"]. Genuine, informed by actual use, not first impressions. The trust comes from time with the product. Natural setting, selfie angle, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 9. Family Test

**Vibe**: Giving it to family members, collecting their genuine reactions.

**Structure**:
- 0-2s: "I'm going to let my family try [PRODUCT]" — setup
- 2-5s: First family member tries it — genuine reaction
- 5-8s: Second family member — different reaction, both honest
- 8-10s: Collecting verdicts — the product passed the family test (or didn't)

**Prompt Template**:
> Family product test. A person introduces [PRODUCT] from [BRAND] to their family — [FAMILY MEMBERS, e.g. mom, partner, sibling]. Each person tries it and gives a genuine reaction — [REACTIONS]. No coaching, no retakes. The reactions range from [REACTION RANGE — e.g. "surprised by the quality" to "immediately wanted their own"]. The family test is the ultimate credibility check. Home setting, candid, multiple reactions, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 10. Car Review

**Vibe**: Reviewing the product in your car — popular TikTok setting, casual drive-thru energy.

**Structure**:
- 0-3s: Sitting in parked car, holding [PRODUCT], car lighting
- 3-6s: Talking through the product — showing it, demonstrating features
- 6-8s: Using it in the car context — it works anywhere
- 8-10s: Casual verdict, tossing it on the passenger seat — approved

**Prompt Template**:
> Car review. A person sitting in their parked car, holding [PRODUCT] from [BRAND]. The car provides natural framing — window light, dashboard visible. They show the product, talk through [KEY FEATURES/IMPRESSIONS]. They use or demonstrate it — [CAR DEMO]. They casually toss it on the passenger seat — it's coming with them. The car setting adds intimacy and authenticity — classic TikTok review energy. Car interior, natural daylight through windows, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 11. The Thing That Fixed

**Vibe**: "I had this problem, this product fixed it" — simple storytime, genuine.

**Structure**:
- 0-3s: Describing the problem — relatable frustration, talking to camera
- 3-6s: "Then I found this" — introducing [PRODUCT]
- 6-8s: Showing how it solved the problem — demo or explanation
- 8-10s: Life after the fix — relief, satisfaction, problem gone

**Prompt Template**:
> Problem-solution storytime. A person talking to camera about [PROBLEM — e.g. a daily frustration, something that was broken, an unmet need]. Relatable, genuine frustration. "Then I found [PRODUCT] from [BRAND]." They show how it solved the problem — [SOLUTION DEMO]. The relief is visible. Life is better now, the problem is handled. Simple, effective storytelling. Casual setting, selfie angle, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 12. Durability Check

**Vibe**: Showing the product after heavy use — "still going strong" or honest wear report.

**Structure**:
- 0-3s: Holding [PRODUCT] — visible signs of real use over time
- 3-6s: Showing specific wear points — "here's how it's held up"
- 6-8s: Demonstrating it still works perfectly (or showing honest wear)
- 8-10s: Verdict on longevity — "built to last" energy

**Prompt Template**:
> Durability check. A person showing [PRODUCT] from [BRAND] after [TIME PERIOD] of regular use. They point out how it's held up — [DURABILITY NOTES, e.g. "no scratches," "the fabric hasn't pilled," "still works like day one," "some patina that actually looks cool"]. They demonstrate it still functioning perfectly. The message: this product is built to last and gets better with use. Close-up details, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 13. Gift Guide Energy

**Vibe**: "If you don't know what to get someone, this" — effortless recommendation.

**Structure**:
- 0-3s: "If you need a gift for [PERSON TYPE]…" — face to camera
- 3-6s: Holding up [PRODUCT], showing it off — it's a crowd-pleaser
- 6-8s: Quick demo of why it works as a gift — universal appeal
- 8-10s: "Trust me, they'll love it" — confident recommendation

**Prompt Template**:
> Gift guide content. A person talking to camera — "if you need a gift for [PERSON TYPE — e.g. your partner, a friend who has everything, your mom], get them this." They hold up [PRODUCT] from [BRAND], showing it off. Quick demo of why it's a great gift — [GIFT APPEAL, e.g. "it's useful but also looks premium," "everyone who sees it asks about it," "it's the kind of thing you wouldn't buy yourself"]. Confident recommendation energy. Casual setting, holiday or everyday vibe, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 14. POV You Own This

**Vibe**: First-person POV of daily life with the product — you're living it.

**Structure**:
- 0-3s: POV reaching for [PRODUCT] on shelf/counter/desk
- 3-6s: Using it in first-person — hands visible, product in action
- 6-8s: The result or satisfaction of using it
- 8-10s: Setting it down, moving on with your day — it just works

**Prompt Template**:
> First-person POV of owning [PRODUCT] from [BRAND]. The camera IS the person. Hands reach for [PRODUCT] on [LOCATION]. Using it — [USE IN POV, e.g. opening it, operating it, applying it, activating it]. The result is satisfying. Setting it back down and moving on. The message: this is what daily life with this product feels like — seamless, easy, good. POV camera, natural movements, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 15. The Aesthetic

**Vibe**: Product styled beautifully in its environment — no talking, vibes only.

**Structure**:
- 0-3s: [PRODUCT] in a beautifully styled setting — morning light, clean surface
- 3-6s: Slow pan or close-up, capturing texture, color, design details
- 6-8s: A hand enters frame, interacts gently — picks it up or adjusts it
- 8-10s: Final hero shot, product looking its best, pure visual vibes

**Prompt Template**:
> Pure aesthetic product video. [PRODUCT] from [BRAND] styled in a beautiful setting — [ENVIRONMENT, e.g. marble countertop with morning light, minimal desk with a plant, cozy bedside table]. Slow pan capturing the details — [DESIGN DETAILS, e.g. texture, color, form factor]. A hand gently enters frame and interacts with the product — picking it up, turning it slightly. Final hero shot. No talking, no text, just vibes. The product speaks for itself visually. Soft, warm lighting, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`
