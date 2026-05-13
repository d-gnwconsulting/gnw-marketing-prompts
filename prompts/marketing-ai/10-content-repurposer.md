# Content Repurposer

**Category:** Marketing + AI
**Model tested:** Claude Sonnet 4.6
**Last updated:** 2026-05-13

## What it does

Takes a long-form piece of content (blog post, report, interview, newsletter) and generates adapted versions for three different channels, each respecting that channel's native format, length, and tone. Eliminates the copy-paste-shorten approach that produces bad social content.

## Input needed

- Original long-form content
- Target channels (choose 3 from: LinkedIn, Instagram, X/Twitter, email newsletter, YouTube description, WhatsApp/Telegram, short-form video script)
- Brand voice or tone notes (optional)

## Prompt

```
You are a content strategist and copywriter. Repurpose the following content into three channel-specific versions.

Each version must be native to its channel — not a shortened copy of the original. Respect the format, tone, and user behavior of each platform.

**Original content:**
[paste your long-form content here]

**Target channels:** [list 3 channels]

**Brand voice notes:** [optional — adjectives or tone guidance]

For each channel, produce:
- The content itself (ready to publish)
- A one-line note on the key adaptation decision you made for that channel

**Channel guidelines to follow:**
- **LinkedIn**: Professional but human. Lead with an insight or contrarian take. 150-300 words. No hashtag spam (max 3 relevant ones).
- **Instagram**: Hook in the first line. Short punchy sentences. Storytelling or list format. 80-150 words + 5-10 hashtags.
- **X/Twitter**: One sharp idea per tweet. 280 chars max. Thread format if the content is complex (max 5 tweets).
- **Email newsletter**: Subject line + preview text + body. Conversational, value-first. 200-400 words.
- **YouTube description**: SEO-optimized. First 2 lines must be compelling (they show before "more"). 150-300 words + timestamp structure if relevant.
- **Short-form video script**: Hook (0-3s) + body (3-45s) + CTA (last 5s). Written as spoken word.
```

## Example

**Input:**
- Original content: Blog post titled "Why Your Content Isn't Showing Up in AI Search (And What to Fix)"
- Target channels: LinkedIn, Email newsletter, Short-form video script
- Brand voice: Direct, expert, no fluff

**Output:**

---

**LINKEDIN**

Most brands have a content problem they don't know about yet.

They're publishing consistently. Getting decent traffic. Ranking on Google for a few things.

But when someone asks Perplexity or ChatGPT about their industry, they don't appear. Not even close.

The reason is almost always the same: content written for keyword rankings doesn't work for AI citation. Different systems, different rules.

The three fixes that move the needle fastest:
→ Rewrite your H2s as questions people actually ask
→ Put the answer in the first sentence of every section
→ Add a FAQ block to every page that targets an informational query

None of these require new content. Most teams can do all three in a week.

If your content team is still writing for 2019 Google, this is the gap.

*Key adaptation: Opened with a relatable problem statement, used short punchy lines native to LinkedIn, structured the insight as a numbered list for scannability.*

---

**EMAIL NEWSLETTER**

**Subject:** Your content isn't broken. It's optimized for the wrong thing.
**Preview:** Here's what AI search actually needs from you.

---

If your organic traffic is flat or declining, there's a good chance it's not a quantity problem — it's a format problem.

Most content is written to rank in Google: target a keyword, build links, optimize the title tag. That system still works, partially. But it doesn't work for AI-powered search engines like Perplexity, ChatGPT, or Gemini — and those are where a growing share of discovery is happening.

AI systems don't rank pages. They extract answers. And they favor content that:

- Gets to the point immediately (answer-first structure)
- Uses specific language, not vague descriptors
- Has clear H2 headings that match how people phrase questions
- Includes direct, quotable statements

The good news: you probably don't need to create new content. You need to reformat what you already have.

The three highest-impact changes you can make this week:

1. Rewrite your H2s as direct questions
2. Move your main point to the first sentence of each section
3. Add a FAQ block to your top 5 pages

That's it. No new content budget. No new tools.

Reply if you want the prompt we use to do this with Claude.

*Key adaptation: Added subject line + preview text, expanded the insight into a scannable body with a clear CTA, kept it actionable and outcome-focused.*

---

**SHORT-FORM VIDEO SCRIPT**

**Hook (0–3s):**
Your content isn't showing up in AI search — and it's not because you're not publishing enough.

**Body (3–40s):**
AI search engines like Perplexity and ChatGPT don't rank pages — they extract answers. So if your content is written for Google, it's probably invisible to AI.

The fix is simpler than you think. Three things:

One — rewrite your H2 headings as questions. Not "Our Services." "What services does [your company] offer?"

Two — put the answer in the first sentence of every section. AI skips warm-up paragraphs.

Three — add a FAQ section to your most important pages. It's the most-cited content format in AI responses.

You don't need new content. You need to reformat what you already have.

**CTA (last 5s):**
Link in bio — free prompt to do this in Claude in under 10 minutes.

*Key adaptation: Tight hook with a counterintuitive statement, body structured as a numbered list for clarity when spoken, CTA drives to a specific action.*

---

## Notes

- For best results, paste the full original content — not a summary. The prompt extracts the most repurposable insights itself.
- If your channels aren't in the list above, describe the platform and its native format in the brand voice notes field.
