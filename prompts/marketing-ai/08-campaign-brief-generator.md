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

## Example

**Input:**
- Product: Project management software for marketing teams
- Objective: Generate free trial signups
- Target audience: Marketing managers at B2B companies with 50–500 employees
- Budget: $12,000/month
- Timeline: July–September 2026
- Constraints: Cannot mention competitor names

**Output:**

**1. Campaign summary**
A 3-month digital campaign targeting marketing managers at mid-size B2B companies, designed to drive free trial signups for a project management platform built specifically for marketing workflows. The campaign focuses on the pain of disorganized campaign management and positions the product as the system that brings clarity.

**2. Objective**
Generate 180 free trial signups over 90 days (2/day average) at a cost per signup under $67.

**3. Target audience**
- Demographics: Marketing managers and directors, 28–45, at B2B companies with 50–500 employees
- Psychographics: Responsible for cross-functional campaign execution, frustrated by spreadsheets and missed deadlines, evaluating tools to professionalize their team's workflow
- Pain points: Too many tools that don't talk to each other, lack of visibility into what the team is working on, campaigns that slip because there's no single source of truth

**4. Key message**
Finally, a project management tool built the way marketing teams actually work.

**5. Supporting messages**
- Built for campaigns, not construction projects
- Your whole team. One place. No more status meetings.
- From campaign brief to final report — without switching tabs

**6. Tone and personality**
Direct, confident, a little dry. Talks to marketers like marketers. Avoids: corporate jargon, feature-dumping, "revolutionary" or "game-changing."

**7. Channel recommendations**
- LinkedIn Ads (sponsored content + lead gen forms) — primary channel; audience targeting by job title and company size is precise
- Google Search (branded + category keywords) — captures active searchers comparing tools
- Email nurture sequence — converts trial signups who don't activate within 7 days

**8. Creative directions**
- Direction A: "The chaos brief" — opens with the familiar scene of a marketing team managing a campaign across 6 different tools. Product as the resolution.
- Direction B: Social proof-led — leads with a stat or quote from a marketing team that switched. Outcome-first, feature-second.

**9. KPIs**
- Free trial signups (primary)
- Cost per signup
- Trial-to-paid conversion rate (secondary)
- LinkedIn CTR benchmark: >0.5%

**10. Open questions**
- Is there a referral or incentive for signing up? (affects CTA copy)
- What does the free trial include — full access or limited features?
- Is there a sales-assisted path for larger teams, or fully self-serve?

---

## Notes

- Replace "not defined" inputs with reasonable assumptions and flag them clearly in the brief
- The brief works best when the objective is specific — "increase sales" is weaker than "generate 50 qualified leads in Q3"
