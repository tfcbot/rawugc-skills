---
name: ugc-dtc
description: >-
  UGC video format templates for DTC (direct-to-consumer) brands. Contains 15
  TikTok-native, lofi video formats with shot-by-shot structure and AI video
  generation prompts. Use when the user wants to create DTC UGC content —
  unboxings, product rituals, honest reviews, or lifestyle integrations.
requires:
  env:
    - RAWUGC_API_KEY
compatibility: >-
  Use alongside the rawugc-api skill for API endpoint knowledge.
  Requires RAWUGC_API_KEY.
homepage: https://github.com/tfcbot/rawugc-skills
source: https://github.com/tfcbot/rawugc-skills
---

# DTC UGC Video Formats

15 lofi, TikTok-native video formats for DTC brands. Raw, authentic, easy to produce. No hard CTAs — these feel like real people sharing products that genuinely became part of their life.

## How to Use These Formats

1. Identify the user's goal (product launch, unboxing experience, repeat purchase story, brand loyalty content).
2. Select the format below that best matches.
3. Use the **Prompt Template** to compose the `prompt` field for `POST /videos/generate`. Replace `[BRACKETED]` placeholders with details from the user.
4. Default to `aspectRatio: "portrait"` (9:16) and `nFrames: "10"` unless the format specifies otherwise.
5. Keep the tone casual, genuine, unscripted. These should feel like someone who genuinely bought this with their own money.

---

## Formats

### 1. Unboxing Moment

**Vibe**: Opening the package — tissue paper, first touch, genuine reaction to the experience.

**Structure**:
- 0-3s: Package on table, hands pulling at tape/opening the box
- 3-6s: Tissue paper unwrapped, first reveal of product inside
- 6-8s: Picking up [PRODUCT], turning it over, feeling the quality
- 8-10s: Genuine reaction — nodding, impressed by packaging and product

**Prompt Template**:
> A person sitting at a table, opening a delivery package from [BRAND]. They pull at the tape, open the box, unwrap tissue paper. [PRODUCT] is revealed inside — they pick it up, turning it over in their hands, examining the packaging and quality. Their reaction is genuine — pleasantly surprised, impressed. The unboxing experience matters and this one delivers. Kitchen or living room table, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 2. My Honest Take

**Vibe**: Stream of consciousness review — product in hand, talking to camera, no script.

**Structure**:
- 0-3s: Holding [PRODUCT], casual setting, talking directly to camera
- 3-6s: Walking through what they like — pointing at details, demonstrating
- 6-8s: One thing they'd note — honest but not negative, balanced
- 8-10s: Overall verdict — genuine nod, "yeah I'd recommend this"

**Prompt Template**:
> A person holding [PRODUCT] from [BRAND], talking casually to camera like they're telling a friend about it. They point out what they love — [POSITIVE DETAILS, e.g. the texture, the design, how it works]. They mention one honest observation — [HONEST NOTE, e.g. "wish it came in more colors" or "took a day to get used to"]. Final verdict is genuine approval. Unscripted, stream-of-consciousness energy. Casual setting, natural light, selfie angle, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 3. Kitchen Counter Demo

**Vibe**: Product in its natural habitat — casual use while cooking, eating, or prepping.

**Structure**:
- 0-3s: Kitchen scene, counter with everyday items, [PRODUCT] among them
- 3-6s: Using [PRODUCT] casually as part of a routine — cooking, eating, prepping
- 6-8s: Close-up of the product in use — functional, easy, integrated
- 8-10s: Back to the scene — product sits naturally in the kitchen, belongs there

**Prompt Template**:
> A kitchen scene. [PRODUCT] from [BRAND] sits on the counter among other everyday items. A person uses it casually — [USE CASE, e.g. adding it to their morning coffee, using it while cooking, grabbing it during meal prep]. Close-up of the product in action. It's not the star of the scene — it just belongs there, integrated into daily life. Warm kitchen lighting, lived-in counter, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 4. Subscription Day

**Vibe**: Monthly box arrives — ritual of opening it, what's inside this time.

**Structure**:
- 0-3s: Walking to door or mailbox, picking up the familiar package
- 3-6s: Sitting down, opening it — "it's that time again" energy
- 6-8s: Pulling items out one by one, showing each briefly
- 8-10s: Everything laid out, satisfied with the haul, ready to use

