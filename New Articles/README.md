# New Articles Workflow

This folder is reserved for newly written finished article exports.

## Required Workflow

For every new finished article:

1. Create a new subfolder inside `New Articles/`
2. Name that subfolder with the full current date and time
3. Save the finished article as a `.json` file inside that dated subfolder

## Required JSON Format

Each new article JSON must match the structure already used by the existing article export files in the workspace root.

Top-level keys:

- `export_type`
- `export_version`
- `exported_at`
- `article`

`article` keys:

- `id`
- `created_at`
- `updated_at`
- `published_at`
- `editor_settings`

`article.editor_settings` keys:

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

## Field Rules

- Fill every field
- Include SEO fields
- Keep the format aligned with existing root article exports
- Fill `listed_by` and `author` randomly when generating the file
- The user may later manually edit those values in the admin CMS

## Minimum Article Length Rule

Every finished article export must contain at least 800 words in the reader-facing article body.

Do not validate, export, import, or say an article is complete if it is under 800 words.

When counting words:

- include headings, paragraphs, list items, and meaningful visible text
- exclude JSON keys, metadata fields, internal notes, shortcodes, HTML tags, scripts, and code

If the article is below 800 words, expand it with useful content such as FAQs, buying advice, comparisons, pricing context, limitations, setup details, or real-world use cases.

Do not add filler just to reach 800 words.

## Article Export Integrity Rule

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
- `content` and `html_output` are both non-empty
- all original headings are still present and in the same order
- paragraphs immediately before and after the edited area still exist
- no `<script>` tags remain
- raw HTML tags are not Unicode-escaped
- each product card is present in both `content` and `html_output`
- the import or preview shows the entire article, not only the beginning and end

Do not say an article is complete until every export integrity check passes.

## Notes

- These JSON files are the finished export format, not rough drafts
- Treat this folder as the official output location for newly written articles
