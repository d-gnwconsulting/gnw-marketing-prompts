# Campaign Brief Generator

**Category:** Marketing + AI
**Model tested:** Claude Sonnet 4.6
**Last updated:** 2026-05-13

## What it does

Generates a complete, structured campaign brief from minimal input. Eliminates the blank-page problem when starting a new campaign and ensures no critical element is left undefined before execution begins.

## Input needed

- Product or service being promoted
- Campaign objective
- Target audience
- Budget range (optional)
- Timeline (optional)
- Any constraints or mandatories (optional)

## Prompt

```
You are a senior marketing strategist. Generate a complete campaign brief based on the inputs below.

The brief should be detailed enough for a creative team, media buyer, and copywriter to begin work without needing a kickoff call.

**Inputs:**
Product/service: [what you're promoting]
Objective: [what success looks like — sales, leads, awareness, etc.]
Target audience: [who you're talking to]
Budget: [range or "not defined"]
Timeline: [campaign dates or "not defined"]
Constraints/mandatories: [anything that must or must not be included]

**Generate the brief with these sections:**

1. **Campaign summary** (2-3 sentences)
2. **Objective** (specific, measurable if possible)
3. **Target audience** (demographics + psychographics + pain points)
4. **Key message** (the one thing the audience should take away)
5. **Supporting messages** (2-3 secondary points)
6. **Tone and personality** (3-5 adjectives + what to avoid)
7. **Channel recommendations** (with rationale)
8. **Creative directions** (2 distinct creative angles to explore)
9. **KPIs** (what to measure)
10. **Open questions** (what needs to be defined before launch)
```

## Notes

- Replace "not defined" inputs with reasonable assumptions and flag them clearly in the brief
- The brief works best when the objective is specific — "increase sales" is weaker than "generate 50 qualified leads in Q3"
