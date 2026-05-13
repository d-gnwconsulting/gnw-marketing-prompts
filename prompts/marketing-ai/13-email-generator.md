# Email Generator

**Category:** Marketing + AI
**Model tested:** Claude Sonnet 4.6
**Last updated:** 2026-05-13

## What it does

Generates a complete marketing or nurture email — subject line, preview text, and body — from a minimal brief. Works for campaign emails, product announcements, nurture sequences, and re-engagement. Output is ready to paste into any ESP (Mailchimp, HubSpot, Klaviyo, etc.).

## Input needed

- Email goal (campaign, nurture, announcement, re-engagement, etc.)
- Product or topic
- Audience segment
- Key message or offer
- CTA (what you want them to do)
- Tone / brand voice notes (optional)

## Prompt

```
You are an email copywriter. Write a complete marketing email based on the brief below.

The email should feel like it was written by a human who knows the reader — not a mass blast. Be direct, get to the point, and make the CTA obvious.

**Brief:**
Email goal: [campaign / nurture / product announcement / re-engagement / other]
Product or topic: [what this email is about]
Audience: [who's receiving this]
Key message: [the one thing they should take away]
Offer or incentive: [discount, free trial, free resource, or "none"]
CTA: [what you want them to do]
Tone: [optional — e.g., professional, conversational, direct, warm]

**Deliver:**

Subject line: [compelling, under 50 characters]
Preview text: [extends the subject line, under 90 characters]

Body:
[Full email — opening hook, body, CTA. 150-250 words. No filler, no "I hope this email finds you well."]

Then provide:
- 2 alternative subject lines to A/B test
- 1 sentence on the copywriting choice that most affects open rate for this email
```

## Example

**Input:**
- Email goal: Nurture (trial users who haven't activated)
- Product: Project management software for marketing teams
- Audience: Free trial users who signed up 5 days ago but haven't created a project
- Key message: Getting started takes 3 minutes
- Offer: None
- CTA: Create your first project
- Tone: Direct, friendly, no pressure

**Output:**

**Subject line:** You haven't started yet — here's why that's fine
**Preview text:** Most people get stuck on the same thing. Here's the fix.

---

Hey [First name],

You signed up 5 days ago and haven't created a project yet. That's completely normal — most people get stuck deciding what to set up first.

Here's what works: don't start with your biggest campaign. Start with something you're already managing somewhere else — a spreadsheet, a doc, a Slack thread. Move it in. Takes 3 minutes.

Once you see your work laid out in one place, the rest clicks.

[Create your first project →]

If you get stuck, reply to this email. Someone on the team will help.

— [Sender name]

---

**Alternative subject lines:**
- "3 minutes to your first project (really)"
- "Still thinking about it? Start here."

**Key copywriting choice:** The subject line leads with the user's actual behavior ("you haven't started") rather than a product feature — this increases open rate because it feels personal and specific, not promotional.

## Notes

- For sequences, run this prompt once per email and vary the "key message" each time
- Include the previous email's CTA in the brief if writing a follow-up — it prevents repetition
