# Brand Voice Checker

**Category:** Marketing + AI
**Model tested:** Claude Sonnet 4.6
**Last updated:** 2026-05-13

## What it does

Reviews a piece of copy against a brand voice description and identifies where it drifts off-brand. Returns specific line-by-line feedback and a revised version that stays true to the brand's voice. Useful for agencies managing multiple client voices or teams with new copywriters.

## Input needed

- Brand voice description (adjectives, dos/don'ts, examples)
- Copy to review

## Prompt

```
You are a brand voice editor. Review the following copy against the brand voice guidelines and identify where it breaks from the brand's personality.

**Brand voice:**
[paste your brand voice description, guidelines, or adjectives here]
[include examples of on-brand and off-brand language if you have them]

**Copy to review:**
[paste the copy here]

Provide:

1. **Overall alignment score** (1-10) with a one-sentence verdict
2. **Line-by-line review** — flag specific phrases that are off-brand and explain why
3. **Revised version** — rewrite the copy staying true to the brand voice, keeping the same message and approximate length
4. **3 words that describe the copy's current voice** vs **3 words that describe the brand's intended voice**
```

## Tips

- The better your brand voice description, the more precise the output. If you don't have a formal brand voice guide, describe it in 3-5 adjectives and add one example of copy you love and one you hate.
- Run this before sending any copy to a client — it catches generic AI-sounding language that slips in during drafting.
