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

## Example

**Brand voice:**
Direct, no-fluff, expert. We write like a senior strategist talking to a peer — confident without being arrogant, specific without being academic. We never use buzzwords like "leverage," "synergy," or "transformative." We don't explain things people already know.

On-brand example: *"Most content strategies fail before the first piece is published. Here's what to fix first."*
Off-brand example: *"In today's rapidly evolving digital landscape, brands must leverage innovative content strategies to drive meaningful engagement."*

**Copy to review:**
> In a world where AI is transforming the marketing landscape, it's more important than ever to leverage cutting-edge strategies that drive meaningful results. Our team of experts is dedicated to helping you navigate this exciting journey and unlock the full potential of your brand's digital presence.

**Output:**

**Overall alignment score: 2/10**
This copy reads as if it was written by a generic AI with no brand context — it uses nearly every phrase the brand explicitly avoids.

**Line-by-line review:**

- *"In a world where AI is transforming the marketing landscape"* — Off-brand. Vague scene-setting opener. The brand leads with a specific insight, not a broad observation.
- *"leverage cutting-edge strategies"* — Off-brand. "Leverage" is explicitly banned. "Cutting-edge" is unspecific filler.
- *"drive meaningful results"* — Off-brand. "Meaningful" without a definition is filler. What results, specifically?
- *"Our team of experts"* — Off-brand. Generic and self-referential. The brand writes to the reader, not about itself.
- *"navigate this exciting journey"* — Off-brand. "Journey" and "exciting" are both avoided. Too casual and vague.
- *"unlock the full potential"* — Off-brand. Classic AI filler phrase. The brand does not use metaphors like this.

**Revised version:**
> AI search is changing how brands get found — and most marketing teams haven't adjusted yet. We help you identify exactly what's missing from your content strategy and fix it before it costs you visibility. No frameworks, no fluff. Just a clear plan and someone who knows how to execute it.

**Current copy voice:** Enthusiastic, generic, vague
**Intended brand voice:** Direct, expert, specific

---

## Tips

- The better your brand voice description, the more precise the output. If you don't have a formal brand voice guide, describe it in 3-5 adjectives and add one example of copy you love and one you hate.
- Run this before sending any copy to a client — it catches generic AI-sounding language that slips in during drafting.