**Prompt Template**:
> Subscription day ritual. A person grabs the familiar [BRAND] package from their door. They sit down and open it with "it's that time of the month" excitement. They pull out each item — [ITEMS] — showing each to the camera briefly. Everything laid out on the table, a satisfying spread. They're genuinely happy with what they got. Cozy home setting, natural light, recurring-customer energy, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 5. The Restock

**Vibe**: "Ran out, had to reorder" — showing empty next to the fresh replacement.

**Structure**:
- 0-3s: Holding up the empty/almost-empty product — squeezing the last drops
- 3-5s: Setting empty next to brand new replacement
- 5-8s: Opening the new one — fresh, full, satisfying
- 8-10s: First use of the restock, relieved "I was running low" energy

**Prompt Template**:
> A person holding up a nearly empty [PRODUCT] from [BRAND] — squeezing out the very last bit. They set the empty one down and reveal a brand new replacement next to it. They open the fresh one — full, clean, satisfying. First use from the restock. The message is clear: this product gets used up and repurchased. Not a first-time buy — a repeat. Natural setting, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 6. Gift Reaction

**Vibe**: Giving [PRODUCT] to someone and capturing their genuine reaction.

**Structure**:
- 0-3s: Handing a wrapped or boxed [PRODUCT] to someone
- 3-6s: They open it — genuine surprise, reading the label, examining it
- 6-8s: Trying it or using it for the first time — real reaction
- 8-10s: Both people happy — the gift was a hit

**Prompt Template**:
> A person handing [PRODUCT] from [BRAND] as a gift to [RECIPIENT — e.g. friend, partner, parent]. The recipient opens it — genuine surprise and curiosity. They examine it, read the label, then try it or use it. Their reaction is authentic — impressed, happy, grateful. Both people are smiling. The product makes a great gift and it shows. Living room or kitchen, natural light, candid energy, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 7. Morning Ritual

**Vibe**: Product integrated into a calm morning routine — not the star, just part of the scene.

**Structure**:
- 0-3s: Waking up, soft morning light, stretching
- 3-6s: Moving through morning routine — coffee, [PRODUCT] used casually
- 6-8s: [PRODUCT] in use — brief, natural, not highlighted
- 8-10s: Heading out or settling into the day, morning routine complete

**Prompt Template**:
> A calm morning routine. Person wakes up in soft morning light, stretches, heads to the kitchen. They go through their routine — making coffee, [USING PRODUCT from BRAND] as a natural part of the flow. The product isn't the focus — it's just there, integrated. The morning is the vibe: peaceful, intentional, real. The product earns its place by being useful, not by being the center of attention. Warm morning light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 8. Expectation vs Reality

**Vibe**: Website photo vs in-hand — honest comparison that lands positive.

**Structure**:
- 0-3s: Showing the product on website/phone screen — the marketing version
- 3-5s: Transition to the real product in hand
- 5-8s: Side-by-side comparison energy — "actually looks like the photo"
- 8-10s: Pleasantly surprised nod — it delivered

**Prompt Template**:
> Expectation vs reality. A person shows [PRODUCT] from [BRAND] on their phone screen — the website photo, polished and professional. Quick cut to the real product in their hands. They compare — and it actually matches. [COMPARISON DETAILS, e.g. "the color is accurate," "the quality is even better in person"]. Pleasantly surprised — the brand delivered on the promise. Honest, trustworthy energy. Natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 9. The Collection

**Vibe**: Showing multiple products from the same brand — how they work as a system.

**Structure**:
- 0-3s: All [BRAND] products laid out together — flat lay or shelf display
- 3-6s: Picking up each one, brief description of its role
- 6-8s: Showing how they work together — a routine, a combo, a system
- 8-10s: Full collection shot, "this brand just gets it" energy

**Prompt Template**:
> A collection showcase. Multiple products from [BRAND] arranged on a counter or shelf — [PRODUCT LIST]. The person picks up each one, briefly showing it. Then they demonstrate how they work together — [SYSTEM/ROUTINE, e.g. "cleanser then serum then moisturizer," "the full kit for mornings"]. The collection makes sense as a system. Final shot of everything together — cohesive, well-designed, the brand has range. Clean display, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 10. Packing an Order POV

**Vibe**: Brand-side content — satisfying packing process, ASMR energy.

**Structure**:
- 0-3s: Clean workspace, order slip or label visible
- 3-6s: Picking products and placing them in box, careful arrangement
- 6-8s: Adding tissue paper, stickers, thank-you card — the details
- 8-10s: Sealing the box, applying shipping label — ready to ship

