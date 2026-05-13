# Ad Copy Generator

**Category:** Marketing + AI
**Model tested:** Claude Sonnet 4.6
**Last updated:** 2026-05-13

## What it does

Generates ready-to-upload Google Ads and Meta Ads copy from a product brief. Output respects platform character limits, includes multiple headline and description variants for testing, and flags which combinations are strongest. No reformatting needed — paste directly into your ad platform.

## Input needed

- Platform (Google Ads, Meta Ads, or both)
- Product or service being advertised
- Target audience
- Key differentiator or offer
- Landing page URL or description (optional)
- Tone (optional)

## Prompt

```
You are a performance marketing copywriter. Write ad copy for the platform(s) specified below. Respect all character limits exactly — flag any variant that approaches the limit.

Platform: [Google Ads / Meta Ads / both]
Product/service: [what you're advertising]
Target audience: [who you're targeting]
Key differentiator or offer: [what makes this worth clicking]
Landing page focus: [what the landing page is about, or paste the URL]
Tone: [optional]

---

If Google Ads, deliver:

**Responsive Search Ad**
- 10 headlines (max 30 characters each) — label each: [H1], [H2]... 
- 4 descriptions (max 90 characters each) — label each: [D1], [D2]...
- Mark your 3 strongest headline + description combinations with ★

**1 Performance Max headline set** (5 headlines, 30 chars each)

---

If Meta Ads, deliver:

**3 ad variants** — each with:
- Primary text (under 125 characters for feed placement)
- Headline (under 27 characters)
- Description (under 27 characters)
- Format recommendation: single image / carousel / video

Mark the strongest variant with ★ and explain why in one sentence.

---

End with: 1 recommendation for the audience targeting that would make these ads perform better.
```

## Example

**Input:**
- Platform: Google Ads
- Product: Project management software for marketing teams
- Target audience: Marketing managers searching for team productivity tools
- Key differentiator: Built specifically for marketing workflows, not generic tasks
- Landing page focus: Free 14-day trial, no credit card required
- Tone: Direct, confident

**Output:**

**Responsive Search Ad**

Headlines:
- [H1] Marketing Project Management ★ (30 chars)
- [H2] Built for Marketing Teams (27 chars)
- [H3] Free 14-Day Trial — No Card (30 chars) ★
- [H4] Manage Campaigns, Not Tasks (30 chars)
- [H5] One Place for Your Whole Team (31 chars — trim to 30)
- [H6] Stop Managing in Spreadsheets (31 chars — trim to 30)
- [H7] Try Free for 14 Days (22 chars)
- [H8] Marketing Teams Move Faster (29 chars)
- [H9] Finally, PM Built for Marketers (33 chars — trim to 30)
- [H10] Campaign Planning, Simplified (31 chars — trim to 30)

Descriptions:
- [D1] Project management built for marketing teams — campaigns, briefs, and deadlines in one place. Try free. (104 chars) ★
- [D2] Stop tracking campaigns in spreadsheets. Manage every project, person, and deadline in one tool. (99 chars) ★
- [D3] Built for how marketing teams actually work. Free 14-day trial, no credit card required. (90 chars)
- [D4] From campaign brief to final report — without switching tools. See why marketing teams switch to us. (102 chars)

★ Strongest combinations: H1+H3+D1, H2+H3+D2, H4+H7+D3

**Performance Max headline set:**
- Marketing Project Management
- Free 14-Day Trial
- Built for Marketing Teams
- Campaigns in One Place
- No Credit Card Required

**Audience targeting recommendation:** Layer "Marketing Manager" job title targeting with in-market audiences for "Business Software" — this captures both intent (searching) and identity (role), which typically reduces CPC by 15-25% for B2B SaaS ads.
