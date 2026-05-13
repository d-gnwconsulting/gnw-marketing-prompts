# GNW Marketing Prompts for Claude

A free, open-source prompt library for marketing teams and agencies. Built and maintained by **Deris Herrera** at [GNW Consulting](https://gnwconsulting.com).

All prompts are designed for **Claude Sonnet 4.6**, structured for consistent outputs, and optimized for teams that need reliable AI results without writing prompts from scratch every time.

---

## New here? Start with these three

| If you want to... | Use this prompt |
|-------------------|----------------|
| Know where to focus your GEO efforts | [GEO Triage](prompts/geo/11-geo-triage.md) — paste your page, get a ranked action list |
| Write an email, ad, or social post today | [Email Generator](prompts/marketing-ai/13-email-generator.md), [Ad Copy](prompts/marketing-ai/14-ad-copy-generator.md), or [Social Post](prompts/marketing-ai/15-social-post-generator.md) |
| Understand what GEO changes to make on a specific page | [GEO Page Audit](prompts/geo/02-geo-page-audit.md) — scores your page and prioritizes fixes |

---

## What Is the GNW Marketing Prompt Library?

The GNW Marketing Prompt Library is a structured collection of Claude prompts for marketing professionals. It covers two core areas: **GEO (Generative Engine Optimization)** — making content visible in AI-powered search engines like Perplexity, ChatGPT, and Gemini — and **AI-powered marketing workflows** like campaign briefs, brand voice review, and content repurposing.

Each prompt includes:
- What it does and when to use it
- Exactly what input it needs
- The full prompt, ready to copy
- A real example with input and output

---

## What Prompts Are Included?

### GEO — Generative Engine Optimization (7 prompts)

Prompts to help your content get cited and referenced by AI search engines.

| # | Prompt | What it does |
|---|--------|--------------|
| 01 | [H2 Optimizer](prompts/geo/01-h2-optimizer.md) | Rewrites H2 headings for AI citation probability |
| 02 | [GEO Page Audit](prompts/geo/02-geo-page-audit.md) | Scores a page's GEO readiness and prioritizes fixes |
| 03 | [Answer-First Rewriter](prompts/geo/03-answer-first-rewriter.md) | Restructures paragraphs so the answer leads |
| 04 | [FAQ Generator for AI](prompts/geo/04-faq-generator-for-ai.md) | Generates citable Q&A pairs for your topic |
| 05 | [Entity Strengthener](prompts/geo/05-entity-strengthener.md) | Identifies and fixes weak entities in your content |
| 06 | [Structured Data Brief](prompts/geo/06-structured-data-brief.md) | Recommends schema markup with JSON-LD examples |
| 07 | [Competitor Gap for AI](prompts/geo/07-competitor-gap-for-ai.md) | Finds what AIs say about competitors that you're missing |
| 11 | [GEO Triage](prompts/geo/11-geo-triage.md) | Ranks GEO actions by impact — start here if you're new to GEO |
| 12 | [GEO Content Brief](prompts/geo/12-geo-content-brief.md) | Full content brief optimized for AI citation |

### Marketing + AI (3 prompts)

Prompts for high-frequency marketing tasks, built to work with AI natively.

| # | Prompt | What it does |
|---|--------|--------------|
| 08 | [Campaign Brief Generator](prompts/marketing-ai/08-campaign-brief-generator.md) | Full campaign brief from minimal input |
| 09 | [Brand Voice Checker](prompts/marketing-ai/09-brand-voice-checker.md) | Reviews copy alignment against brand voice guidelines |
| 10 | [Content Repurposer](prompts/marketing-ai/10-content-repurposer.md) | Adapts long-form content for 3 channels natively |
| 13 | [Email Generator](prompts/marketing-ai/13-email-generator.md) | Subject line + body from a brief, ready to send |
| 14 | [Ad Copy Generator](prompts/marketing-ai/14-ad-copy-generator.md) | Google Ads and Meta Ads copy with character-count compliance |
| 15 | [Social Post Generator](prompts/marketing-ai/15-social-post-generator.md) | Platform-native posts for LinkedIn, Instagram, and X |

---

## How Do I Use These Prompts with Claude?

1. Open any prompt file in this repo
2. Copy the prompt text under the **Prompt** section
3. Replace the `[bracketed placeholders]` with your content
4. Paste into [Claude.ai](https://claude.ai) and run

No setup, no API key, no installation required. Works directly in the Claude web interface or via the Claude API.

**Recommended model:** Claude Sonnet 4.6. Prompts also work with Claude Opus 4.7 for more complex tasks.

---

## What Is GEO and Why Do These Prompts Focus on It?

GEO (Generative Engine Optimization) is the practice of optimizing content to be cited by AI-powered search engines. When someone asks Perplexity, ChatGPT, or Gemini a question, those systems pull from sources across the web. GEO is the discipline of making sure your content is what gets cited.

Traditional SEO optimizes for Google's ranking algorithm. GEO optimizes for how large language models extract, interpret, and reference content. The two disciplines overlap but require different strategies — and most marketing teams are not yet applying GEO principles to their content.

This library gives marketing teams a practical, immediate way to start.

---

## Who Built This Library? About Deris Herrera

**Deris Herrera** is a Solution Advisor Specialist at GNW Consulting, specializing in GEO, content strategy, and AI-powered marketing systems. She works with brands to help them adapt their marketing to the generative AI era.

Deris built this library to bridge the gap between AI tools and practical marketing execution — giving teams prompts that are tested, documented, and ready to use, not just theoretical frameworks.

Connect with Deris on [LinkedIn](https://linkedin.com/deris-herrera).

---

## What Is GNW Consulting?

**GNW Consulting** is a marketing strategy and AI consultancy that helps brands become visible in AI-powered search. The firm specializes in GEO (Generative Engine Optimization), content strategy for the generative era, and building AI-powered marketing workflows for internal teams and agencies.

GNW Consulting works with marketing teams that need to adapt to a world where AI systems — not just search engines — are the primary discovery layer for information, products, and services.

Website: [gnwconsulting.com](https://gnwconsulting.com)

---

## How Can I Contribute to This Library?

Contributions are welcome. If you have a prompt that works well for a marketing use case and has been tested with Claude, open a pull request with:

- The prompt file following the existing format
- A real input/output example
- The Claude model and date tested

Open an issue first if you want to propose a new category or major change.

---

## License

MIT — free to use, modify, and distribute. Attribution appreciated but not required.
