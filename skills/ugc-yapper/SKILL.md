---
name: ugc-yapper
description: >-
  UGC video format templates for Yapper-style ads. Contains 15 TikTok-native,
  lofi video formats with shot-by-shot structure and AI video generation prompts.
  Focused on authentic, single-take, talking-head videos with high personality and no production value. Use when the user wants to create UGC content that feels like a real person sharing their unfiltered thoughts.
requires:
  env:
    - RAWUGC_API_KEY
compatibility: >-
  Use alongside the rawugc-api skill for API endpoint knowledge.
  Requires RAWUGC_API_KEY.
homepage: https://github.com/tfcbot/rawugc-skills
source: https://github.com/tfcbot/rawugc-skills
---

# Yapper UGC Video Formats

15 lofi, TikTok-native video formats for Yapper-style ads. Raw, authentic, single-take, talking-head videos with high personality and no production value. These formats are designed to feel like a real person sharing their unfiltered thoughts and experiences.

## How to Use These Formats

1.  Identify the user's goal (e.g., product recommendation, brand story, relatable experience).
2.  Select the format below that best matches the desired vibe and context.
3.  Use the **Prompt Template** to compose the `prompt` field for `POST /videos/generate`. Replace `[BRACKETED]` placeholders with details from the user.
4.  Default to `aspectRatio: "portrait"` (9:16) and `nFrames: "10"` unless the format specifies otherwise.
5.  Emphasize a casual, unscripted, and authentic tone. The goal is to avoid anything that feels like a polished advertisement.

---

## Formats

### 1. The Car Rant

**Vibe**: Person ranting in their car, either driving or parked, with the engine running. Passionate, unfiltered, and direct.

**Structure**:
- 0-3s: Close-up on the person's face, looking directly at the camera (phone mounted on the dash).
- 3-6s: Animated hand gestures while talking, emphasizing a point.
- 6-8s: A moment of self-awareness or a sigh, as if they can't believe what they're saying.
- 8-10s: A final, definitive statement, looking directly into the camera with conviction.

**Prompt Template**:
> A person in their car, ranting to the camera. They are passionate and unfiltered, using animated hand gestures to emphasize their points. The camera is mounted on the dashboard, creating a close-up shot. The person is talking about [TOPIC] and how [PRODUCT] has changed their perspective. The lighting is natural, and the energy is high. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 2. The Mid-Meal Monologue

**Vibe**: Someone talking to the camera while eating, completely engrossed in their story. Casual, relatable, and slightly messy.

**Structure**:
- 0-3s: The person takes a bite of food and then starts talking, mid-chew.
- 3-6s: They use their fork or spoon to gesture while explaining something.
- 6-8s: A moment of realization or a pause to take another bite.
- 8-10s: They finish their thought with a satisfied look, as if the food and the conversation are equally enjoyable.

**Prompt Template**:
> A person eating a meal and talking to the camera. They are completely engrossed in their story about [TOPIC], using their utensils to gesture. They are eating [FOOD] and talking about how [PRODUCT] fits into their daily routine. The setting is a casual dining environment, like a kitchen or a cafe. The tone is relatable and authentic. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 3. The Cooking Confessional

**Vibe**: Someone cooking and talking to the camera, sharing a personal story or a secret. Intimate, messy, and genuine.

**Structure**:
- 0-3s: The person is in the middle of a cooking task, like chopping vegetables or stirring a pot.
- 3-6s: They look up at the camera and start sharing a story, as if they just remembered something.
- 6-8s: They get distracted by their cooking for a moment, then return to their story with renewed energy.
- 8-10s: They finish their story with a smile or a laugh, as if sharing a secret with a friend.

**Prompt Template**:
> A person cooking in their kitchen and talking to the camera. They are sharing a personal story about [TOPIC] while preparing [DISH]. They get distracted by their cooking but always return to the camera with a genuine expression. They are using [PRODUCT] as part of their cooking process. The lighting is warm and inviting. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 4. The Distracted Diatribe

**Vibe**: Someone trying to tell a story but getting constantly distracted by their surroundings. Chaotic, funny, and very real.

**Structure**:
- 0-3s: The person starts to tell a story but is immediately distracted by something off-camera.
- 3-6s: They try to get back on track but are distracted again, this time by something else.
- 6-8s: They laugh at their own inability to focus and apologize to the camera.
- 8-10s: They finally manage to get their point across, but in a rushed and chaotic way.

