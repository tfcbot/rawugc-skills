---
name: ugc-fashion
description: >-
  UGC video format templates for fashion brands. Contains 20 TikTok-native,
  lofi video formats with shot-by-shot structure and AI video generation prompts.
  Use when the user wants to create fashion UGC content — OOTDs, try-on hauls,
  styling videos, or outfit showcases.
requires:
  env:
    - RAWUGC_API_KEY
compatibility: >-
  Use alongside the rawugc-api skill for API endpoint knowledge.
  Requires RAWUGC_API_KEY.
homepage: https://github.com/tfcbot/rawugc-skills
source: https://github.com/tfcbot/rawugc-skills
---

# Fashion UGC Video Formats

20 lofi, TikTok-native video formats for fashion brands. Raw, authentic, easy to produce. No hard CTAs — these feel like real people showing how they actually dress.

## How to Use These Formats

1. Identify the user's goal (new collection launch, styling inspiration, size-inclusive showcase, seasonal content).
2. Select the format below that best matches.
3. Use the **Prompt Template** to compose the `prompt` field for `POST /videos/generate`. Replace `[BRACKETED]` placeholders with details from the user.
4. Default to `aspectRatio: "portrait"` (9:16) and `nFrames: "10"` unless the format specifies otherwise.
5. Keep the tone casual, genuine, unscripted. These should feel like someone showing their friend what they're wearing.

---

## Formats

### 1. Mirror OOTD

**Vibe**: Classic mirror outfit check — simple spin, natural lighting, main character energy.

**Structure**:
- 0-3s: Standing in front of a full-length mirror, phone visible in reflection
- 3-6s: Slow reveal from feet up, showing the full outfit
- 6-8s: A casual spin or turn, showing the back and sides
- 8-10s: Final pose — confident, effortless, looking at the mirror

**Prompt Template**:
> A person standing in front of a full-length mirror taking an OOTD photo/video. They're wearing [OUTFIT DESCRIPTION — e.g. oversized blazer, wide-leg pants, and loafers]. The camera (phone in reflection) slowly captures the outfit from shoes up. They do a casual spin showing all angles. The vibe is confident but effortless — they know they look good. Natural bedroom/hallway lighting, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 2. Try-On in Real Time

**Vibe**: Getting dressed on camera — genuine first reaction to how it fits.

**Structure**:
- 0-3s: Holding up the piece on a hanger, showing it flat
- 3-6s: Putting it on — pulling over head, buttoning up, zipping
- 6-8s: First look in mirror or camera — genuine reaction to the fit
- 8-10s: Adjusting, smoothing, final satisfied expression

**Prompt Template**:
> A person holding up [GARMENT] on a hanger, showing it to the camera. They start putting it on — [DRESSING ACTION, e.g. pulling it over their head, buttoning it up, stepping into it]. First look at themselves — genuine surprise at how well it fits. They adjust and smooth the fabric, checking different angles. Real, unscripted reaction energy. Bedroom setting, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 3. 3 Ways to Style

**Vibe**: Same piece, 3 completely different outfits — quick transitions.

**Structure**:
- 0-2s: Look 1 — the piece styled casually (jeans + sneakers)
- 2-5s: Quick transition cut
- 5-7s: Look 2 — dressed up (heels + accessories)
- 7-10s: Quick transition cut
- 10-12s: Look 3 — unexpected styling (layered, tied differently)
- 12-15s: All three looks in rapid succession

