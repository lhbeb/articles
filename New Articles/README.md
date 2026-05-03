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

## Notes

- These JSON files are the finished export format, not rough drafts
- Treat this folder as the official output location for newly written articles
