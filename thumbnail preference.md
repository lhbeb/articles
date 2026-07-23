# Thumbnail Preference

Use this guide when creating thumbnails for the article exports in this workspace.

## Overall Style

The preferred thumbnail style is bold, high-contrast, YouTube-style, and curiosity-driven.

The thumbnail should look like a serious buyer-decision video, not a clean blog hero image.

It should feel:

- urgent
- clickable
- product-focused
- comparison-driven
- slightly dramatic
- easy to understand in one second

## Format

- Use a 16:9 landscape layout.
- Design for readability at small sizes.
- Keep the image dense but not messy.
- Every thumbnail should have one clear question or buying decision.

Good framing examples:

- "2026: WORTH IT?"
- "WHICH SHOULD YOU BUY?"
- "WHICH PS5 SHOULD YOU ACTUALLY BUY?"
- "iPhone vs Canon G7X"
- "TRUTH OR LIE?"

## Main Composition

Use a three-part layout when possible:

1. Large human face on one side.
2. Product image or product box on the other side.
3. Big bold text filling the remaining space.

The face should not be tiny. It should take up a large part of the frame and show a clear emotion:

- confused
- thinking
- surprised
- serious
- curious
- pointing at the product

The product should be clearly visible and recognizable.

## Human Subject

The human subject is important.

Preferred poses:

- pointing at the product
- holding the product
- looking confused at the product
- looking off-frame as if deciding
- hand on chin in a thinking pose

Preferred expression:

- curious
- skeptical
- slightly shocked
- focused
- buyer-decision face

Avoid:

- casual smiling portrait with no emotion
- tiny face in the corner
- lifestyle-only photos
- faceless product-only thumbnails unless the product itself is very strong

## Text Style

Text must be huge, bold, and readable.

Use all caps for the main hook.

Preferred font style:

- bold condensed sans-serif
- thick block letters
- heavy YouTube thumbnail type
- white text with shadow or stroke
- yellow text for key numbers or urgency
- red text for warning or choice tension
- blue/cyan glow for tech products

Text should be short.

Best text length:

- 2 to 6 words for the main phrase
- 1 large number or year if relevant
- 1 question phrase

Good text patterns:

- "2026:"
- "WORTH IT?"
- "WHICH SHOULD YOU BUY?"
- "ACTUALLY BUY?"
- "TRUTH OR LIE?"
- "BETTER THAN iPHONE?"
- "$80 G7X?"

Avoid long article titles in the thumbnail.

## Color Palette

Use strong contrast.

Preferred colors:

- deep blue background
- black background
- red vs blue split background
- bright yellow text
- white text
- red warning blocks
- cyan glow

The colors should feel energetic and commercial.

Avoid:

- soft beige
- muted editorial colors
- pastel-only palettes
- low-contrast gray text
- clean minimalist blog style

## Background

Backgrounds should be dark, dramatic, and slightly tech-like.

Good options:

- blue glow
- red and blue split lighting
- blurred gaming or tech setup
- dark desk background
- subtle product-related environment

The background should support the subject and text, not compete with them.

Avoid:

- plain white background
- flat product catalog background
- busy room details
- realistic lifestyle background with weak contrast

## Product Treatment

Products should be large, sharp, and cut out cleanly.

Use glow, rim light, or shadow to separate the product from the background.

For article topics:

- Canon G7X articles should show the camera large and clear.
- iPhone vs Canon articles should show both devices or a split comparison.
- Price/deal articles should include a price cue or question mark.
- "Worth it" articles should show the product and a skeptical face.
- Comparison articles should show both options side by side.

Avoid tiny product images.

## Price Tag Rule

If the article is about pricing, price comparison, discount, refurbished price, resale price, MSRP, Amazon price, or best current price, the thumbnail should include a visible price tag or price cue.

Good examples:

- `$679?`
- `$849 MSRP`
- `$1,299?`
- `LOWEST PRICE?`
- `TOO HIGH?`

Keep the price cue short and readable.

For articles that are not mainly about price, do not spam price tags.

Only use a price tag on non-pricing articles if the price is a major reason someone would click.

## Layout Rules

Keep one dominant focal point.

Best layouts:

- face right, text left, product behind or bottom left
- face left, product center, text right
- product boxes bottom, face side, question mark center
- split red/blue comparison with product A vs product B

