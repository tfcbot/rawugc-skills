---
name: ugc-skincare
description: >-
  UGC video format templates for skincare brands. Contains 20 TikTok-native,
  lofi video formats with shot-by-shot structure and AI video generation prompts.
  Use when the user wants to create skincare UGC content — routines, texture shots,
  ingredient education, or product showcases.
requires:
  env:
    - RAWUGC_API_KEY
compatibility: >-
  Use alongside the rawugc-api skill for API endpoint knowledge.
  Requires RAWUGC_API_KEY.
homepage: https://github.com/tfcbot/rawugc-skills
source: https://github.com/tfcbot/rawugc-skills
---

# Skincare UGC Video Formats

20 lofi, TikTok-native video formats for skincare brands. Raw, authentic, easy to produce. No hard CTAs — these feel like real people sharing real routines.

## How to Use These Formats

1. Identify the user's goal (routine showcase, product launch, ingredient education, social proof).
2. Select the format below that best matches.
3. Use the **Prompt Template** to compose the `prompt` field for `POST /videos/generate`. Replace `[BRACKETED]` placeholders with details from the user.
4. Default to `aspectRatio: "portrait"` (9:16) and `nFrames: "10"` unless the format specifies otherwise.
5. Keep the tone casual, genuine, unscripted. These should never feel like ads.

---

## Formats

### 1. GRWM ASMR Routine

**Vibe**: Silent broll of a full skincare routine — close-up textures, no talking, pure ASMR.

**Structure**:
- 0-2s: Hands reaching for first product on a bathroom counter, natural morning light
- 2-5s: Close-up of product being dispensed onto fingertips, creamy texture visible
- 5-8s: Gentle application to face, slow circular motions, skin glistening
- 8-10s: Final product applied, person looking in mirror with a subtle satisfied expression

**Prompt Template**:
> A young woman in a naturally lit bathroom performing her morning skincare routine. Close-up shots of her hands applying [PRODUCT] to her face. The texture of the [PRODUCT TEXTURE — e.g. cream, serum, gel] is visible on her fingertips. No talking, ASMR energy — you can almost hear the soft sounds of product on skin. Smartphone quality, vertical video, warm soft lighting. The vibe is calm, unhurried, genuine. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 2. Shelfie Tour

**Vibe**: POV showing your bathroom shelf, casually picking up each product and putting it back.

**Structure**:
- 0-3s: Camera pans across a bathroom shelf lined with skincare products
- 3-6s: Hand picks up [PRODUCT], holds it to camera briefly
- 6-8s: Sets it back, picks up another, casual browsing energy
- 8-10s: Returns to [PRODUCT], lingering shot — the star of the shelf

**Prompt Template**:
> POV shot of a hand browsing a bathroom shelf filled with skincare products. Natural lighting, real bathroom setting. The hand picks up [PRODUCT] and holds it toward the camera, showing the label. Casual, like someone showing a friend their collection. The camera lingers on [PRODUCT] — it's clearly the favorite. Vertical smartphone video, authentic UGC aesthetic. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 3. Texture Porn

**Vibe**: Extreme close-up of product texture on skin — satisfying swatch and spread.

**Structure**:
- 0-3s: Product squeezed onto back of hand, thick satisfying dollop
- 3-6s: Finger swirls through the texture slowly
- 6-8s: Spread onto skin, showing absorption and finish
- 8-10s: Clean skin with a subtle glow, product bottle in soft focus behind

**Prompt Template**:
> Extreme close-up of [PRODUCT] being squeezed onto the back of a hand. The [TEXTURE — e.g. thick cream, lightweight serum, whipped mousse] catches the light. A finger slowly swirls through it, then spreads it across the skin. The camera captures every detail of the texture — satisfying, almost meditative. Natural daylight, vertical video, macro lens energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 4. Morning Routine Speedrun

**Vibe**: Sped-up morning skincare routine in 15 seconds — real bathroom, natural light.

**Structure**:
- 0-4s: Quick splash of water on face (sped up 2x)
- 4-8s: Rapid application of cleanser, toner, serum (each ~1.5s)
- 8-12s: [PRODUCT] application — slows to normal speed for this one, hero moment
- 12-15s: Final look in mirror, fresh-faced, grabbing keys and heading out

