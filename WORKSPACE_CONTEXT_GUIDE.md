# Workspace Context Guide

This file is a shared context guide for future AI models working in this workspace.

Its purpose is to preserve the user's preferences, the blog's editorial strategy, the product-card strategy, and the working conventions already established in earlier prompts.

## Project Purpose

This workspace supports a blog project centered around:

- product reviews
- product comparisons
- viral-style product news
- tech news
- buying guides
- resale/value analysis
- trend-driven commerce content

The articles are not meant to feel like hard-sell affiliate pages. They should read like useful editorial content first, while still supporting conversions when the product-card insert is genuinely relevant.

## Core Editorial Positioning

Articles should feel:

- helpful
- current
- natural
- persuasive without sounding pushy
- informed by real market behavior
- SEO-aware without sounding robotic

The goal is to make the reader feel:

- they learned something real
- they understand the product, trend, or market angle
- the inserted deal is unusually good
- the opportunity is worth taking seriously

Do not make the article sound like an ad. The recommendation should feel earned by the content.

## Thumbnail Prompt Response Rule

When the user asks for a thumbnail prompt, says `thumbnail`, says `prompt for thumbnail`, or asks for thumbnail prompts after an article, future models should respond with three different thumbnail prompt modes by default:

1. **Clicky Thumbnail**
   - bold YouTube-style buyer-decision thumbnail
   - strong emotion, high contrast, big readable hook text
   - product large and sharp
   - dramatic curiosity-gap composition

2. **Editor/Author Face + Reviewed Item**
   - use the writer/editor face with identity lock
   - show the reviewed item clearly
   - cleaner, premium, less noisy
   - little to no text

3. **Item-Only Stylish Thumbnail**
   - no author/editor face
   - focus only on the reviewed item or product
   - stylish commercial composition
   - dramatic but clean lighting
   - no noisy text unless a price cue is necessary

4. **Cutout Cascade / Printed Magazine Effect**
   - include this optional fourth mode when the user attaches an item screenshot/image or asks to recreate a cutout look
   - cut out the item/object and recreate it as multiple overlapping cutouts in a vertical or diagonal cascade
   - use soft feathered edges, subtle halo bloom, cool teal/cyan desaturated grading, lifted blacks, milky whites, blue-to-cream gradient background, and uniform halftone/newsprint grain
   - keep it stylish and editorial, with little to no text

5. **Hero Subject + Motion Echo Poster**
   - include this optional fifth mode when the attached image is a person, athlete, creator, model, or main subject
   - cut out one large sharp hero subject in the foreground and keep it fully saturated in natural color
   - add 2 smaller duplicate/echo versions of the same subject behind it, desaturated or duotone-tinted to one accent color
   - blend background echoes into a radial or diagonal gradient wash with darker corners and a brighter center spotlight
   - apply uniform fine grain or halftone print texture across the whole image
   - optional soft-blurred mood graphics can be used when they match the article tone

Do not only provide one thumbnail prompt unless the user explicitly asks for one.

For face-based thumbnail modes, use the established identity-lock language from `thumbnail preference.md`.

Identity lock applies only to the attached writer/editor image. Other attached images should be treated as product, result, tutorial, before/after, or style references.

## Product Card Strategy

Inside many articles, insert one, two, or three product cards when they are contextually relevant.

These product cards come from the database and are stored locally for context in the `products/` folder.

Each product card is identified by a slug and embedded with this exact format:

`[product-card:slug]`

Any relevant product card stored in the local `products/` folder may be used in articles.

There is no longer an `ABDO-only` restriction for product-card inserts.

Listings can be from `abdo`, but they can also come from other admin uploaders. A relevant listing should not be rejected just because its `listed_by` value is not `abdo`.

### Product Rotation Rule

Do not keep inserting the same product card across every new article when multiple relevant product cards exist for the same item or topic.

Future models should:

- rotate between relevant matching product cards
- shuffle product-card selection across new articles
- avoid repetitive reuse of the same default card
- still prioritize topical relevance over random rotation

The goal is variety with relevance.