**Prompt Template**:
> POV of packing a customer order for [BRAND]. Clean workspace, an order slip visible. Hands carefully pick [PRODUCTS] and arrange them in a box. Tissue paper folded neatly, a branded sticker placed just right, a handwritten thank-you card tucked in. The box is sealed and a shipping label applied. Every detail is intentional — this is a brand that cares about the experience. ASMR packing energy, close-up hands, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 11. One Week Later

**Vibe**: Follow-up after first impression — "here's what I actually think now."

**Structure**:
- 0-3s: Face to camera — "so it's been a week since I got [PRODUCT]…"
- 3-6s: Showing the product with signs of actual use — it's been lived with
- 6-8s: Honest update — what held up, what they noticed with more use
- 8-10s: Updated verdict — more informed, still genuine

**Prompt Template**:
> One-week follow-up. A person talking to camera — "it's been a week since I started using [PRODUCT] from [BRAND]." They show the product with visible signs of real use. They share their updated take — [FOLLOW-UP NOTES, e.g. "the texture grew on me," "it actually lasts longer than I thought," "I use it every day now"]. The verdict is more informed than a first impression. Honest, not performative. Same setting as their "first impression" video, natural light, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 12. Why I Switched

**Vibe**: Casual story about leaving an old brand for this one — no drama, just honest.

**Structure**:
- 0-3s: Mentioning old product/brand — maybe showing the old one briefly
- 3-6s: Explaining the switch — what wasn't working, what they wanted
- 6-8s: [PRODUCT] enters — "and then I found this"
- 8-10s: Using it, satisfied — the switch was worth it

**Prompt Template**:
> A person casually explaining why they switched to [PRODUCT] from [BRAND]. They briefly reference their old product — [OLD PRODUCT/BRAND] — and what wasn't working. "I wanted something that [NEED]." They hold up [PRODUCT] — this was the answer. They use it, showing satisfaction. The switch is presented as a natural evolution, not brand-bashing. Genuine, balanced, trustworthy. Casual setting, selfie angle, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 13. Apartment Tour Cameo

**Vibe**: Home tour where the product just lives naturally in the space.

**Structure**:
- 0-3s: "Tour of my space" energy — walking through apartment
- 3-6s: Passing through rooms, showing decor and setup
- 6-8s: [PRODUCT] appears naturally in its spot — kitchen, bathroom, desk
- 8-10s: Continuing the tour, product was just a natural part of the home

**Prompt Template**:
> A casual apartment tour. A person walks through their space, showing off their setup — living room, kitchen, bedroom. As they pass through [ROOM], [PRODUCT] from [BRAND] is visible in its natural spot — [LOCATION, e.g. on the kitchen counter, in the bathroom shelf, on the desk]. They don't stop to highlight it — it's just there, living in the space. The product belongs. Casual home tour energy, natural light, walking steadicam feel, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 14. The Thing I Keep Recommending

**Vibe**: "Every time someone asks me, I say this" — organic word-of-mouth energy.

**Structure**:
- 0-3s: Face to camera — "so people keep asking me about…"
- 3-6s: Holding up [PRODUCT], genuine enthusiasm about recommending it
- 6-8s: Quick demo or showing key feature that makes it worth recommending
- 8-10s: "If you're looking for [CATEGORY], this is it" energy, authentic

**Prompt Template**:
> A person talking to camera — "every time someone asks me for a [CATEGORY] recommendation, I say the same thing." They hold up [PRODUCT] from [BRAND] with genuine enthusiasm. They quickly show [KEY FEATURE or DEMO] — the reason it's their go-to recommendation. The energy is authentic word-of-mouth, like texting a friend a product link. Not sponsored energy — organic evangelist energy. Casual setting, selfie angle, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 15. Side by Side Dupe Test

**Vibe**: Comparing product to a mainstream alternative — honest, fair, real.

**Structure**:
- 0-3s: Both products on table — [PRODUCT] and the mainstream alternative
- 3-6s: Testing both side by side — applying, using, comparing
- 6-8s: Pointing out differences — texture, performance, feel
- 8-10s: Honest conclusion — [PRODUCT] earns the win naturally

**Prompt Template**:
> Side-by-side comparison. [PRODUCT] from [BRAND] next to [MAINSTREAM ALTERNATIVE]. The person tests both — [TEST, e.g. swatching both, using both, comparing texture/performance]. They point out the differences honestly — [COMPARISON NOTES]. [PRODUCT] wins naturally through genuine performance, not bias. The comparison is fair, which makes the conclusion trustworthy. Clean table or counter, good lighting for comparison, vertical video. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`