**Prompt Template**:
> A person speedrunning their morning skincare routine in a bright bathroom. Everything is slightly sped up — splashing water, applying cleanser, patting on toner. When they reach [PRODUCT], the video slows to normal speed, highlighting the application moment. They look fresh and glowing. The energy is fun, efficient, relatable. Smartphone quality, vertical, natural light. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "15"`

---

### 5. Night Routine Wind-Down

**Vibe**: Dimly lit, cozy vibes — slow application, ASMR tapping on bottles.

**Structure**:
- 0-3s: Warm lamp-lit bathroom or bedroom vanity, candle flickering in background
- 3-6s: Fingers tapping on product bottle (ASMR energy), then opening it
- 6-8s: Slow, luxurious application to face, eyes closed
- 8-10s: Settling into bed/pillow, skin glowing, peaceful expression

**Prompt Template**:
> A cozy nighttime skincare scene. Warm lamp lighting, a candle in the background. A person gently taps on the bottle of [PRODUCT] before opening it — satisfying ASMR energy. They apply [PRODUCT] slowly to their face, eyes closed, savoring the moment. The vibe is end-of-day peace. They settle back onto a pillow with glowing skin. Vertical video, dim warm lighting, intimate. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 6. Skin Check-In Vlog

**Vibe**: Talking to camera about how skin has been, holding product casually.

**Structure**:
- 0-3s: Face close to camera, natural light, no makeup — "okay so my skin lately…"
- 3-6s: Gesturing at skin, pointing to areas of concern or improvement
- 6-8s: Casually holds up [PRODUCT], "this has been helping though"
- 8-10s: Applying it while still talking, genuine and unscripted energy

**Prompt Template**:
> A person sitting in natural light, face close to the camera, talking casually like a vlog. They're gesturing at their skin — pointing at their cheeks and forehead. They casually hold up [PRODUCT] and start applying it while talking. No makeup, genuine expression, like they're updating a friend about their skin journey. Vertical smartphone selfie-style video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 7. This or That

**Vibe**: Holding two products side by side, pointing to the one you actually use.

**Structure**:
- 0-3s: Both hands holding a product each, camera facing both
- 3-5s: Looks at one, looks at the other — playful indecision
- 5-8s: Puts one down decisively, holds [PRODUCT] up with a knowing nod
- 8-10s: Opens [PRODUCT] and starts applying, case closed

**Prompt Template**:
> A person holding two skincare products side by side — [PRODUCT] in one hand, a competitor in the other. They look back and forth playfully, pretending to decide. Then they put the other one down and hold up [PRODUCT] with a confident smile. They open it and start applying. The vibe is casual, fun, decisive. Natural lighting, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 8. Empty Jar Reveal

**Vibe**: Showing a fully used-up product — "had to rebuy" energy.

**Structure**:
- 0-3s: Holding up an empty jar/bottle, scraping the last bit out
- 3-6s: Camera shows how completely empty it is — tipped upside down
- 6-8s: Reveal of the brand new replacement, fresh and unopened
- 8-10s: Opening the new one, first scoop/pump, satisfying full-product moment

**Prompt Template**:
> A person holding up a completely empty jar of [PRODUCT], scraping the last bits out with their finger. They tip it upside down to show it's truly gone. Then they reveal a brand new, unopened [PRODUCT] — the replacement. They open it and take the first scoop, showing the fresh, full texture. The energy is "couldn't live without this." Natural lighting, vertical video, genuine excitement. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 9. Fridge Skincare

**Vibe**: Opening a mini skincare fridge, pulling out the star product.

**Structure**:
- 0-3s: Hand reaching for a small pastel mini-fridge, opening the door
- 3-6s: Reveal of neatly organized skincare products inside, cold mist visible
- 6-8s: Hand selects [PRODUCT] from the fridge, holds it up
- 8-10s: Pressing the cold product against cheek, satisfying "ahhh" expression

**Prompt Template**:
> Close-up of a hand opening a small pastel mini-fridge on a vanity counter. Inside, skincare products are neatly arranged and slightly dewy from the cold. The hand reaches in and pulls out [PRODUCT]. They press the chilled [PRODUCT] against their cheek with a refreshed, satisfied expression. Aesthetic, organized, satisfying. Vertical video, soft lighting. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 10. Ingredient Decoded

**Vibe**: Casual explainer pointing at ingredient list — "this is the one that actually works."

**Structure**:
- 0-3s: Holding product bottle, flipping it to show the back/ingredients
- 3-6s: Finger pointing at a specific ingredient on the label
- 6-8s: Tapping the ingredient name emphatically, nodding
- 8-10s: Flips bottle back to front, applies product, confident expression

**Prompt Template**:
> A person holding [PRODUCT] and flipping it around to show the ingredient list on the back. They point at a specific ingredient — [KEY INGREDIENT, e.g. niacinamide, hyaluronic acid] — tapping it with their finger and nodding knowingly. They flip the bottle back to the front and start applying the product. The vibe is casual education, like telling a friend a secret. Natural light, vertical video, close-up. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 11. 3-Step Only

**Vibe**: "My entire routine is 3 products" — minimal routine flex.

**Structure**:
- 0-2s: Three products lined up on counter, clean and minimal
- 2-5s: Pick up first product, quick application, set down
- 5-8s: Second product, same energy
- 8-12s: Third product is [PRODUCT], slightly longer application — the star
- 12-15s: Fresh face, done. That's it. Simple.

**Prompt Template**:
> Three skincare products lined up neatly on a clean bathroom counter. A person picks up each one in sequence and applies it quickly — cleanser, then toner, then [PRODUCT]. The application of [PRODUCT] lingers slightly longer, the hero of the routine. They finish and look at the camera with a fresh, glowing face. The message is simplicity — this is all you need. Minimal, clean aesthetic, vertical video, natural light. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "15"`