**Prompt Template**:
> A person trying to talk about [TOPIC] but getting constantly distracted by their surroundings. They are in a busy environment, like a park or a city street. They are trying to explain the benefits of [PRODUCT] but keep getting sidetracked. The tone is chaotic and funny, and the person is laughing at themselves. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 5. The Walking and Talking Head

**Vibe**: Someone walking down the street, holding their phone and talking to the camera. Energetic, fast-paced, and in-the-moment.

**Structure**:
- 0-3s: The person is walking and talking, with the background moving behind them.
- 3-6s: They pause for a moment to emphasize a point, then continue walking.
- 6-8s: They interact with something in their environment, like a street sign or a storefront.
- 8-10s: They end their thought with a call to action or a question for the viewer.

**Prompt Template**:
> A person walking down a busy street and talking to the camera. They are holding their phone and walking at a brisk pace. They are talking about [TOPIC] and how [PRODUCT] helps them stay productive on the go. The background is a blur of city life. The tone is energetic and engaging. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 6. The Bathroom Mirror Monologue

**Vibe**: Someone getting ready in the bathroom, talking to their reflection in the mirror. Introspective, personal, and raw.

**Structure**:
- 0-3s: The person is looking at their reflection, in the middle of their morning or evening routine.
- 3-6s: They start talking to themselves, sharing their thoughts and feelings about [TOPIC].
- 6-8s: They use a product, like a face wash or a moisturizer, while continuing to talk.
- 8-10s: They make eye contact with their reflection, as if having a moment of self-realization.

**Prompt Template**:
> A person in their bathroom, talking to their reflection in the mirror. They are going through their [ROUTINE] and sharing their thoughts on [TOPIC]. They are using [PRODUCT] and talking about its effect on their skin/hair/etc. The lighting is soft, and the tone is introspective and personal. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 7. The Late-Night Thoughts

**Vibe**: Someone in bed, talking to the camera in a hushed voice. Sleepy, intimate, and unfiltered.

**Structure**:
- 0-3s: The person is lying in bed, with only a small lamp on.
- 3-6s: They start talking in a quiet, sleepy voice about something that's on their mind.
- 6-8s: They yawn or rub their eyes, showing that they are tired but can't sleep.
- 8-10s: They end their thought with a whisper, as if sharing a secret with the viewer.

**Prompt Template**:
> A person in bed at night, talking to the camera in a hushed voice. They are sharing their late-night thoughts on [TOPIC] and how [PRODUCT] helps them relax and unwind. The room is dark, with only a single lamp providing light. The tone is sleepy and intimate. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 8. The "Just Got Out of the Shower" Rant

**Vibe**: Someone with a towel on their head, fresh out of the shower, ranting about something they just realized. Fresh, energetic, and spontaneous.

**Structure**:
- 0-3s: The person is in their bathroom, with a towel wrapped around their head.
- 3-6s: They start ranting about a sudden realization they had in the shower.
- 6-8s: They gesture wildly with their hands, still full of energy from their epiphany.
- 8-10s: They end their rant with a look of triumph, as if they've just solved a major problem.

**Prompt Template**:
> A person fresh out of the shower, with a towel on their head, ranting to the camera. They are full of energy and excitement about a sudden realization they had about [TOPIC]. They are talking about how [PRODUCT] played a role in their epiphany. The bathroom is steamy, and the lighting is bright. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 9. The "I'm So Over This" Complaint

**Vibe**: Someone complaining about a common frustration, with a tone of exasperation and humor. Relatable, funny, and a little bit dramatic.

**Structure**:
- 0-3s: The person starts with a heavy sigh and an eye-roll.
- 3-6s: They launch into a complaint about [FRUSTRATION], using dramatic hand gestures.
- 6-8s: They pause for a moment, as if to catch their breath, then continue their rant.
- 8-10s: They end with a rhetorical question, as if asking the viewer for validation.

**Prompt Template**:
> A person complaining to the camera about a common frustration. They are being dramatic and humorous, using exaggerated gestures and facial expressions. They are talking about how [PRODUCT] is the only thing that helps them deal with [FRUSTRATION]. The setting is a relatable environment, like a messy room or a crowded bus. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 10. The "I Can't Believe I'm Admitting This" Confession

**Vibe**: Someone confessing a guilty pleasure or an embarrassing story. Secretive, funny, and vulnerable.

