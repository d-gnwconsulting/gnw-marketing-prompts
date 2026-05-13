# GEO & AEO Benchmarks and Reference Data

Industry benchmarks, statistics, and data points for GEO and AEO work. Use this file to ground your optimization decisions in real numbers.

*Last updated: May 2026. Sources linked where available.*

---

## AI Search Adoption

- Perplexity AI reported over 100 million monthly active users as of early 2026
- ChatGPT reached 300 million weekly active users in 2025 (OpenAI)
- Google's AI Overviews appear in approximately 47% of Google searches in the US (as of early 2026)
- AI-generated answers now appear for an estimated 20–30% of all commercial search queries across platforms

---

## Featured Snippets

- Featured snippets appear for approximately 12% of all Google search queries
- Question-format queries ("how to," "what is," "why does") trigger featured snippets at a significantly higher rate than non-question queries
- Pages in positions 1–5 win featured snippets most frequently, but position is not required — pages outside the top 10 have won snippets with well-structured content
- Paragraph snippets average 40–60 words; list snippets average 5–8 items; table snippets average 3–5 rows
- Earning a featured snippet does not guarantee a position zero CTR advantage — CTR varies widely by query intent

---

## Voice Search

- Over 50% of smartphone users use voice search daily (Google, 2024)
- Voice search queries average 5–9 words vs 3–4 words for typed queries
- 70% of voice search answers come from featured snippets
- Voice answers average 29 words and are read from HTTPS pages with high domain authority
- "Near me" voice searches grew over 200% in two years (Google)

---

## GEO Content Performance

- Answer-first paragraphs (where the direct answer appears in the first sentence) are cited by AI systems at a measurably higher rate than context-first paragraphs
- Pages with FAQ sections containing 5+ Q&A pairs have higher AI citation rates than pages without FAQ sections
- Specifically named entities (brand names, people, products with descriptions) are cited more frequently than anonymous entities ("we," "our team," "the solution")
- Question-format H2 headings correlate with both featured snippet wins and AI citation frequency

---

## Schema Markup Impact

- Pages with structured data (schema markup) are eligible for rich results, which increase CTR by an estimated 20–30% on average
- FAQPage schema enables FAQ rich results and makes Q&A content directly extractable by AI
- Organization schema is among the most impactful for brand entity recognition in both Google and AI systems
- Only 33% of websites have any schema markup implemented (Search Engine Journal, 2024)

---

## People Also Ask (PAA)

- PAA boxes appear in approximately 43% of all Google searches (Semrush, 2024)
- The average PAA box shows 3–4 questions initially, expanding to 8–10 on click
- Answering a PAA question on your page increases the probability of appearing in that PAA box
- PAA content overlaps significantly with AI search citation — content optimized for PAA performs well in both environments

---

## Content Formats by Citation Frequency (AI Search)

Based on observed citation patterns across Perplexity, ChatGPT Search, and Gemini:

| Format | AI Citation Frequency | Notes |
|--------|----------------------|-------|
| FAQ sections (5+ items) | High | Most consistently cited format |
| Definition pages | High | Especially for "what is X" queries |
| How-to guides (numbered steps) | High | Structure aids extraction |
| Comparison pages | Medium-High | Tables are highly extractable |
| Long-form blog posts | Medium | Depends heavily on structure |
| Homepage / about page | Low-Medium | Cited for brand, not topics |
| Product/service pages (generic) | Low | Unless well-structured with FAQs |

---

## GEO Audit Scoring Reference

Use this as a benchmark when running the Page Audit prompt:

| Score | GEO Readiness Level | Typical Issues |
|-------|---------------------|---------------|
| 80–100 | Strong | Minor optimization opportunities |
| 60–79 | Moderate | Missing FAQs, weak entity definitions |
| 40–59 | Weak | Answer-buried structure, vague language |
| 20–39 | Poor | No structure, no entities, no direct answers |
| 0–19 | Critical | Content written entirely for keyword ranking, no extractable value |

---

*Sources: Google, OpenAI, Semrush, Search Engine Journal, Perplexity AI, internal GNW Consulting analysis. Statistics reflect conditions as of May 2026 and should be verified against current data for client-facing work.*