---

### 12. Sunscreen Reapply

**Vibe**: Midday reapplication, outdoors or car mirror — casual PSA energy.

**Structure**:
- 0-3s: Sitting in car or outdoors, pulling [PRODUCT] from bag
- 3-6s: Checking face in mirror/phone camera, squinting at skin
- 6-8s: Applying sunscreen over makeup/existing skincare, patting it in
- 8-10s: Satisfied nod, tossing product back in bag, heading out

**Prompt Template**:
> A person sitting in their car (or outdoors in daylight) pulling [PRODUCT — sunscreen] out of their bag. They check their face in the car mirror, then squeeze out sunscreen and pat it onto their face over their existing makeup. Quick, casual, no fuss. They nod approvingly, toss it back in their bag. Midday light, real setting, vertical video, effortless PSA energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 13. Skin Diary

**Vibe**: Sequence showing skin over days/weeks — no pressure, just documenting.

**Structure**:
- 0-3s: Day 1 — close-up of bare skin, natural light, no filter
- 3-6s: Day 7 — same angle, same lighting, subtle changes visible
- 6-9s: Day 14 — clearer improvement, same framing
- 9-12s: Day 30 — noticeable glow, person touches face and smiles
- 12-15s: [PRODUCT] bottle shown casually on counter in background

**Prompt Template**:
> A skin transformation diary. Close-up of a person's bare face on Day 1 — natural light, no makeup, honest. The same shot repeats for Day 7, Day 14, and Day 30, each time showing gradual improvement in skin clarity and glow. The framing stays consistent. On the final frame, the person touches their face and smiles. [PRODUCT] is visible on the bathroom counter in the background — never the focus, just present. Vertical video, documentary style. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "15"`

---

### 14. No-Makeup Makeup Prep

**Vibe**: Skincare as the base — natural "glass skin" result, no makeup needed.

**Structure**:
- 0-3s: Starting with bare, clean face
- 3-6s: Layering hydrating products — toner, serum
- 6-8s: [PRODUCT] application, the glow builder
- 8-10s: Final result — dewy, glass skin, no makeup. Person admires the finish.

**Prompt Template**:
> A person starting with a bare, clean face and layering skincare to achieve a glass-skin glow. They apply toner, then serum, then [PRODUCT] as the final step. The camera catches the dewy, luminous finish on their skin — no makeup, just skincare doing the work. They tilt their face to catch the light and admire the result. Bathroom mirror setting, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 15. Unpacking Haul

**Vibe**: Opening a skincare delivery, first impressions, genuine reactions.

**Structure**:
- 0-3s: Package on table/bed, hands pulling tape, opening box
- 3-6s: Pulling out products one by one, holding each up briefly
- 6-8s: [PRODUCT] gets an excited reaction — opening it immediately, smelling it
- 8-10s: First swatch on hand, genuine "ooh" expression

