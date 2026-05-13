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

## Notes

- For best results, paste the full original content — not a summary. The prompt extracts the most repurposable insights itself.
- If your channels aren't in the list above, describe the platform and its native format in the brand voice notes field.
