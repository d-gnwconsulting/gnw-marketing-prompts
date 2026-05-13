---
version: 1.0
tested_model: claude-sonnet-4-6
tested_date: 2026-05-13
category: aeo
---

# Featured Snippet Optimizer

**Category:** AEO — Answer Engine Optimization
**Model tested:** Claude Sonnet 4.6
**Last updated:** 2026-05-13

## What it does

Rewrites content to win Google featured snippets (position zero) — the boxed answer that appears above all search results. Covers the three snippet types Google surfaces: paragraph snippets (direct definitions), list snippets (steps or rankings), and table snippets (comparisons or data).

Featured snippet content is also heavily cited by AI search engines. Optimizing for one typically improves performance on both.

## Input needed

- Target keyword or query
- Current page content (or description of what the page covers)
- Snippet type goal: paragraph / list / table / let Claude decide

## Prompt

```
You are an AEO (Answer Engine Optimization) specialist. Rewrite the following content to win a Google featured snippet for the target query, and to be cited by AI search engines.

Target query: [the exact search query you want to rank for]
Current content: [paste your content or describe the page]
Snippet type: [paragraph / list / table / decide based on query]

Google featured snippets follow these patterns:

**Paragraph snippet** (40–60 words): A direct, self-contained answer to a definition or explanation question. Starts with the query subject, not "I" or "We."

**List snippet** (5–8 items): Numbered steps or bulleted items. Each item is concise (under 10 words). Works for "how to" and "best X" queries.

**Table snippet** (3–5 rows, 2–3 columns): Comparison data. Header row with clear column labels. Works for "X vs Y" and "types of X" queries.

Deliver:
1. The recommended snippet type for this query and why
2. The optimized snippet-ready block (formatted exactly as Google would display it)
3. The 2–3 sentences that should appear directly after the snippet in the page body (context that reinforces the answer)
4. The H2 heading for this section
```

## Example

**Input:**
- Target query: `what is a featured snippet`
- Current content: Blog post about SEO basics, with a paragraph that loosely defines featured snippets in the middle of the post
- Snippet type: Let Claude decide

**Output:**

**Recommended type:** Paragraph snippet — "what is" queries almost always surface paragraph snippets, not lists.

**Optimized snippet block:**
> A featured snippet is a boxed answer that Google displays above all organic search results in response to a question or query. It pulls a direct, concise answer (typically 40–60 words) from a web page and shows it with the page title and URL. Featured snippets appear for approximately 12% of all search queries.

**Follow-up sentences for page body:**
> Google selects featured snippets algorithmically — there is no way to manually request one. The most reliable way to earn a featured snippet is to write a direct, well-structured answer to the target query near the top of a relevant page section.

**H2 heading:** `What Is a Featured Snippet in Google Search?`