**Prompt Template**:
> A person sitting on their bed opening a skincare delivery package. They pull products out one by one, holding each up to the camera. When they get to [PRODUCT], their face lights up — they immediately open it, smell it, and swatch it on the back of their hand. Genuine excitement, not performative. Natural bedroom lighting, vertical video, real unboxing energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 16. Travel Minis

**Vibe**: Packing a dopp kit, showing what skincare makes the cut for a trip.

**Structure**:
- 0-3s: Open suitcase or travel bag on bed, toiletry bag open
- 3-6s: Selecting products from a larger collection, putting some aside
- 6-8s: [PRODUCT] goes straight in — no debate, it always comes
- 8-10s: Zipping up the travel bag, ready to go

**Prompt Template**:
> A person packing a toiletry bag for a trip. Their full skincare collection is spread on the bed. They pick through it, selecting only the essentials. [PRODUCT] goes straight into the bag without hesitation — it always makes the cut. They zip up the travel bag, looking satisfied with their curated selection. Bedroom setting, natural light, vertical video, travel prep energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 17. Slugging Routine

**Vibe**: Nighttime heavy moisturizer/occlusive routine — cozy, glistening skin.

**Structure**:
- 0-3s: Bedroom at night, soft warm lighting, pajamas on
- 3-6s: Applying a thick layer of [PRODUCT] to face, generous amount
- 6-8s: Close-up of glistening, slug-like sheen on skin
- 8-10s: Lying back on pillow, skin absolutely glowing, cozy vibes

**Prompt Template**:
> A cozy nighttime scene. A person in pajamas sitting on their bed, warm lamp light. They scoop out a generous amount of [PRODUCT] and apply a thick, glossy layer all over their face. Close-up shows the glistening, dewy sheen — full slug mode. They lie back on their pillow with a content expression, skin absolutely glowing. Intimate, cozy, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 18. Maskimize

**Vibe**: Sheet mask on, just vibing — watching TV, scrolling phone. Product placement is passive.

**Structure**:
- 0-3s: Person applying a sheet mask, adjusting it on their face
- 3-6s: Sitting on couch with mask on, scrolling phone or watching TV, totally relaxed
- 6-8s: Peeling off mask, skin underneath looks hydrated and plump
- 8-10s: [PRODUCT] serum/cream visible on the coffee table — it was there the whole time

**Prompt Template**:
> A person applying a sheet mask and then casually lounging on their couch — scrolling their phone, watching TV, completely relaxed. After a few moments they peel the mask off, revealing hydrated, plump skin underneath. [PRODUCT] sits on the coffee table nearby, visible but not the focus — it's just part of the scene. The vibe is self-care without trying hard. Living room, evening light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 19. Derm Said This

**Vibe**: "My dermatologist told me to do this" — storytime while applying product.

**Structure**:
- 0-3s: Talking to camera, animated expression — "okay so my derm said…"
- 3-6s: Holding up [PRODUCT], gesturing at it while explaining
- 6-8s: Applying it to face, still talking, demonstrating the technique
- 8-10s: Finished applying, pointing at camera — "trust me on this one"

**Prompt Template**:
> A person talking directly to the camera with animated, storytelling energy — like they're sharing a secret their dermatologist told them. They hold up [PRODUCT] and gesture at it excitedly. They start applying it to their face while still talking, showing the application technique. They point at the camera at the end — sharing genuine advice. Close-up selfie angle, natural light, vertical video, authentic energy. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 20. One Product Wonder

**Vibe**: Entire video dedicated to one product — why it's the only one you need.

**Structure**:
- 0-3s: [PRODUCT] sitting alone on a clean surface, hero shot
- 3-5s: Picking it up, showing all angles — label, texture, size
- 5-8s: Applying it, close-up of skin absorbing it
- 8-10s: Holding it up to camera one more time, satisfied nod — this is it

**Prompt Template**:
> A single product hero video. [PRODUCT] sits alone on a clean, minimal surface — beautifully lit. A hand picks it up, rotates it to show the label and packaging. They open it and apply [PRODUCT] to their face — close-up of the texture absorbing into skin. They hold it up to the camera one final time with a confident, satisfied expression. Clean, minimal, focused. One product is all you need. Vertical video, soft natural light. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`