If several valid product cards fit the article, do not always choose the same one by habit.

### Important Positioning Rules

The product cards that live in the DB are special:

- they are usually rare deals
- they are often private or unusually hard to find
- they should be treated as the source of truth for the listing details available in the local product data
- they may sell out quickly
- they should be checked first when they match the article topic
- if the embedded product is sold out, look for other relevant product-card deals because a better available listing may exist

Because of that, these are not normal affiliate products. They should be framed as:

- exclusive deals
- unusually strong value opportunities
- must-check or must-snipe opportunities when truly relevant
- rare listings that serious buyers should check before looking elsewhere

However, this must never be forced into the article unnaturally.

The article should lead the reader to that conclusion through context, price reality, demand, scarcity, comparison, or market behavior.

Do not write fixed discount claims such as "40% off," "40% below market," or similar percentage-off language unless that exact discount has been verified against current market pricing.

Without verification, use safer framing:

- rare deal
- strong listing
- worth checking first
- could sell out quickly
- compare it against current market prices before buying
- if it is sold out, check other related product cards for a better available deal

## How to Frame Deal Inserts

When inserting a DB-backed product card:

- make it feel like a natural buying option
- position it as a standout opportunity
- explain why it is notable
- connect it to the topic of the article
- support the insert with logic like resale value, market shortage, buyer demand, rarity, specs, condition, or price advantage
- treat the product card itself as the source of truth for the listing details
- avoid exact savings or percentage claims unless independently verified
- if a referenced product card is sold out, search for another relevant available product-card deal instead of pretending the sold-out listing is still available

Avoid:

- aggressive sales language
- obvious hype with no support
- unverified percentage-off claims
- repetitive CTA-heavy writing
- making every article sound like the same pitch

Preferred tone:

- calm confidence
- insider market awareness
- practical recommendation
- selective urgency

## Comparison Strategy

Sometimes an article may mention:

- the same item on Amazon at a much higher price
- the same item on eBay at current resale price
- retail or marketplace alternatives with worse value

This is useful context.

The logic is:

- show the broader market reality
- show what normal or inflated pricing looks like
- let the DB product card look obviously stronger by comparison

Important:

- do not oversell the contrast
- do not sound manipulative
- do not fake urgency
- let the pricing gap speak for itself

The reader should come away feeling that the DB-backed card is the smart move.

## Article Types

Future models should understand that this blog can publish several styles of content:

### 1. Product Reviews

Use when the article is centered on one item and answers whether it is worth buying, still relevant, overhyped, underrated, profitable to resell, or good for a certain use case.

### 2. Product Comparisons

Use when the article compares two or more products, generations, models, or buying paths.

### 3. Viral Product News

Use when an item is trending on TikTok, YouTube, Reddit, resale communities, or short-form social content.

### 4. Tech News

Use when discussing launches, hype cycles, upgrades, rumors, market reactions, or current buyer behavior.

### 5. Buyer Intent / SEO Articles

Use when the goal is to rank for a keyword with strong purchase, research, or comparison intent.

## SEO and Keyword Workflow

This workspace already uses product-specific keyword files.

When the user provides a keyword list:

- create a new `.md` file named after that product/topic
- preserve the keyword order exactly as given
- treat the order as ranked from highest search volume to lowest search volume
- use that file later when writing about the item

These keyword files are used as long-term SEO briefs.

When writing an article about a product:

- check whether a product keyword file already exists
- strongly consider those keywords while writing
- target them naturally in headings, phrasing, and search-intent alignment
- avoid obvious keyword stuffing

The goal is to rank on Google while keeping the article high quality and human-readable.

## Answer-First Summary Rule

Every article should add the important points of the article near the top in a compact, summarized, straight-to-the-point section.

This section should appear after the opening hook and before the deeper article body.

Use a heading like:

- `Quick Take`
- `Quick Verdict`
- `Key Points`
- `What You Need To Know`

The section should summarize the article's golden nuggets:

- the direct answer to the main search query
- the strongest verdict or recommendation
- the key buying/value warning
- the most useful comparison point
- the reader's best next step

