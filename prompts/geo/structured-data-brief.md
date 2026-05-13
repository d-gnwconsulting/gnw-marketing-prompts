---
version: 1.0
tested_model: claude-sonnet-4-6
tested_date: 2026-05-13
category: geo
---

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

## Example

**Input:**
- Brand name: [a B2B SaaS company]
- Website: [their URL]
- Page type: Homepage
- Page content: Homepage for a project management tool built for marketing teams, with sections covering features, pricing, integrations, and customer testimonials

**Output:**

**1. Organization — impact: high**
Establishes the brand as a recognized entity. AI systems use this to describe the company in responses.

```json
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "[Company name]",
  "url": "[URL]",
  "description": "Project management software built for marketing teams, with workflow automation, campaign tracking, and cross-channel reporting.",
  "knowsAbout": ["marketing project management", "campaign workflow software", "marketing team collaboration tools"]
}
```

**2. SoftwareApplication — impact: high**
Directly tells AI what type of product this is and what it does. Critical for product-category queries.

```json
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "[Product name]",
  "applicationCategory": "BusinessApplication",
  "operatingSystem": "Web",
  "description": "Project management platform for marketing teams. Includes campaign planning, task assignment, deadline tracking, and integrations with major marketing tools.",
  "offers": {
    "@type": "Offer",
    "price": "29",
    "priceCurrency": "USD",
    "priceSpecification": {
      "@type": "UnitPriceSpecification",
      "billingIncrement": "month"
    }
  }
}
```

**3. FAQPage — impact: medium**
Enables FAQ rich results and gives AI extractable Q&A pairs from your homepage.

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "What is [Product name] used for?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "[Product name] is a project management tool built specifically for marketing teams. It helps teams plan campaigns, assign tasks, track deadlines, and report on results — all in one place."
      }
    },
    {
      "@type": "Question",
      "name": "How much does [Product name] cost?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "[Product name] starts at $29 per month per user. A free 14-day trial is available with no credit card required."
      }
    }
  ]
}
```

**4. Review / AggregateRating — impact: medium**
If the page includes testimonials or a star rating, this schema surfaces that credibility signal to AI systems.

```json
{
  "@context": "https://schema.org",
  "@type": "SoftwareApplication",
  "name": "[Product name]",
  "aggregateRating": {
    "@type": "AggregateRating",
    "ratingValue": "4.7",
    "reviewCount": "312"
  }
}
```
