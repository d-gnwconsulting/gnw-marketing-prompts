# GEO Page Audit

**Category:** GEO
**Model tested:** Claude Sonnet 4.6
**Last updated:** 2026-05-13

## What it does

Evaluates a page's content and gives it a GEO readiness score with specific, actionable recommendations. Identifies the biggest gaps that prevent AI search engines from citing the page.

## Input needed

- Full page text (copy/paste the content)

## Prompt

```
You are a GEO (Generative Engine Optimization) auditor. Analyze the following page content and evaluate how likely it is to be cited by AI-powered search engines like Perplexity, ChatGPT, and Gemini.

Score the page from 0 to 100 across these 5 dimensions:

1. **Answer-first structure** (0-20): Does the content answer questions directly and quickly, without burying the answer?
2. **Entity clarity** (0-20): Are the brand, people, products, and topics clearly identified and described?
3. **Query alignment** (0-20): Does the content match the language and phrasing of real user queries?
4. **Citability** (0-20): Are there clear, quotable statements that an AI could extract and reference?
5. **Structured formatting** (0-20): Does the page use headers, lists, and clear sections that AI can parse?

For each dimension, give the score and 1-2 specific recommendations to improve it.

End with a total score and a prioritized list of the top 3 changes that would have the most GEO impact.

Page content to audit:
[paste your page content here]
```

## Example output structure

```
**GEO Audit Results**

1. Answer-first structure: 12/20
   - The main value proposition appears in paragraph 3. Move it to the first sentence.
   - Add a TL;DR or summary at the top of long sections.

2. Entity clarity: 8/20
   - The brand name appears only once. Repeat it in context throughout.
   - Add descriptive context: instead of "our platform", say "GNW's marketing analytics platform".

[...]

**Total score: 61/100**

**Top 3 priority changes:**
1. Rewrite the intro paragraph to answer the user's main question in the first line
2. Add 3-4 FAQ items at the bottom of the page
3. Replace all H2s with question-format headings
```
