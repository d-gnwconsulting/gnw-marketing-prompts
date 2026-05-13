# How to Get Better Results from Claude: A Marketing Team's Guide

This guide translates Anthropic's official prompt engineering best practices into marketing-specific advice. Every principle here is sourced from [Anthropic's prompt engineering documentation](https://platform.claude.com/docs/en/docs/build-with-claude/prompt-engineering/overview) — customized for how marketing teams actually work.

Use this before running any prompt in this library.

---

## 1. Treat Claude like a brilliant new hire, not a search engine

**What Anthropic says:** Think of Claude as a brilliant but new employee who lacks context on your norms and workflows. The more precisely you explain what you want, the better the result.

**What this means for marketing:**

Claude doesn't know your client, your brand voice, your campaign history, or your industry unless you tell it. Every prompt is a blank slate.

**Don't do this:**
```
Write an email for our product launch.
```

**Do this instead:**
```
Write a product launch email for [product name], a B2B SaaS tool for HR teams.
Audience: HR directors at companies with 200–500 employees.
Tone: Direct and confident, no corporate filler.
Goal: Drive free trial signups.
CTA: "Start your free trial"
Length: Under 200 words.
```

The second version gives Claude everything it needs. You'll get a usable draft on the first run.

---

## 2. Explain the WHY, not just the WHAT

**What Anthropic says:** Providing context or motivation behind your instructions helps Claude better understand your goals and deliver more targeted responses. Claude is smart enough to generalize from the explanation.

**What this means for marketing:**

When you tell Claude *why* a constraint exists, it applies that constraint intelligently instead of mechanically.

**Don't do this:**
```
Don't mention pricing in the ad copy.
```

**Do this instead:**
```
Don't mention pricing in the ad copy — we're running this in awareness campaigns where price anchoring too early reduces click-through. The goal is curiosity, not conversion.
```

The second version lets Claude make smart decisions about related choices (what to include instead, how to frame the CTA) without you micromanaging every word.

---

## 3. Show Claude an example of what good looks like

**What Anthropic says:** Examples are one of the most reliable ways to steer Claude's output format, tone, and structure. A few well-crafted examples can dramatically improve accuracy and consistency. Include 3–5 examples for best results.

**What this means for marketing:**

If you have existing copy you love — an email that performed well, a headline that got clicks, a social post that resonated — paste it in. Claude will match the style and quality level far better than any adjective description can.

**Example:**
```
Here are 3 subject lines that performed well for us previously:
- "You're losing leads you don't know about"
- "The fix takes 10 minutes"
- "Most teams get this wrong"

Write 5 new subject lines for our upcoming webinar on marketing attribution, in the same style.
```

You'll get results that actually sound like your brand — not like a generic AI output.

---

## 4. Use XML tags when your prompt has multiple pieces

**What Anthropic says:** XML tags help Claude parse complex prompts unambiguously, especially when your prompt mixes instructions, context, examples, and variable inputs.

**What this means for marketing:**

When you're giving Claude a brief that includes background info, brand guidelines, existing copy, and instructions — separate them with tags. Otherwise Claude tries to figure out what's instruction and what's context, and sometimes gets it wrong.

**Do this:**
```
<brand_context>
[Company name] is a project management tool for marketing teams. Voice: direct, no fluff. Avoid: corporate jargon, excessive enthusiasm.
</brand_context>

<existing_copy>
Here is copy from our homepage that you should use as a tone reference:
[paste copy]
</existing_copy>

<task>
Rewrite the "Features" section of our pricing page using the same voice as the homepage copy above.
</task>
```

Especially useful when running the Brand Voice Checker, Campaign Brief Generator, or GEO Page Audit prompts in this library.

---

## 5. Give Claude a role at the start of every prompt

**What Anthropic says:** Setting a role focuses Claude's behavior and tone for your use case. Even a single sentence makes a difference.

**What this means for marketing:**

The role shapes how Claude approaches the entire task — what expertise it draws from, how it frames its answers, how critical it is of weak copy.

Notice that every prompt in this library starts with "You are a [role]." That line matters.

| Role | When to use it |
|------|---------------|
| `You are a performance marketing copywriter` | Ad copy, email, CTA optimization |
| `You are a GEO content strategist` | Any content for AI search visibility |
| `You are a senior brand strategist` | Brand voice, positioning, messaging |
| `You are a marketing director reviewing this work` | Getting critical feedback on existing copy |
| `You are a first-time visitor to this website` | UX copy review, landing page critique |

---

## 6. Tell Claude what format you want — positively

**What Anthropic says:** Tell Claude what TO do instead of what NOT to do. Match your prompt style to the desired output style.

**What this means for marketing:**

Negative instructions ("don't use bullet points," "no fluff") are less effective than positive ones. Describe the output you want, not the output you're trying to avoid.

**Don't do this:**
```
Don't make it too long. Don't use buzzwords. Don't be vague.
```

**Do this instead:**
```
Write in plain sentences. Maximum 3 paragraphs. Every sentence should earn its place — if it doesn't add new information, cut it.
```

Also: if you want a specific format (table, numbered list, headers, no headers), say so explicitly. Claude will adapt precisely.

---

## 7. Put your long content at the top, your question at the bottom

**What Anthropic says:** Place your long documents and inputs near the top of your prompt, above your query, instructions, and examples. Queries at the end can improve response quality by up to 30% in tests with complex, multi-document inputs.

**What this means for marketing:**

When you're running a GEO Page Audit, Brand Voice Checker, or Entity Strengthener — paste the content you want analyzed first, then ask the question.

**Structure to use:**
```
[Paste the full page content, campaign brief, or copy here]

---

Based on the content above, [your instruction here].
```

This is counterintuitive but it works. Claude processes better when it has all the context before the task, not after.

---

## 8. Specify length when it matters

**What Anthropic says:** Claude calibrates response length to how complex it judges the task to be. If your product depends on a specific length or verbosity, tune your prompts.

**What this means for marketing:**

Claude will give you as much as it thinks the task needs. Sometimes that's perfect. Sometimes you need to constrain it.

Add length instructions at the end of your prompt:

| Situation | What to add |
|-----------|------------|
| Email body | `Maximum 200 words.` |
| Social post | `Under 150 words, no hashtags yet.` |
| Executive summary | `3 bullet points maximum.` |
| First draft to iterate on | `Give me a rough first draft — I'll refine from here.` |
| Full exploration | `Be thorough — I'd rather have too much to cut than too little to work with.` |

---

## Quick reference: Before you run any prompt

Ask yourself:
- Did I tell Claude **who it is** (role)?
- Did I give it **enough context** about my brand, audience, and goal?
- Did I show it **an example** of what good looks like (if I have one)?
- Did I tell it **what format** I want the output in?
- Did I specify **how long** the response should be?

If yes to all five — your output will be significantly better than if you paste the prompt and hit enter without any customization.

---

*Sources: [Anthropic Prompt Engineering Documentation](https://platform.claude.com/docs/en/docs/build-with-claude/prompt-engineering/overview) — verified May 2026.*