Keep it short:

- 3 to 6 bullets maximum
- no fluff
- no generic filler
- no long paragraphs

Reason:

Google, readers, and AI-assisted discovery all benefit when the core answer is easy to extract at the top of the article. Do not bury the best information deep in the body.

## Product Context Workflow

The top-level `products/` folder exists for future context.

It contains:

- a raw product export snapshot
- one Markdown file per product
- the slug, product ID, and embed shortcode for each product

When asked to write about item `X`:

1. search the `products/` folder for matching products
2. identify the most relevant product card slug
3. if multiple relevant product cards exist, rotate or shuffle the choice instead of defaulting to the same card every time
4. use the product details to understand the exact offer
5. insert the product card naturally where it strengthens the article
6. if helpful, contrast it against Amazon, eBay, retail, or resale context

Do not insert unrelated product cards just to monetize the article.

## How Articles Should Sell Without Feeling Salesy

The article should do the persuasion indirectly by showing:

- why the item matters
- why people want it
- how the market currently prices it
- where hype is real or overblown
- why this specific embedded deal stands out

The article should feel like:

- editorial content with real judgment
- not an affiliate landing page

Best practice:

- teach first
- compare second
- recommend third

## Writing Style Preferences

The user's preferred article approach is:

- high quality
- search-aware
- market-aware
- persuasive but subtle
- useful for future monetization
- grounded in real-world value

Strong article qualities:

- clean hook
- strong search-intent match
- easy-to-scan subheads
- real buying insight
- believable market framing
- natural placement of product cards
- no spammy tone

## Reuse of the Same Item Across Platforms

The same item may appear in different forms inside an article:

- a DB product card with an unusually low deal price
- an Amazon listing at a much higher new price
- an eBay listing around resale price

This is acceptable and often strategically useful.

Use these multiple references to help the reader understand:

- normal price
- inflated marketplace price
- resale baseline
- why the DB-backed product card is exceptional

## Existing Workspace Conventions

The following conventions have already been established and should continue:

### Keyword Files

- keyword lists should be saved as `.md` files
- file names should match the product/topic
- keyword order should stay exactly as the user gave it

### AI Prompt Research Files

- whenever the user pastes phrases or statements labeled as AI prompts for item `X`, process them and save them as prompt-style research for that item
- treat those prompts as real discovery and answer-intent signals
- these prompts should be preserved because users around the world ask similar questions inside AI chats
- those AI chats increasingly use search engines and external sources
- the strategic goal is for this blog to become useful enough that AI systems may read it, cite it, recommend it, or mention it as a source in future answers

This means prompt-style research is not secondary. It is part of the search and discovery strategy.

Future models should understand there are now three important intent inputs for many items:

- ranked keywords from most searched to least searched
- Google-style question clusters such as who, what, when, where, why, and how
- AI prompt phrasing that mirrors how people ask modern AI systems for advice or explanations

When the user provides AI prompts for an item:

- save them in a structured `.md` file for that item
- keep the wording close to what the user supplied
- use them later to shape article framing, headings, summaries, and answer-first writing
- treat them as high-value signals for how content should sound when targeting AI-assisted discovery

## Discovery Strategy Beyond Google

This project is not only trying to rank in classic search.

It is also trying to become useful in AI-assisted discovery.

That means article writing should consider:

- classic SEO
- buyer intent
- question intent
- AI-answer intent

The content should be strong enough that:

- humans trust it
- search engines understand it
- AI systems can easily parse it
- AI systems may use it as a useful cited or recommended source

This is one reason the user may provide:

- standard keyword rankings
- Google question clusters
- AI prompt clusters

All three should be preserved and used together when planning articles for an item.

## Mandatory Local File Search Before Writing

This is a must.

Before writing about any item, always search the local workspace files first by item name.

Future models should use local file search to find existing `.md` files that already contain context for that item.

This includes files that may contain:

- ranked keywords
- long-tail keywords
- low-competition or low-term keywords
- Google question clusters
- AI prompt phrasing
- product context
- prior research
- item-specific notes

Operational rule:

- always grep or otherwise search local files by the item name first
- review the matching local context files before writing
- use those local files as core planning inputs for the article

The reason is simple:

- this workspace is building long-term memory through files
- future article quality depends on reusing that memory
- articles should be based on the stored local research, not only on fresh web research

For any item-based article, the ideal order is:

1. search local files by item name
2. read the relevant `.md` files
3. extract keywords, questions, prompts, and product references
4. then do external research and verification
5. then write the article using both local context and verified web understanding

This rule applies to both the current model and any future AI agent working in this workspace.

## Raw Web Paste Sanitization Rule

The user may paste data copied directly from the web in a fast, unsanitized form.

This is expected.

That pasted material may include:

- repetitive UI words
- navigation labels
- filter labels
- buttons
- view-count text
- duplicated headings
- formatting noise
- broken spacing
- irrelevant copied interface fragments

Future models must sanitize that material before treating it as usable research.

Sanitization rules:

- remove repetitive UI language
- remove obvious interface noise
- remove duplicated junk text
- preserve the useful research signal
- keep the meaningful keywords, prompts, questions, volumes, CPC values, and item-specific data
- reorganize the cleaned information into a readable `.md` structure when saving it

The goal is:

- clean research files
- usable context for future writing
- no messy raw web clutter inside the long-term workspace memory

In short:

- raw web paste is acceptable as input
- raw web paste is not acceptable as saved research without cleanup

### Product Files

- product data should be pulled from the DB using credentials found in the blog code source
- product context should be saved in the top-level `products/` folder
- each product should have its own `.md` file
- each file should preserve the slug and exact embed shortcode

### New Article Export Files

- newly written finished articles should be saved as `.json` files
- the JSON format should match the existing article export files already stored in the workspace root
- the expected top-level structure is:
  - `export_type`
  - `export_version`
  - `exported_at`
  - `article`
- the expected `article` structure is:
  - `id`
  - `created_at`
  - `updated_at`
  - `published_at`
  - `editor_settings`
- the expected `article.editor_settings` structure is:
  - `originalSlug`
  - `slug`
  - `title`
  - `content`
  - `html_output`
  - `author`
  - `category`
  - `category_label`
  - `image_url`
  - `read_time`
  - `published`
  - `article_type`
  - `generation_status`
  - `listed_by`
  - `meta_description`
  - `meta_keywords`
  - `focus_keyword`
  - `og_title`
  - `og_description`
  - `og_image`
  - `canonical_url`
  - `twitter_card`
  - `is_featured`
  - `programmatic_template`
  - `programmatic_key`
  - `programmatic_data`

### New Articles Folder Workflow

- all newly written finished article JSON files should be stored inside the top-level `New Articles/` folder
- inside `New Articles/`, create a separate folder for each finished article
- each article folder should be named with the full current date and time so progress can be traced over time
- place the final article `.json` file inside that dated folder
- each finished article export should have every field filled, including SEO fields
- for `listed_by` and `author` or editor-related values, fill them randomly during generation because the user will manually edit them later in the admin CMS

### Category Slug Rule

Article JSON imports accept only canonical category slugs.

The `category` field must be a slug, not a display name and not an old alias.

Accepted:

```json
{
  "category": "graphics-cards",
  "category_label": "Graphics Cards"
}
```

Rejected:

```json
{
  "category": "Graphics Cards"
}
```

Also rejected:

```json
{
  "category": "photography-tips"
}
```

Valid category slugs are:

- `smartphones`
- `laptops`
- `graphics-cards`
- `gaming`
- `cameras`
- `audio`
- `wearables`
- `tvs-displays`
- `home-appliances`
- `deals`
- `buying-guides`
- `price-comparison`
- `news`
- `automotive-tech`
- `style-gear`

Use `category_label` for the readable display label when available.

Before validating an article export, verify that `category` exactly matches one valid slug from this list.

Common mappings:

- Graphics Cards -> `graphics-cards`
- Gaming Consoles -> `gaming`
- Cameras or Photography Tips -> `cameras`
- Audio & Headphones -> `audio`
- Laptops & PCs -> `laptops`
- TVs & Displays -> `tvs-displays`
- Home Appliances -> `home-appliances`
- Buying Guide -> `buying-guides`
- Price Comparisons -> `price-comparison`
- Style & Gear -> `style-gear`
- Automotive -> `automotive-tech`

### Article Completion Standard

- a newly written article is not considered fully finished unless its export JSON is complete
- complete means:
  - article body is written
  - reader-facing article body has at least 800 words total
  - SEO fields are filled
  - slug fields are filled
  - metadata fields are filled
  - export wrapper fields are filled
  - the file is saved in the dated `New Articles/` subfolder

Do not validate, export, import, or say an article is complete if it is under 800 words.

When counting words, include headings, paragraphs, list items, and meaningful visible reader-facing text. Exclude JSON keys, metadata fields, internal notes, shortcodes, HTML tags, scripts, and code.

If an article is under 800 words, expand it with useful information such as FAQs, buying advice, comparisons, pricing context, product limitations, setup details, or real-world use cases. Do not add fluff just to hit the number.

### Article Export Integrity Rule

An article export is not complete just because its JSON is valid.

It must import into the blog with every paragraph, heading, social embed, and product card visible in the correct order.

When editing an existing article JSON:

- preserve both `content` and `html_output`
- never make a small string replacement near HTML tags unless the complete before-and-after HTML has been inspected
- keep article HTML as readable raw HTML
- do not serialize tags such as `<p>`, `<h2>`, `<blockquote>`, or `<product-embed>` into Unicode escapes like `\u003c` and `\u003e`
- never leave an unclosed HTML tag
- do not include TikTok, X, or Twitter provider `<script>` tags in article exports
- save only the supported social embed blockquote markup because the blog renderer handles provider scripts itself

An unclosed `<script>` tag can cause every following section of the article to disappear.

When adding a product card:

- in `content`, use the exact shortcode:
  `[product-card:slug]`
- in `html_output`, use:
  `<div><product-embed data-slug="slug"></product-embed></div>`

Before declaring an article finished, verify:

- the JSON parses successfully
- `category` is exactly one valid canonical category slug
- `content` and `html_output` are both non-empty
- all original headings are still present and in the same order
- paragraphs immediately before and after the edited area still exist
- no `<script>` tags remain
- raw HTML tags are not Unicode-escaped
- each product card is present in both `content` and `html_output`
- the import or preview shows the entire article, not only the beginning and end

Do not say an article is complete until every export integrity check passes.

### Article Insert Logic

- use one to three product cards where appropriate
- only insert cards that strengthen the article
- frame them as rare, valuable, and worth checking first
- do not claim exact percentage discounts unless verified
- if a deal is sold out, look for other relevant product-card deals that may still be available
- do not force them if the fit is weak

## What Future Models Should Remember

If you are a future AI model working in this workspace, remember:

- this is not just a blog, it is an editorial + conversion system
- the product cards in the DB are unusually strong deal assets
- product cards are the source of truth for listing details, but exact discount claims still need verification
- the writing should make readers trust the recommendation
- the recommendation should feel discovered, not pushed
- keyword files and product files are part of the long-term memory of this workspace
- when in doubt, choose natural persuasion over aggressive monetization

## Default Behavior for Future Article Requests

When the user asks for an article:

1. identify the target topic or product
2. check for an existing keyword `.md` file
3. check the `products/` folder for relevant product-card candidates
4. understand whether the article should be a review, comparison, viral news piece, tech news piece, or buyer guide
5. write the article in a high-quality editorial style
6. include a compact answer-first summary near the top with the article's key golden nuggets
7. insert one to three product cards only where they genuinely fit
8. make the value of the DB-backed offer obvious through reasoning, not force

This file should be treated as a standing guide for future work in this workspace.

## Mandatory Reading

Before writing any article, future AI models should also read:

- [Writing Style.md](/Users/elma777boubi/Downloads/articles/Writing%20Style.md)

That file contains the strict writing manifesto for high-conversion article output and should be treated as required instruction, not optional guidance.