**Prompt Template**:
> The same [GARMENT] styled three completely different ways. Look 1: casual — paired with [CASUAL COMBO, e.g. jeans and sneakers]. Quick transition. Look 2: dressed up — [ELEVATED COMBO, e.g. heels, statement jewelry]. Quick transition. Look 3: unexpected — [CREATIVE COMBO, e.g. layered over a dress, tied at the waist]. Each look is a full outfit in a mirror or against a clean wall. Fast transitions, same person, same piece, three vibes. Vertical video, natural light. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "15"`

---

### 4. Closet Dig

**Vibe**: Rummaging through closet, pulling out the piece — "found it" energy.

**Structure**:
- 0-3s: Hands pushing through hangers in a closet, searching
- 3-5s: Pulling out [GARMENT] — "this one" moment
- 5-8s: Holding it up, admiring it, maybe pressing it against body
- 8-10s: Walking toward mirror to try it on, excited energy

**Prompt Template**:
> A person rummaging through a full closet, pushing hangers aside, searching for something specific. They pull out [GARMENT] with a "found it" expression — holding it up, admiring it. They press it against their body in the mirror, head tilted, already styling it mentally. They head to try it on. The energy is getting-ready excitement, real closet chaos. Natural bedroom light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 5. Fit Check Walk

**Vibe**: Walking toward camera in the outfit — street or hallway, confident energy.

**Structure**:
- 0-3s: Camera at end of hallway or sidewalk, person walking toward it
- 3-6s: Full outfit visible as they approach, each step confident
- 6-8s: Getting closer — details of fabric, fit, accessories visible
- 8-10s: Walk past camera, slight turn/look back

**Prompt Template**:
> A person walking confidently down a [SETTING — hallway, sidewalk, corridor] toward the camera. They're wearing [OUTFIT DESCRIPTION]. Each step is confident, natural. As they get closer, details become visible — the way [GARMENT] drapes, the accessories, the shoes. They walk past the camera with a slight backward glance. Main character energy, effortless. Natural outdoor or indoor light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 6. Unboxing Try-On

**Vibe**: Opening a fashion package, holding up items, immediately putting them on.

**Structure**:
- 0-3s: Package on bed/table, tearing open, pulling out tissue paper
- 3-5s: First garment out — holding up, genuine "oh" reaction
- 5-8s: Immediately trying it on — no waiting, need to see it now
- 8-10s: Mirror check with the new piece on, pleasantly surprised

**Prompt Template**:
> A person sitting on their bed, opening a fashion package from [BRAND]. They pull apart tissue paper and lift out [GARMENT]. Immediate genuine reaction — eyes widening, holding it up to see the full piece. They throw it on right away, too excited to wait. Quick mirror check — pleasantly surprised by the fit. Unscripted, real excitement. Bedroom, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 7. Day to Night Transition

**Vibe**: Same base outfit, swap a few pieces, go from daytime to evening.

**Structure**:
- 0-3s: Daytime look — casual, clean, work-appropriate
- 3-5s: Quick transition — swapping shoes, adding jewelry, changing a layer
- 5-8s: Evening look — elevated, going-out energy
- 8-10s: Confident walk out or final mirror check, ready for the night

**Prompt Template**:
> Day-to-night outfit transition. Starting with a daytime look — [DAY OUTFIT, e.g. blazer, simple top, trousers, flats]. Quick transition: swapping [CHANGES — e.g. flats for heels, adding statement earrings, switching blazer for leather jacket]. The evening look emerges — same base, elevated vibe. Final mirror check, going-out confidence. The transformation is subtle but effective. Natural to warm evening lighting transition, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 8. Thrift Flip Energy

**Vibe**: Taking a piece that looks basic on the hanger and styling it into a full look.

**Structure**:
- 0-3s: Holding up a plain/basic-looking garment — "trust me on this"
- 3-6s: Pairing it with unexpected pieces — layering, tucking, accessorizing
- 6-8s: The full styled look revealed — way better than expected
- 8-10s: Proud reveal, the transformation energy

**Prompt Template**:
> A person holding up [GARMENT] that looks plain and basic on the hanger — nothing special. They start styling it — [STYLING STEPS, e.g. tucking it into high-waisted pants, adding a belt, layering a jacket, rolling the sleeves]. Piece by piece, the outfit comes together. Final reveal — the look is unexpectedly fire. Proud expression, "told you" energy. Bedroom or closet setting, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 9. What I Actually Wore This Week

**Vibe**: Rapid montage of real daily outfits — honest, not curated.

**Structure**:
- 0-2s: Monday outfit — quick mirror selfie
- 2-4s: Tuesday — different setting, different vibe
- 4-6s: Wednesday — maybe more casual
- 6-8s: Thursday — stepping it up
- 8-12s: Friday — best outfit of the week
- 12-15s: Quick flash through all five again

**Prompt Template**:
> A week-of-outfits montage. Monday: [MONDAY OUTFIT] — quick mirror shot. Tuesday: [TUESDAY OUTFIT] — different energy. Wednesday: [WEDNESDAY OUTFIT] — casual day. Thursday: [THURSDAY OUTFIT] — elevated. Friday: [FRIDAY OUTFIT] — the best look of the week, lingering a beat longer. Each day is a quick 2-second clip in a different setting. Rapid fire, real, not overly curated. All featuring pieces from [BRAND]. Multiple locations, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "15"`

---

### 10. Size Honest

**Vibe**: "I'm a size X and here's how this actually fits" — genuine, no filter.

