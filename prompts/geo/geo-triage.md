---
version: 1.0
tested_model: claude-sonnet-4-6
tested_date: 2026-05-13
category: geo
---

# GEO Triage

**Category:** GEO
**Model tested:** Claude Sonnet 4.6
**Last updated:** 2026-05-13

## What it does

The entry point for anyone new to GEO. Takes a page description or URL content and outputs a ranked action list — what to fix first, second, and third — based on impact and effort. Eliminates the paralysis of not knowing where to start.

Run this before any other GEO prompt.

## Input needed

- Page content or description (paste the text, or describe what the page is about)
- Page type (homepage, service page, blog post, product page, etc.)
- One sentence about the target audience

## Prompt

```
You are a GEO (Generative Engine Optimization) strategist doing a rapid triage of a page. Your job is to identify the highest-impact actions this page needs, ranked by impact-to-effort ratio.

GEO is the practice of optimizing content to be cited by AI-powered search engines like Perplexity, ChatGPT, and Gemini.

Page type: [homepage / service page / blog post / product page / other]
Target audience: [who this page is for]

Page content:
[paste your page content or describe the page here]

Produce a GEO Triage Report with this structure:

**Quick wins (do this week — high impact, low effort):**
List 3 actions. For each: what to do, where on the page, and why it matters for GEO.

**Medium-term fixes (do this month — high impact, more effort):**
List 3 actions. Same format.

**Low priority (optional — low impact):**
List 2 actions briefly.

**Which prompt to use next:**
Based on the biggest gap you found, recommend which prompt from this library to run next and why.

Keep each action to 2-3 sentences max. Be specific — reference actual content from the page, not generic advice.
```

## Example

**Input:**
- Page type: Service page
- Target audience: HR directors at companies with 200+ employees
- Page content: "We offer comprehensive HR consulting services to help your organization thrive. Our experienced consultants work closely with your team to develop customized solutions. Services include talent acquisition, performance management, and organizational development. Contact us to schedule a consultation."

**Output:**

**Quick wins (do this week):**

1. **Rewrite the opening sentence** — Replace "We offer comprehensive HR consulting services" with a direct, entity-specific statement: "[Company name] provides HR consulting services — talent acquisition, performance management, and organizational development — for companies with 200+ employees." The current opener is uncitable; the rewrite gives AI a quotable definition.

2. **Add question-format H2s** — The page has no headings. Add at least 3: "What HR Consulting Services Does [Company] Offer?", "Who Are [Company]'s HR Consulting Services For?", and "How Does the [Company] HR Consulting Process Work?" These directly match how HR directors query AI tools.

3. **Remove "Contact us to schedule a consultation" from the intro** — CTAs in the first paragraph interrupt content before AI can extract value. Move it to the bottom.

**Medium-term fixes (do this month):**

1. **Add a FAQ section** — Write 5-6 Q&A pairs answering the questions HR directors ask before hiring a consultant (cost, timeline, what's included, how results are measured). FAQ content is the most-cited format in AI responses.

2. **Strengthen entity definitions** — "Our experienced consultants" names nobody. Add consultant bios or at minimum a description of team credentials. AI systems cite sources with identifiable people, not anonymous teams.

3. **Add a definition of each service** — "Talent acquisition," "performance management," and "organizational development" are listed but never defined. A 2-sentence definition of each gives AI extractable content for each service query.

**Low priority:**

1. Add schema markup (ProfessionalService type) — helpful but won't move the needle until content issues are fixed.
2. Internal linking to related blog content — beneficial for SEO, minor GEO impact on its own.

**Which prompt to use next:**
Run **Entity Strengthener** (prompt 05) first — the page's biggest gap is unresolvable entities ("we," "our team," "your organization"). Fixing that will amplify every other change you make.