Use visual hierarchy:

1. Big year, price, or decision word.
2. Product.
3. Face.
4. Supporting text.

Do not let text cover the face too much.

Do not let the product hide behind the text.

## Click Psychology

The thumbnail should create a decision gap.

The viewer should instantly think:

- "Which one should I buy?"
- "Is this still worth it?"
- "Is this deal real?"
- "Am I about to overpay?"
- "Is the cheaper one better?"

Use uncertainty and comparison, but keep it honest.

Good hooks:

- "WORTH IT?"
- "WHICH ONE?"
- "BUY OR SKIP?"
- "TRUTH?"
- "OVERHYPED?"
- "STILL GOOD?"

## Canon G7X Thumbnail Direction

For Canon G7X articles, thumbnails should usually include:

- Canon G7X camera cutout
- iPhone if the article is a comparison
- big text like "G7X VS iPHONE" or "STILL WORTH IT?"
- shocked or thinking face
- blue or red/blue dramatic background
- yellow price or year if relevant

Good Canon G7X examples:

- "G7X IN 2026?"
- "$80 G7X?"
- "G7X VS iPHONE"
- "MARK II WORTH IT?"
- "TRUTH OR LIE?"

## Attached Image Workflow

The usual thumbnail generation workflow may use multiple attached references.

Sometimes the user may attach more than three images plus the writer/editor image.

The writer/editor image is the identity reference.

Identity lock applies only to the writer/editor image.

Other attached images may be:

- product images
- example results from a tutorial
- before/after examples
- screenshots from a video
- reference photos showing the desired look
- visual proof for how-to articles

Use those extra images as subject, product, style, or result references.

Do not apply identity lock to those extra images unless the user explicitly says one of them is also the writer/editor identity image.

When multiple attached images are provided, the thumbnail prompt should clearly say which image is for face identity and which images are for product/result/reference visuals.

When generating thumbnails from attached images, preserve the identity of the person.

Use identity lock language:

```text
identity lock, keep the same facial structure, same features, same face identity
```

The generated person should still look like the attached editor/writer.

Keep:

- same facial structure
- same recognizable features
- same face shape
- same general age
- same skin tone
- same hair style when possible
- same beard or glasses if present

Do not:

- turn the person into a different model
- over-beautify the face
- change ethnicity
- change age strongly
- remove important features like glasses, beard, or hairline
- make the face look AI-perfect or plastic

The product image should also be used directly as a reference.

Keep the product recognizable and close to the attached product photo.

## Standard Thumbnail Prompt Pattern

Use this kind of prompt when generating thumbnails:

```text
identity lock, keep the same facial structure, same features, same face identity. Generate a bold YouTube-style thumbnail for this person for an article talking about “[ARTICLE TITLE VARIABLE]”. Use the attached product image clearly in the thumbnail. Keep the product recognizable. Use graphics that match the article subject, or use a relevant blurred background if no specific graphic is needed. Use a dark high-contrast tech background, strong blue/red lighting, sharp cutout style, dramatic buyer-decision mood. Not much text in the thumbnail, only a short readable hook.
```

`[ARTICLE TITLE VARIABLE]` should be replaced with the actual article title each time.

Example article title variable:

```text
iPhone Camera vs Canon G7X Mark II: Which One Looks Better?
```

Example filled prompt:

```text
identity lock, keep the same facial structure, same features, same face identity. Generate a thumbnail for this person for an article talking about “iPhone Camera vs Canon G7X Mark II: Which One Looks Better?” Also use the attached product image clearly. Not much text in the thumbnail.
```

## Default Response Rule For Thumbnail Prompt Requests

When the user asks for a thumbnail prompt, says `thumbnail`, says `prompt for thumbnail`, or asks for thumbnail prompts after an article, respond with three different thumbnail prompt modes by default.

Do not only provide one prompt unless the user explicitly asks for one.

The three default modes are:

1. **Clicky Thumbnail**
   - bold YouTube-style buyer-decision thumbnail
   - strong emotion
   - product large and sharp
   - big readable hook text
   - high contrast, dramatic lighting, curiosity gap

2. **Editor/Author Face + Reviewed Item**
   - use the writer/editor face with identity lock
   - show the reviewed item clearly
   - clean, premium, less noisy
   - little to no text
   - good for articles where trust and human review matter more than loud clickbait

