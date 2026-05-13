---
version: 1.0
tested_model: claude-sonnet-4-6
tested_date: 2026-05-13
category: geo
---

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

## Example

**Input page content:**
> We are a passionate team of marketers dedicated to helping businesses grow. With years of experience in the industry, we offer a range of solutions tailored to your needs. Our approach is data-driven and results-oriented. Contact us today to learn more about what we can do for your brand.

**Output:**

**GEO Audit Results**

1. **Answer-first structure: 6/20**
   - The page never states what the company does or who it serves. The first sentence should answer: what do you do, for whom, and with what result.
   - Remove the "Contact us" CTA from the intro — it interrupts the content before AI can extract any value.

2. **Entity clarity: 4/20**
   - "We," "our team," and "businesses" are unresolvable to any AI system. Replace with the actual company name and specific client types.
   - "A range of solutions" names nothing. List the actual service categories.

3. **Query alignment: 5/20**
   - "Passionate team" and "tailored solutions" are marketing filler — no user queries these phrases to an AI.
   - Rewrite using the language your clients actually use when searching: "paid media," "content strategy," "lead generation."

4. **Citability: 3/20**
   - There is no single quotable statement. AI needs a clear, standalone sentence it can extract as a direct answer.
   - Add at least one definition or factual claim per section.

5. **Structured formatting: 8/20**
   - Single block of text. AI cannot distinguish topics or extract specific answers.
   - Break into headed sections, each answering one question.

**Total score: 26/100**

**Top 3 priority changes:**
1. Rewrite the first sentence to state: who you are, what you do, and who you serve — in that order, with no warm-up
2. Replace all pronouns and vague nouns with the company name and specific service names
3. Add H2 headers to every section, each phrased as a question a user would ask an AI
