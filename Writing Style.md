# Writing Style

This file is a mandatory writing guide for every future AI agent working in this workspace.

Read this file before writing any article.

These rules are strict and should override generic article-writing habits.

## HIGH-CONVERSION ARTICLE WRITING MANIFESTO

You are not here to “write articles.”
You are here to produce content that maximizes:

- click-through rate
- time on page
- perceived usefulness
- reader trust

Every output must follow the rules below.

## 1. Core Principle

Reduce thinking effort. Increase clarity and curiosity.

If the content feels slow, generic, or effortful to read, it fails.

## 2. Language Style

Non-negotiable rules:

- use natural, conversational language
- prefer simple words over complex ones
- avoid academic, corporate, or robotic tone
- write like a smart human explaining something quickly

Rule:

If it would not be said out loud in a conversation, do not write it.

## 3. Forbidden Generic Phrases

Never use:

- “In today’s fast-paced world”
- “It is important to note that”
- “This article will explore”
- any filler introduction

Start directly with value.

## 4. Opening Structure

First 3 lines must follow this pattern:

- hook
- relatability
- clear promise

No long introductions.
No background stories.

## 5. Structure For Readability

- short paragraphs, one to three lines maximum
- frequent subheadings
- use bullet points when useful
- highlight key insights naturally

Write for scanners, not readers.

## 6. Anti-AI / Anti-Generic Rules

Your content must include:

- specific details
- numbers when relevant
- timeframes when relevant
- observations
- real-world friction
- limitations
- downsides
- trade-offs
- micro-details when possible

Example:

- bad: “Battery life is good”
- good: “Lasted about 6 hours, drops fast after 20%”

## 7. Opinions Are Required

Do not stay neutral.

You must:

- take positions
- make judgments
- eliminate options

Examples:

- “This is overpriced”
- “Only worth it if you need X”
- “Most people should avoid this”

Neutrality equals low value.

## 8. Decision-Driven Writing

Every section must help the reader decide something.

Avoid:

- listing specs without interpretation

Always answer:

What should the reader do?

## 9. Use Of “I” And “You”

- use “I” only to show experience or testing
- use “you” to guide and engage the reader
- avoid both in purely factual or news contexts

## 10. Contrast Creation

Actively create contrast:

- expectation vs reality
- pros vs cons
- good vs bad use cases

Example:

“Looks premium, feels cheap in hand”

## 11. Sentence Rhythm

- mix short and medium sentences
- occasionally break flow naturally
- avoid overly perfect or repetitive structure

The writing should feel human, not generated.

## 12. Complexity Control

- 90% simple language
- 10% precise or technical terms only when necessary
- always prioritize clarity over sounding intelligent

## 13. Article-Specific Rules

### Reviews

- give verdict early
- include pros and cons quickly
- speak from usage, not specs

### Comparisons

- clearly state which option wins and why
- use “If you want X, choose A” logic
- remove indecision

### News

- first sentence equals key information
- focus on what changed and why it matters
- no personal opinions

## 14. What To Avoid

Strictly avoid:

- long paragraphs
- over-explaining basic concepts
- rewriting manufacturer descriptions
- empty statements without insight
- trying to sound smart

## 15. Final Output Check

Before finishing, verify:

- is this easy to scan in seconds?
- did I include at least one strong opinion?
- did I provide real, specific insight?
- does it help the reader make a decision?
- does it sound like a real person?

If any answer is no, rewrite.

## Final Rule

The goal is not to impress.
The goal is to be understood instantly and trusted immediately.

- clear beats clever
- specific beats broad
- opinionated beats neutral
- human beats perfect

## 16. Grammar And Punctuation Rule

Strict rules:

- small, natural grammar imperfections are acceptable if they help the writing feel human
- it is not acceptable to use em dashes
- it is not acceptable to use multiple dashes as filler
- it is not acceptable to use dash-based filler structures

Reason:

These are strong signals of generic or AI-generated content.

## 17. No Filler Policy

- never add text just to sound complete
- no fluff
- no padding
- no empty transitions

Avoid:

- repeating the same idea in different words
- adding sentences that do not provide new value
- explanatory filler with no real insight

## 18. Internal Process Language Must Never Reach the Reader

This is a brutal rule.

Anything meant for the creation process must stay in the creation process.

Never expose internal workflow language inside reader-facing article copy.

Strictly forbidden in final article text:

- database language
- CMS language
- workspace language
- slug language
- shortcode language
- internal template language
- any phrase that sounds like article production machinery

Examples of bad wording:

- “DB-backed card”
- “workspace”
- “slug”
- “shortcode”
- “in the CMS”
- “this product card in the database”

The final reader should never feel the content was assembled from an internal system.

Reader-facing content must sound:

- editorial
- natural
- intentional
- fully human

If a sentence sounds like it belongs to the creation pipeline instead of the published article, remove or rewrite it.

## 19. Mandatory Research Before Writing

For any article about product X, research is required before writing.

This is a strict rule.

Before writing, you must:

- do a web search about product X
- understand the product from multiple angles
- verify important claims before using them
- study what people are saying in reviews and discussion spaces
- check Reddit when useful
- check other information-rich websites when useful
- understand praise, complaints, limitations, and buyer sentiment
- understand pricing, resale behavior, market perception, and common comparisons when relevant

Do not write blindly.

Do not write from vague memory.

Do not write unverified claims as if they are facts.

The article should be based on:

- verified information
- market understanding
- product understanding
- real user sentiment when available

If information is unclear, incomplete, or unstable, research more before writing.

Writing without verification is strongly prohibited.

## 20. Use Provided SEO Research Heavily And Smartly

When the user asks for a set of articles about a product and provides mass SEO research data, treat that data as core planning material.

The SEO research is not decoration.

It should shape:

- article angles
- headings
- answer sections
- comparison points
- buying advice
- FAQ-style explanations
- exact questions readers are searching
- normal search queries people type into Google
- related searches and long-tail keywords

Use the provided keyword and query data heavily, but do it naturally.

Do not dump keywords randomly.

Do not repeat the same phrase until it feels like spam.

Do not make the article sound like keyword stuffing.

Instead, turn search data into useful reader answers.

If the SEO data includes questions, the article should answer those questions clearly inside the body.

If the SEO data includes normal buyer queries, the article should cover those topics in natural sections.

If the SEO data shows repeated concerns, those concerns should become real editorial points, not hidden keywords.

The goal is to help the article get indexed by matching real search intent while still sounding like a human wrote it for a reader.

## Final Enforcement

Keep it:

- short
- direct
- useful

Every sentence must earn its place.

If a sentence does not add value, remove it.

## 21. Default Listed By Value

For this workspace setup, always use:

- `listed_by`: `Mehdi`

This should be treated as the default value for newly generated article export files unless the user explicitly asks for a different value.

## 22. Product Card Insert Filter

For this project, when inserting a new product card inside an article, you may use any relevant product card that exists in the local `products/` library.

This replaces the old `ABDO-only` restriction.

Use the best topical match available from the local product reference files or the latest product pull.

Do not force an unrelated product card into an article just because it exists.

## 23. Product Card Rotation Rule

When multiple relevant product cards exist for the same article topic, do not keep reusing the same product card by default.

You must:

- rotate between relevant matching product cards
- shuffle product-card selection across new articles
- avoid falling into the habit of inserting the same card repeatedly

Relevance still comes first.

Do not rotate randomly into a worse match just for variety.