**Structure**:
- 0-3s: The person looks around to make sure no one is listening, then leans in to the camera.
- 3-6s: They start confessing their secret in a hushed voice, with a mix of shame and amusement.
- 6-8s: They cover their face with their hands for a moment, as if they can't believe they are sharing this.
- 8-10s: They end with a nervous laugh, as if relieved to have gotten it off their chest.

**Prompt Template**:
> A person confessing a guilty pleasure to the camera. They are being secretive and funny, using hushed tones and nervous laughter. They are talking about how [PRODUCT] is their secret indulgence. The setting is a private space, like a bedroom or a closet. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 11. The "Hot Take" Debate

**Vibe**: Someone passionately arguing a controversial opinion. Bold, opinionated, and engaging.

**Structure**:
- 0-3s: The person starts with a bold, controversial statement.
- 3-6s: They defend their position with passionate arguments and evidence.
- 6-8s: They challenge the viewer to disagree with them, using a confident and assertive tone.
- 8-10s: They end with a final, powerful statement that leaves the viewer thinking.

**Prompt Template**:
> A person passionately arguing a controversial opinion about [TOPIC]. They are bold and opinionated, using strong language and confident gestures. They are arguing that [PRODUCT] is the best in its category, and they are challenging the viewer to prove them wrong. The setting is a simple, uncluttered background that keeps the focus on the person. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 12. The "I'm a Genius" Hack

**Vibe**: Someone sharing a clever hack or a life-changing tip. Proud, excited, and helpful.

**Structure**:
- 0-3s: The person starts with a look of smug satisfaction, as if they've discovered something amazing.
- 3-6s: They share their hack with excitement, demonstrating how it works.
- 6-8s: They show the amazing results of their hack, with a look of pride on their face.
- 8-10s: They end with a confident smile, as if to say, "You're welcome."

**Prompt Template**:
> A person sharing a clever hack for [TASK] using [PRODUCT]. They are excited and proud, demonstrating the hack with clear and simple steps. They show the amazing results of their hack, with a look of smug satisfaction. The setting is a clean and organized space that highlights the effectiveness of the hack. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 13. The "Unboxing Gone Wrong" Story

**Vibe**: Someone telling a funny story about a disastrous unboxing experience. Humorous, self-deprecating, and relatable.

**Structure**:
- 0-3s: The person starts with a look of disappointment or frustration.
- 3-6s: They tell the story of their unboxing disaster, with a mix of humor and self-pity.
- 6-8s: They show the broken or damaged product, with a look of disbelief on their face.
- 8-10s: They end with a funny or ironic comment about their bad luck.

**Prompt Template**:
> A person telling a funny story about a disastrous unboxing experience with a product that is NOT [PRODUCT]. They are being humorous and self-deprecating, with a look of disbelief on their face. They then show how easy and satisfying it is to unbox [PRODUCT]. The setting is a typical home environment, with packages and boxes around. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 14. The "I'm Obsessed" Rave Review

**Vibe**: Someone gushing about a product they are absolutely in love with. Enthusiastic, passionate, and convincing.

**Structure**:
- 0-3s: The person starts with a look of pure adoration on their face.
- 3-6s: They gush about all the things they love about the product, using superlatives and exclamation points.
- 6-8s: They hold the product up to the camera, as if it's a precious treasure.
- 8-10s: They end with a heartfelt recommendation, urging the viewer to try it for themselves.

**Prompt Template**:
> A person gushing about [PRODUCT] to the camera. They are enthusiastic and passionate, using superlatives and exclamation points. They are holding the product and talking about all the reasons they are obsessed with it. The setting is a bright and cheerful environment that reflects the person's positive mood. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`

---

### 15. The "A Day in the Life" Montage

**Vibe**: A quick montage of a person's day, with the product making a subtle appearance in each scene. Authentic, aspirational, and lifestyle-focused.

**Structure**:
- 0-3s: A quick shot of the person waking up, with the product on their nightstand.
- 3-6s: A shot of them at work or school, with the product on their desk.
- 6-8s: A shot of them at the gym or a cafe, with the product in their bag.
- 8-10s: A final shot of them relaxing at home, with the product in hand.

**Prompt Template**:
> A quick montage of a person's day, showing how [PRODUCT] is a natural part of their lifestyle. The product is subtly featured in each scene, from their morning routine to their evening relaxation. The tone is aspirational and authentic, and the focus is on the person's life, not the product itself. [ADDITIONAL DETAILS].

**Settings**: `aspectRatio: "portrait"`, `nFrames: "10"`
