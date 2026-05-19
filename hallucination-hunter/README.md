# Hallucination Hunter

A web-based AI literacy game where teens read AI-style passages and try to spot the planted hallucinations — fake citations, wrong dates, invented people, made-up quotes, and other patterns of confident-but-wrong AI output.

## What it is

A single-page HTML/JS app — no install, no backend, no API keys. Open `index.html` in any modern browser.

The teen picks a passage, reads it carefully, clicks on suspicious sentences (or selects a specific phrase first), tags each with the type of hallucination they think it is, rates their confidence, then submits to see the ground truth. Score breakdown teaches calibration: true positives (caught a real lie), false positives (flagged something true), and false negatives (missed a lie).

## Age

12–14 (best for middle schoolers; works fine for older teens who want quick practice too).

## Learning goal

Teach pattern recognition for the most common kinds of AI hallucination so the player learns to read AI output with healthy skepticism. By the end of a few rounds, the player should be able to:

- Spot **fake citations** (oddly specific journal names, made-up authors).
- Notice **wrong dates and numbers** (especially "exactly" before a too-round number).
- Recognize **invented people** (real-sounding names that don't match real roles).
- Catch **made-up quotes** (especially dramatic/profound ones attributed to historical figures).
- Be cautious of **plausible-but-unverifiable** claims (dramatic scene-setting, suspiciously specific stats).
- See how **hybrid/composite** claims wrongly mash together two real things.

The confidence slider + per-tag accuracy chart teach a higher-order lesson: how good are you at knowing when you're right vs. wrong?

## How to play

1. Open `hallucination-hunter/index.html` in a browser.
2. Pick a difficulty (Easy / Medium / Hard / All) and a passage.
3. Read it carefully.
4. **Click a sentence** to flag it as suspicious. Or **highlight a specific phrase** with your mouse, then click — only that phrase gets flagged.
5. Pick a hallucination tag from the picker. Adjust the confidence slider (1–5).
6. Repeat for as many suspicious parts as you want.
7. Click **Submit My Hunt** to reveal the ground truth.
8. Green underlines = the real facts (you should NOT have flagged these). Red = hallucinated. Yellow = plausible-but-unverifiable.
9. Check the per-passage feedback and your running per-tag accuracy. Try another passage.

## Parent tips

- **Play together the first time.** The "missed" explanations are mini-lessons; reading them aloud surfaces the reasoning.
- **Discuss false positives.** When your kid flags a real fact as fake, ask why it *felt* fake. That's the actual signal you want them building intuition around.
- **Talk about real-world stakes.** Fake citations in homework, made-up quotes in social media posts, invented "experts" cited in news articles — all real and growing.
- **Don't let them just guess.** The scoring penalizes flagging everything. Calibration is the point.
- **Revisit periodically.** Hard passages are subtle and re-reading the same one after a few weeks shows growth.

## Why hand-authored passages (and not live AI output)?

Live AI output is unpredictable. To teach a kid to spot specific hallucination patterns, we need **controlled ground truth** — meaning, we need to know exactly what is true and what is invented in each passage. So the passages here are written by hand, mimicking real AI failure modes, with every hallucination annotated and explained.

This also means:
- No API keys, no cost, no privacy concerns.
- The "lessons" are stable and reviewable.
- The kid doesn't accidentally learn a wrong "real" fact, because every made-up claim is clearly explained as fake in the reveal.

If a teen wants to graduate to spotting real AI hallucinations afterward, they can copy any AI chatbot's answer into a separate document, manually fact-check it, and apply the same patterns they practiced here.

## Run instructions

```
# Just open the file. No build step, no server.
open hallucination-hunter/index.html
# or
xdg-open hallucination-hunter/index.html
# or double-click in your file browser.
```

Works fully offline.

## A note on the content

All passages are hand-written for this app. Any "experts," "papers," and "journals" cited as fake within the passages are invented for teaching purposes and are not meant as accusations against real people or institutions. Real public figures (e.g., Marie Curie, Stephen Hawking, Tim Berners-Lee) are mentioned only with widely-known biographical facts; the hallucinated claims attached to them are clearly labeled in the ground truth reveal.
