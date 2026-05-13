# Social Post Generator

**Category:** Marketing + AI
**Model tested:** Claude Sonnet 4.6
**Last updated:** 2026-05-13

## What it does

Turns any source content (blog post, product update, campaign brief, data point, or idea) into platform-native social posts for LinkedIn, Instagram, and X. Each post is written for how people actually consume content on that platform — not a shortened copy of the original.

## Input needed

- Source content (paste text, or describe the idea/update)
- Which platforms (LinkedIn, Instagram, X, or all three)
- Goal (awareness, engagement, traffic, or lead gen)
- Brand voice notes (optional)

## Prompt

```
You are a social media copywriter. Turn the source content below into platform-native posts. Write each post for how people actually read on that platform — not a compressed version of the source.

Source content: [paste your content, or describe the idea/update in a few sentences]
Platforms: [LinkedIn / Instagram / X / all three]
Goal: [awareness / engagement / traffic to a link / lead generation]
Brand voice: [optional — e.g., direct, expert, conversational, bold]

---

**LinkedIn post:**
- Length: 150–250 words
- Structure: Hook (1 line) → Insight or story → Practical takeaway → Optional CTA
- Tone: Professional but human. Write like a smart colleague sharing something useful, not a brand announcement.
- Formatting: Short paragraphs, line breaks between ideas. Max 3 hashtags at the end.

**Instagram post:**
- Length: 80–130 words
- Structure: Hook (must stop the scroll) → Short punchy body → CTA
- Tone: More direct and visual-forward. Assume there's an image — write to complement it, not describe it.
- Formatting: Short sentences, natural line breaks. 5–8 relevant hashtags at the end.

**X post:**
- If the idea fits in 280 characters: write a single tweet.
- If the idea needs more space: write a thread of 3–5 tweets. Number each tweet [1/n].
- Tone: Sharp, confident, no padding. Every word earns its place.

After all posts, give one sentence on the angle that would perform best for the stated goal, and why.
```

## Example

**Input:**
- Source: Blog post explaining that most brands don't appear when users ask AI tools about their industry — and that 3 content fixes (answer-first structure, question-format H2s, FAQ sections) can change that quickly
- Platforms: All three
- Goal: Traffic to the blog post
- Brand voice: Direct, expert, no fluff

**Output:**

---

**LinkedIn:**

Most brands have a search problem they don't know about yet.

They're publishing consistently. Ranking on a few keywords. Getting traffic.

But when someone asks Perplexity or ChatGPT about their industry — they don't appear. Not even close.

The reason is almost always the same: content written for Google's algorithm doesn't get cited by AI. Different systems, different rules.

The three fixes that move the needle fastest are surprisingly simple:
→ Rewrite H2s as questions people actually ask
→ Put the answer in the first sentence of every section
→ Add a FAQ block to any page targeting an informational query

None of these require new content. Most teams can apply all three in a week.

If you're still writing for 2019 Google, this is the gap. Full breakdown at the link.

#GEO #ContentStrategy #AIMarketing

---

**Instagram:**

Your content isn't showing up in AI search — and publishing more won't fix it.

AI tools like Perplexity and ChatGPT don't rank pages. They extract answers. So if your content isn't structured to be quoted, it's invisible.

Three fixes that actually work:
→ Question-format H2s
→ Answer-first paragraphs
→ FAQ sections on every key page

No new content needed. Just a smarter format.

Link in bio for the full breakdown.

#ContentStrategy #GEO #AIMarketing #MarketingTips #DigitalMarketing #ContentMarketing #SEO #AISearch

---

**X (thread):**

[1/4] Most brands don't appear when users ask AI tools about their industry.

Not because they don't publish enough. Because they're optimized for the wrong system.

[2/4] AI search engines don't rank pages — they extract answers.

Content written for Google keywords gets skipped. Content written to be quoted gets cited.

[3/4] Three fixes, no new content needed:

→ Rewrite H2s as questions
→ Answer first, context second
→ Add a FAQ block to key pages

Most teams can do all three in a week.

[4/4] Full breakdown here: [link]

---

**Best angle for traffic goal:** The LinkedIn post will drive the most clicks — the list format creates a "I need to read the full version" pull, and the audience (marketing professionals) has high intent to learn tactical fixes. The thread works well for reach if you have an engaged X following, but LinkedIn is more reliable for B2B traffic.