3. **Item-Only Stylish Thumbnail**
   - no author/editor face
   - focus only on the item, product, device, camera, console, bag, GPU, or reviewed object
   - stylish commercial composition
   - dramatic but clean lighting
   - no noisy text unless a price cue is necessary
   - useful when the product itself is strong enough to carry the image

Optional fourth mode when the user attaches an item screenshot/image or asks to recreate a cutout look:

4. **Cutout Cascade / Printed Magazine Effect**
   - cut out the attached item or subject from the screenshot/image
   - recreate the object as multiple isolated cutouts
   - arrange the cutouts in a vertical or diagonal cascade
   - use different scales, with the biggest cutout in the foreground and smaller cutouts receding behind it
   - use soft feathered edges, subtle white/light halo bloom, and no hard vector-mask look
   - use a cool teal/cyan desaturated grade, lifted blacks, milky whites, and muted pastel color
   - place everything on a simple blue-to-cream gradient background
   - apply uniform fine halftone/newsprint grain across the whole image
   - add subtle global bloom to unify mismatched source lighting

Use this fourth mode when the user specifically wants the final image-generation model to cut out an attached item, screenshot, product, person, or object and recreate a stylized editorial composite effect.

Optional fifth mode when the attached image is a person, athlete, model, creator, or subject where the thumbnail should feel like a sports/editorial poster:

5. **Hero Subject + Motion Echo Poster**
   - cut out one large hero subject in the foreground
   - keep the hero subject sharp, fully saturated, and in natural color
   - duplicate or echo the same subject in 2 smaller background poses
   - use the same person when possible, with different moments, poses, kits, or angles
   - desaturate, monochrome-tint, or duotone-tint the background echoes
   - blend background echoes softly into a radial or diagonal gradient wash
   - use darker corners and a brighter center spotlight behind the hero subject
   - add soft rim-light glow around the hero cutout
   - apply uniform fine grain or halftone texture across the entire image
   - optionally add soft-blurred mood graphics, such as hearts, sparks, light streaks, or accent icons, only when they match the article tone

Use this fifth mode when the user wants the item/person image to become a stylish editorial poster with a large foreground hero and repeated background echoes.

Every thumbnail prompt response should label these three modes clearly.

If the fourth or fifth mode is relevant, label all relevant modes clearly.

If an author/editor image is attached, apply identity lock only to that image.

If other images are attached, treat them as product, result, tutorial, before/after, or style references. Do not apply identity lock to product/result/reference images.

When writing the face-based modes, include this identity-lock sentence:

```text
identity lock, keep the same facial structure, same features, same face identity, same general age, same skin tone, same hairstyle, and any important features like glasses, beard, or hairline.
```

For pricing articles, include a short price cue or price tag in the clicky mode and item-only mode.

For non-pricing articles, do not force price tags.

## Cutout Cascade / Printed Magazine Effect Prompt Style

Use this prompt style when the user attaches an item screenshot or image and wants the next AI image-generation model to cut out that object and recreate a stylized editorial effect.

Technical style:

- multiple cutout subjects or objects isolated from source images
- vertical or diagonal cascade layout
- overlapping layers from back to front
- largest subject in the foreground, usually bottom-right
- smallest/furthest subject in the background, usually top-left
- off-center asymmetric arrangement
- heads/shoulders crop only for people, no full bodies unless the object requires full-body context
- soft slightly imprecise cutout edges
- subtle feathered white/light halo bloom around cutout edges
- no hard drop shadows
- soft luminous separation between overlapping layers
- edges slightly fade into each other at contact points
- desaturated cool-toned palette pushed toward teal/cyan and muted pastels
- skin tones, if any, shifted slightly cool/pink instead of warm orange
- individual source colors preserved lightly but unified under the same muted low-contrast grade
- lifted blacks, charcoal/navy shadows, milky whites
- simple horizontal gradient background, light blue at top into soft off-white/cream bottom
- subtle darker blue horizon band
- flat background with no scenery detail
- uniform fine halftone, dot-screen, or newsprint texture across both subjects and background
- subtle global glow/bloom pass across the whole final composite
- slight brightness push toward the top of the frame

Reusable prompt:

