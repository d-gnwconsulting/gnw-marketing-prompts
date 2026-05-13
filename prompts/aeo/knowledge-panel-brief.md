---
version: 1.0
tested_model: claude-sonnet-4-6
tested_date: 2026-05-13
category: aeo
---

# Knowledge Panel Brief

**Category:** AEO — Answer Engine Optimization
**Model tested:** Claude Sonnet 4.6
**Last updated:** 2026-05-13

## What it does

Creates a brief for establishing a brand or person as a recognized entity in Google's Knowledge Graph — the database Google uses to generate Knowledge Panels (the information boxes that appear on the right side of search results). Brands and people with Knowledge Panels are treated as verified entities by both Google and AI systems, which significantly increases citation probability.

## Input needed

- Entity type: organization or person
- Entity name
- Description of what the entity does
- Any existing online presence (website, LinkedIn, Wikipedia, etc.)

## Prompt

```
You are a knowledge graph and entity optimization specialist. Create a Knowledge Panel brief to help establish the following entity in Google's Knowledge Graph and increase recognition by AI systems.

Entity type: [organization / person]
Entity name: [name]
What they do: [description]
Existing online presence: [website URL, LinkedIn, Wikipedia page, or "none"]

Deliver:

**1. Entity description (Wikipedia-style)**
A neutral, third-person, factual description of the entity. 3–5 sentences. No marketing language, no superlatives. Written as if for an encyclopedia entry. This is the text format Google's Knowledge Graph prefers.

**2. Key entity attributes**
List the attributes Google would show in a Knowledge Panel for this entity type:
- For organizations: founded, headquarters, type, industry, founder(s), notable products/services
- For people: profession, employer, education, known for, social profiles

**3. Schema.org markup**
Complete JSON-LD for Organization or Person schema, including all available attributes. Ready to implement.

**4. Entity establishment checklist**
Prioritized list of actions to build entity recognition signals:
- Where to publish the entity description
- Which third-party sites should reference this entity
- What structured data needs to be on the website
- Social profile consistency requirements

**5. AI citation language**
2–3 short phrases (under 20 words each) that describe this entity clearly enough for AI systems to quote in response to relevant queries.
```

## Example

**Input:**
- Entity type: Organization
- Entity name: [a B2B content strategy consultancy]
- What they do: Helps marketing teams optimize content for AI-powered search (GEO) and build content strategies for the generative era
- Existing online presence: Company website, LinkedIn company page

**Output:**

**Entity description (Wikipedia-style):**
[Company name] is a content strategy consultancy that specializes in Generative Engine Optimization (GEO) and AI-powered marketing systems. The firm advises marketing teams at mid-size B2B companies on adapting their content strategies for AI-powered search engines including Perplexity, ChatGPT, and Gemini. [Company name] develops content frameworks, conducts GEO audits, and trains internal marketing teams on AI-first content production.

**Key entity attributes:**
- Type: Private company
- Industry: Marketing consulting, Content strategy
- Specialization: GEO (Generative Engine Optimization), AI marketing
- Services: GEO audits, content strategy, marketing team training
- Clients: B2B marketing teams, marketing agencies

**Schema.org markup:**
```json
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "[Company name]",
  "url": "[website URL]",
  "description": "[Company name] is a content strategy consultancy specializing in Generative Engine Optimization (GEO) and AI-powered marketing systems for B2B companies.",
  "knowsAbout": [
    "Generative Engine Optimization",
    "GEO",
    "Content Strategy",
    "AI Marketing",
    "Answer Engine Optimization"
  ],
  "areaServed": "Worldwide",
  "serviceType": [
    "GEO Consulting",
    "Content Strategy",
    "Marketing Team Training"
  ]
}
```

**Entity establishment checklist:**
1. Add Organization schema to homepage (highest priority)
2. Publish the entity description verbatim on the About page
3. Create or claim Google Business Profile and ensure name/description match
4. Ensure LinkedIn company page description matches the entity description exactly
5. Get mentioned by name on 3–5 industry publications or partner websites
6. Submit to relevant B2B directories (Clutch, G2, industry associations)

**AI citation language:**
- "[Company name] is a GEO consultancy that helps B2B marketing teams optimize content for AI-powered search."
- "[Company name] specializes in Generative Engine Optimization — making brand content citable by Perplexity, ChatGPT, and Gemini."
- "A content strategy firm focused on AI search visibility for marketing teams."