**Structure**:
- 0-3s: Talking to camera, stating their size/measurements honestly
- 3-6s: Showing the garment — front, side, back angles
- 6-8s: Pointing out fit details — where it's snug, where it drapes
- 8-10s: Final honest verdict — genuine thumbs up or "runs a little big" energy

**Prompt Template**:
> A person talking to camera — "I'm a size [SIZE] and here's how [GARMENT] from [BRAND] actually fits." They turn to show front, side, and back views. They point out specifics — [FIT DETAILS, e.g. "the waist sits here," "it's a little loose in the shoulders," "perfect length"]. Honest, helpful, no filter. Their verdict is genuine. Good lighting to see the real fit and fabric. Natural setting, vertical video, selfie-to-mirror angles. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 11. Rain Day Fit

**Vibe**: Styled for the weather — practical but still cute, real conditions.

**Structure**:
- 0-3s: Looking out window at rain/overcast weather
- 3-6s: Getting dressed for it — layering, grabbing a jacket, choosing shoes
- 6-8s: Full outfit in mirror — weather-appropriate and stylish
- 8-10s: Walking out the door into the real weather, outfit holding up

**Prompt Template**:
> A rainy day outfit video. Person looks out the window at overcast skies, then starts getting dressed. They layer [OUTFIT — e.g. trench coat, knit sweater, waterproof boots from BRAND]. Mirror check — practical but cute. They step outside into real rain — the outfit works, they look good despite the weather. The message is: bad weather doesn't mean bad style. Natural overcast lighting, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 12. Airport Outfit

**Vibe**: Travel OOTD — comfort meets style, real travel setting.

**Structure**:
- 0-3s: Packing or zipping suitcase, dressed and ready to go
- 3-6s: Full outfit check in hallway mirror — comfortable but put-together
- 6-8s: Walking through airport/station, carry-on in hand
- 8-10s: Sitting at gate or in car, outfit looks good after hours of wear

**Prompt Template**:
> Airport outfit showcase. A person zips their suitcase, already dressed in [TRAVEL OUTFIT — e.g. matching set, oversized hoodie and bike shorts, linen pants and sneakers from BRAND]. Quick mirror check — comfortable and stylish. Walking through the airport with a carry-on, the outfit moves well. Sitting at the gate — still looks put-together after hours of travel. Comfort-meets-style energy. Airport/travel settings, natural fluorescent + daylight, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 13. The Uniform

**Vibe**: "I wear this combo every week" — signature look showcase, consistency over trends.

**Structure**:
- 0-3s: Reaching for the same pieces in the closet — muscle memory
- 3-6s: Putting the combination together, well-practiced ease
- 6-8s: The uniform assembled — it just works, every time
- 8-10s: Confident walk out, this is their look and they own it

**Prompt Template**:
> A person reaching into their closet with zero hesitation — they know exactly what they're grabbing. [THE UNIFORM — e.g. white tee, black blazer, straight-leg jeans, and loafers from BRAND]. They get dressed with practiced ease, everything fitting perfectly. The combination is simple but intentional — this is their go-to, their signature. They walk out with quiet confidence. The vibe is consistency over trends. Natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 14. Accessory Stack

**Vibe**: Building a look from accessories up — rings, chains, bags, close-ups.

**Structure**:
- 0-2s: Clean hands/neck, bare starting point
- 2-5s: Adding pieces one by one — ring, then bracelet, then chain
- 5-8s: Each addition in close-up, satisfying stacking
- 8-10s: Full accessory look assembled, pulling back to show the complete outfit

**Prompt Template**:
> Close-up accessory stacking video. Starting bare — clean hands, bare neck. One by one: [ACCESSORIES — e.g. gold ring, then chain bracelet, then layered necklaces, then watch, then bag from BRAND]. Each piece added in extreme close-up, satisfying layering. The camera pulls back to show the full accessory look with the outfit. Minimal, intentional, each piece matters. Close-up to medium shot, soft lighting, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 15. Color Story

**Vibe**: Entire outfit in one color family — aesthetic broll, visual harmony.

**Structure**:
- 0-3s: First piece — in the color (e.g., all earth tones, all cream, all black)
- 3-6s: Adding matching pieces, same color palette throughout
- 6-8s: Full monochromatic or tonal outfit assembled
- 8-10s: Aesthetic broll — walking, posing, the color harmony is the star

**Prompt Template**:
> A monochromatic outfit video in [COLOR FAMILY — e.g. all cream, head-to-toe black, earth tones]. Piece by piece: [OUTFIT PIECES from BRAND] — all in the same tonal range. The full outfit assembled is visually harmonious, satisfying. Aesthetic broll shots — walking slowly, fabric catching the light, the color story is the hero. Clean backgrounds that complement the palette. Vertical video, soft golden light. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 16. Hand-Me-Up

