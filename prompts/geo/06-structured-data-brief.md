# Structured Data Brief

**Category:** GEO
**Model tested:** Claude Sonnet 4.6
**Last updated:** 2026-05-13

## What it does

Analyzes your page content and recommends which schema markup types to implement, with example JSON-LD snippets. Structured data helps AI systems and search engines understand your content precisely, increasing citation probability.

## Input needed

- Page content or description
- Page type (homepage, service page, blog post, product page, etc.)
- Brand name and website URL

## Prompt

```
You are a structured data specialist with expertise in schema.org markup for GEO and SEO.

Analyze the following page and recommend the most impactful schema markup types to implement. For each type, explain why it matters for AI search visibility and provide a ready-to-use JSON-LD example with realistic placeholder values.

Brand name: [your brand name]
Website: [your URL]
Page type: [homepage / service page / blog post / product page / other]

Page content:
[paste your page content or description here]

For each recommended schema type:
1. Schema type name
2. Why it improves GEO for this specific page
3. JSON-LD snippet (complete, ready to customize)

Prioritize by impact. Maximum 4 schema types.
```

## Example output

**1. Organization schema**
Helps AI systems identify and describe your brand as an entity.

```json
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "GNW Consulting",
  "url": "https://gnwconsulting.com",
  "description": "Marketing strategy and GEO consultancy helping brands appear in AI-powered search.",
  "founder": {
    "@type": "Person",
    "name": "Deris H."
  },
  "areaServed": "Worldwide",
  "knowsAbout": ["GEO", "Generative Engine Optimization", "Marketing Strategy", "AI Marketing"]
}
```
