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

The usual thumbnail generation workflow uses two attached references:

1. The product image.
2. The editor or writer face image.

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
identity lock, keep the same facial structure, same features, same face identity. Generate a bold YouTube-style thumbnail for this person for an article talking about “[ARTICLE TITLE VARIABLE]”. Use the attached product image clearly in the thumbnail. Keep the product recognizable. Use a dark high-contrast tech background, strong blue/red lighting, sharp cutout style, dramatic buyer-decision mood. Not much text in the thumbnail, only a short readable hook.
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

## Minimal Text Rule

When the prompt says "not much text", use only a short hook.

Do not put the full article title on the thumbnail.

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
