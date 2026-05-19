# Prompt Forge

A browser-based game that teaches teens (ages 12-14) how to write better prompts for AI models.

## What is it?

Prompt Forge gives you a series of challenges where you have to coax a "mock AI" into producing
exactly the right output — a 4-line haiku, a JSON list, a polite email, a markdown table, and so on.
You see the target spec, write your prompt, and the mock model returns a response that is graded
against a rubric. If your prompt is missing a rule (like "no rhymes" or "in exactly 2 sentences"),
the model will skip that constraint on purpose, so you learn to be specific.

- **Age:** 12-14
- **Learning goal:** Prompt engineering — specificity, role assignment, constraints, formatting, examples, structured output, conciseness.
- **No backend, no signup, no tracking.** One HTML file. Open it and play.

## How to play

1. Open `index.html` in any modern browser (Chrome, Firefox, Safari, Edge).
2. Pick a challenge from the left panel.
3. Read the target spec at the top.
4. Type your prompt in the prompt box. Click **Run Mock Model**.
5. The mock model's output appears. Below it, every rubric check turns green (✓) or red (✗).
6. If you didn't get 100%, read the tip and refine your prompt.
7. Get all rubric checks green for **2 stars**. Keep it concise (under 35 words) for **3 stars**.
8. Your attempts are saved per-challenge so you can see your progression.

## The mock model

The mock model is a deterministic JavaScript function. It is **not** a real AI — it scans your
prompt for keywords and constraints (like "haiku", "JSON", "no exclamation points", "for a 6-year-old")
and produces a response that respects only the constraints you actually mentioned. This makes the
feedback predictable and educational: you can see *exactly* which words in your prompt unlocked
which behavior.

## Optional: try with a real model (BYO key)

If you have an Anthropic API key, you can paste it under the **"Advanced: use real model"** panel
to see the same prompt run against a real Claude model side-by-side with the mock model.

- The key is stored only in your browser's `localStorage`.
- It is sent **only** to `https://api.anthropic.com` — never to anywhere else.
- A **Clear key** button removes it from your browser at any time.
- **Prompt Forge works fully without a key** — the BYO-key feature is optional.

### Safety note — keys are passwords

An API key is like a password. **Never share your key** with friends, classmates, or anyone online.
Anyone with your key can make API calls billed to your account. Parents should help younger teens
decide whether to enable this feature.

## Parent tips

- Play the first 3-4 challenges together. Talk about *why* a specific word in the prompt produced
  a different output. This is the core lesson of prompt engineering.
- After your teen earns 3 stars on a challenge, ask: "Could you say the same thing in even fewer
  words?" Conciseness is a real skill.
- Challenge #12 introduces *few-shot prompting* (showing examples). This is a real, widely-used
  technique in AI applications — call it out as a "pro move".
- Discuss why a real AI might not always follow instructions perfectly (it's probabilistic, the
  mock model is deterministic). The mock model is a simplified teaching tool.
- If you enable the BYO-key feature, supervise the first run and discuss what kinds of prompts
  are appropriate to send.

## Run instructions

No build step. No install. Just open the file:

```
open prompt-forge/index.html
```

or double-click it in your file browser. It runs entirely client-side.

## What's inside

- `index.html` — single file: HTML, inline CSS, inline JavaScript. No external dependencies.
- `README.md` — this file.
