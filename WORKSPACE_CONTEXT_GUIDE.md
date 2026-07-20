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
- they are typically around 40% below market price
- they are often even below the normal resale price

Because of that, these are not normal affiliate products. They should be framed as:

- exclusive deals
- unusually strong value opportunities
- must-grab offers when truly relevant
- deals that serious buyers should not ignore

However, this must never be forced into the article unnaturally.

The article should lead the reader to that conclusion through context, price reality, demand, scarcity, comparison, or market behavior.

## How to Frame Deal Inserts

When inserting a DB-backed product card:

- make it feel like a natural buying option
- position it as a standout opportunity
- explain why it is notable
- connect it to the topic of the article
- support the insert with logic like resale value, market shortage, buyer demand, rarity, specs, condition, or price advantage

Avoid:

- aggressive sales language
- obvious hype with no support
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

### Article Completion Standard

- a newly written article is not considered fully finished unless its export JSON is complete
- complete means:
  - article body is written
  - SEO fields are filled
  - slug fields are filled
  - metadata fields are filled
  - export wrapper fields are filled
  - the file is saved in the dated `New Articles/` subfolder

### Article Insert Logic

- use one to three product cards where appropriate
- only insert cards that strengthen the article
- frame them as rare, valuable, and worth attention
- do not force them if the fit is weak

## What Future Models Should Remember

If you are a future AI model working in this workspace, remember:

- this is not just a blog, it is an editorial + conversion system
- the product cards in the DB are unusually strong deal assets
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
6. insert one to three product cards only where they genuinely fit
7. make the value of the DB-backed offer obvious through reasoning, not force

This file should be treated as a standing guide for future work in this workspace.

## Mandatory Reading

Before writing any article, future AI models should also read:

- [Writing Style.md](/Users/elma777boubi/Downloads/articles/Writing%20Style.md)

That file contains the strict writing manifesto for high-conversion article output and should be treated as required instruction, not optional guidance.