```text
Use the attached item screenshot/image as the source object. Cut out the object with a soft feathered edge and subtle light halo bloom. Recreate it as multiple overlapping cutout copies arranged in an asymmetric vertical/diagonal cascade, smallest in the top-left background and largest in the bottom-right foreground. Use varied scale and partial overlap, with soft luminous separation instead of hard shadows. Desaturate and grade the whole image cool teal/cyan with muted pastel tones, lifted charcoal blacks, and milky whites. Place the cascade on a flat light-blue-to-cream gradient background with a subtle darker blue horizon band. Apply a uniform fine halftone/newsprint grain texture across the entire composite, including object and background. Add a subtle global bloom pass to unify lighting. No noisy text, no hard vector-mask edges, no realistic scenery, no harsh drop shadows.
```

## Hero Subject + Motion Echo Poster Prompt Style

Use this prompt style when the user attaches a person, athlete, model, creator, or main subject image and wants a sport-style editorial poster effect.

Technical style:

- one large hero cutout centered or foreground
- hero subject sharply in focus
- hero subject kept in full natural color and saturation
- two or more smaller duplicate/echo images of the same subject in the background
- background echoes can use different poses, moments, kits, expressions, or angles when available
- background echoes should flank the hero subject symmetrically or asymmetrically
- background echoes are desaturated, monochrome, heavily tinted, or duotone-tinted to match one accent color
- background echoes have softer edges and lower opacity than the hero subject
- background echoes blend into the color wash
- hero subject has a clean sharp cutout with subtle rim light or edge glow
- radial or diagonal gradient background, darker at corners and brighter behind the hero subject
- no literal scenery or location detail
- strong foreground/background scale contrast
- slight vignette around the frame edges
- uniform fine grain, film grain, halftone dots, or print-poster texture across the whole composite
- optional soft-blurred graphic overlays for mood, such as hearts, sparks, streaks, or accent icons

Reusable prompt:

```text
Use the attached subject image as the main reference. Cut out the main subject with a sharp clean edge and subtle rim-light glow, keep the hero subject fully saturated, natural color, and sharply in focus. Create 2 smaller duplicate or echo versions of the same subject in the background, using different poses or moments if available. Desaturate or duotone-tint the background echoes to match one accent color, lower their opacity, and blend their soft edges into a radial or diagonal gradient backdrop. Make the background darker at the corners and brighter behind the hero subject, like a center spotlight. Scale the hero subject much larger than the background echoes so it feels like the subject is bursting forward. Apply uniform fine grain or halftone print texture across the whole image. Optional: add soft-blurred mood graphics or accent icons only if they fit the article tone. No scenery, no hard shadows, no flat sticker look, no noisy text.
```

## Minimal Text Rule

When the prompt says "not much text", use only a short hook.

Do not put the full article title on the thumbnail.

It is not necessary for a thumbnail to contain title text. Less text is usually better.

The thumbnail's job is to catch attention before the reader sees the title. Use the face, product, price cue, comparison cue, question mark, warning color, or relevant scene to create curiosity.

Graphics must be related to the article subject. If there is no useful related graphic, use a clean blurred tech or shopping background instead.

Do not add unrelated objects, icons, logos, decorations, or random graphics just to fill space.

For example, if the article title variable is:

```text
iPhone Camera vs Canon G7X Mark II: Which One Looks Better?
```

Good thumbnail text:

- `iPHONE VS G7X`
- `WHICH LOOKS BETTER?`
- `G7X OR iPHONE?`
- `BETTER PHOTOS?`

Avoid:

- `iPhone Camera vs Canon G7X Mark II: Which One Looks Better?`
- long subtitles
- more than 2 text blocks
- tiny explanatory text

For most thumbnails, use 1 to 4 words plus maybe a question mark.

## Things To Avoid

Avoid:

- blog-style hero images
- tiny text
- thin fonts
- calm editorial layouts
- too many words
- product-only flat images
- low emotion faces
- generic stock-photo look
- thumbnails that look like ads from a retailer

The thumbnail should look like a high-performing buyer-decision YouTube thumbnail.

## Final Checklist

Before using a thumbnail, check:

- Can the text be read on mobile?
- Is the product obvious?
- Is there a human expression or clear emotion?
- Does it ask or imply a buying decision?
- Is there strong contrast?
- Does it create curiosity in under one second?
- Would someone click it before reading the article title?

If the answer is no, redesign it.
