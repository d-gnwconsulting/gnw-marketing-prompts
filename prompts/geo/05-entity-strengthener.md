# Entity Strengthener

**Category:** GEO
**Model tested:** Claude Sonnet 4.6
**Last updated:** 2026-05-13

## What it does

Identifies weak or underspecified entities in your content (brand names, people, products, locations, topics) and suggests how to describe them more completely. AI systems rely on entities to understand what content is about — weak entities mean your content gets passed over.

## Input needed

- Page content or section of copy
- Your brand name and what it does (for context)

## Prompt

```
You are a GEO entity analyst. Review the following content and identify all entities that are weakly defined or missing important context.

An entity is weak when:
- It's referred to by pronoun or vague noun ("we", "our solution", "the platform") without a proper name
- It lacks descriptive context (a person mentioned without title/role, a product without category)
- It appears only once when repetition would reinforce it
- It's missing attributes that AI systems use to classify it (industry, location, type, function)

Brand context: [your brand name and one sentence about what it does]

Content to analyze:
[paste your content here]

Produce a table with:
| Weak entity | Current usage | Suggested improvement | Reason |

Then rewrite the 2-3 most critical instances directly in the text so I can see the improvement in context.
```

## Example output

| Weak entity | Current usage | Suggested improvement | Reason |
|-------------|--------------|----------------------|--------|
| Brand | "our team" | "GNW Consulting's strategy team" | AI can't associate anonymous "team" with the brand |
| Product | "the tool" | "GNW's GEO Intelligence dashboard" | Needs a proper name and category |
| Person | "our founder" | "Deris H., founder of GNW Consulting" | People entities need name + role |
