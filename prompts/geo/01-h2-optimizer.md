# H2 Optimizer for GEO

**Category:** GEO
**Model tested:** Claude Sonnet 4.6
**Last updated:** 2026-05-13

## What it does

Rewrites H2 headings to increase the probability of being cited by AI-powered search engines (Perplexity, ChatGPT, Gemini). AI systems favor headings that are phrased as questions or clear statements that directly match how users query them.

## Input needed

- Original H2 heading
- Page topic or context (1-2 sentences)
- Target audience

## Prompt

```
You are a GEO (Generative Engine Optimization) specialist. Your job is to rewrite H2 headings so they are more likely to be cited by AI-powered search engines like Perplexity, ChatGPT, and Gemini.

AI search engines favor headings that:
- Are phrased as questions users actually ask
- Are specific and contain the topic entity clearly
- Sound like a direct, authoritative answer to a real query
- Avoid vague marketing language

Here is the H2 I want you to optimize:

Original H2: [paste your H2 here]
Page topic: [brief description of what the page is about]
Target audience: [who reads this page]

Give me 3 rewritten versions of this H2, ordered from most to least conversational. For each one, explain in one sentence why it performs better for GEO.
```

## Example

**Input:**
- Original H2: `What We Do`
- Page topic: Full-service digital marketing agency services page
- Target audience: Marketing directors and CMOs at mid-size B2B companies

**Output:**

1. `What Does a Full-Service Digital Marketing Agency Do for B2B Companies?`
   Why it works: mirrors the exact phrasing a user types into an AI search engine — question format, entity-specific, no filler.

2. `Digital Marketing Services for B2B Companies: Strategy, Content, and Paid Media`
   Why it works: contains specific service categories that help AI classify and cite the page for relevant queries.

3. `How a Full-Service Digital Marketing Agency Drives B2B Revenue`
   Why it works: action-outcome structure gives AI a clear answer frame and ties the heading to a business result.