**Vibe**: Styling a piece borrowed from a friend, partner, or parent — making it your own.

**Structure**:
- 0-3s: Holding up the borrowed piece — "stole this from my [person]"
- 3-6s: Putting it on, immediately making it work with their own style
- 6-8s: The borrowed piece looks completely different on them — elevated
- 8-10s: Confident result, the piece has a new life

**Prompt Template**:
> A person holding up [GARMENT] — something clearly borrowed. "Stole this from my [PERSON — e.g. dad, partner, roommate]" energy. They put it on and immediately make it their own — [STYLING, e.g. rolling the sleeves, belting it, pairing with heeled boots]. The oversized/borrowed piece looks completely elevated and intentional on them. New context, new outfit, same piece. Casual bedroom setting, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 17. Get Ready With Me Silent

**Vibe**: No talking, just getting dressed — music only, aesthetic cuts.

**Structure**:
- 0-3s: Laying out outfit pieces on bed, flat lay
- 3-6s: Getting dressed — pulling on each piece, close-ups of fabric
- 6-9s: Accessories going on — watch, jewelry, belt
- 9-12s: Final mirror look, adjusting, ready to go
- 12-15s: Walking out the door, complete look in motion

**Prompt Template**:
> A silent GRWM fashion video. No talking, just vibes. [OUTFIT PIECES from BRAND] laid out on a bed. The person gets dressed piece by piece — close-ups of fabric textures, buttons being done, sleeves being rolled. Accessories added — [ACCESSORIES]. Final mirror check, small adjustments. They walk out the door looking complete. The entire video is visual — music-video energy without words. Warm bedroom lighting, aesthetic cuts, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "15"`

---

### 18. In My X Era

**Vibe**: Leaning into a trend or aesthetic identity — "in my [aesthetic] era."

**Structure**:
- 0-3s: Text or face-to-camera declaring the era — "in my quiet luxury era" etc.
- 3-6s: Outfit that perfectly embodies the aesthetic
- 6-8s: Styled details — the specific touches that sell the vibe
- 8-10s: Full aesthetic moment — walking, posing, living the era

**Prompt Template**:
> "In my [ERA/AESTHETIC — e.g. quiet luxury, coastal grandmother, dark academia, clean girl] era" energy. A person wearing [OUTFIT from BRAND] that perfectly embodies the aesthetic. Close-ups of the styling details that sell it — [DETAILS, e.g. cashmere texture, specific shoes, particular accessories]. They're fully in the vibe — walking, posing, living it. The outfit isn't just clothes, it's a whole mood. Aesthetic-appropriate setting, vertical video, dreamy lighting. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 19. That Girl Outfit

**Vibe**: Aspirational but attainable everyday outfit — soft morning energy.

**Structure**:
- 0-3s: Morning setting — clean space, natural light pouring in
- 3-6s: Getting dressed in a put-together but effortless outfit
- 6-8s: Grabbing coffee, bag, heading out — "that girl" energy
- 8-10s: Walking out into the day, looking effortlessly assembled

**Prompt Template**:
> "That girl" morning routine outfit. A clean, bright space — morning light streaming in. The person gets dressed in [OUTFIT from BRAND] — [DESCRIPTION, e.g. matching set, clean sneakers, minimal jewelry]. Everything is intentional but not try-hard. They grab their coffee and tote bag, heading out the door with effortless "I have my life together" energy. Aspirational but attainable. Bright, clean aesthetic, morning light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 20. Returns vs Keeps

**Vibe**: Trying on multiple items, sorting honestly into keep and return piles.

**Structure**:
- 0-2s: Multiple packages or items laid out on bed
- 2-5s: First item try-on — honest reaction, sort into keep or return
- 5-8s: Second item — same process, genuine evaluation
- 8-11s: Third item from [BRAND] — clearly a keeper, face lights up
- 11-15s: Final tally — showing the keep pile, [BRAND] piece prominently there

**Prompt Template**:
> A fashion haul sorting video. Multiple items from different brands laid out on a bed. The person tries each on, giving honest reactions. Some go to the return pile with a head shake. When they try on [GARMENT from BRAND], their face lights up — immediate keeper. They continue through the rest. Final shot: the keep pile is curated and [BRAND] piece is front and center. Honest, unsponsored energy — the product earned its spot. Bedroom, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "15"`
