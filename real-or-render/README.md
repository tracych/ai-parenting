# Real or Render?

A media-literacy game for spotting AI-generated images.

## What it is

A single-page, offline-friendly game where players look at illustrative scenes and decide whether each is **Real** (a photo) or **AI-generated** (made by an image model). After each guess they see a "Detective Mode" overlay that circles the tells — the small mistakes AI image generators often make — and a 1-line explanation of each.

## Age

Designed for **10–11 year olds**, also engaging for 12–14. The visual style is intentionally more grown-up than the early-elementary tools in this repo.

## Learning goal

Critical media literacy:

- Notice that AI-generated images are getting really good — and that even adults get fooled.
- Learn a **taxonomy of tells**: hands, text, reflections, symmetry, backgrounds, logic.
- Build **calibration**: knowing what you don't know. The confidence slider trains kids to be confident when they should be and humble when they shouldn't.

## Important note on the images

This game uses **hand-drawn SVG mockups, not real photos**. Two reasons:

1. **Offline + safe.** The whole game is one HTML file with no network calls, no CDN, and no third-party image hosting. Nothing for a parent or school filter to worry about.
2. **Educational by design.** Each "AI" scene has deliberately authored tells in known categories (a six-fingered hand, a melted storefront sign, a mirror reflection that doesn't match, etc.). That lets us *circle the tell* and explain it, which a random photo from the internet wouldn't.

The point isn't to memorize these specific drawings — it's to learn the *categories* of mistakes so kids carry the skill back to real images they see in the wild.

## How to play

1. Open `index.html` in any modern browser.
2. Read the intro and press **Start**.
3. For each scene:
   - Look at the picture and caption.
   - Move the **confidence slider** (50–100%).
   - Press **Real** or **AI-generated**.
4. The reveal shows the correct answer plus Detective Mode overlay.
5. Your **score** rewards being confident *and* right, and penalizes being confident *and* wrong. Low-confidence guesses move your score very little — that's calibration.
6. Your **Field Guide** unlocks a new tell category each time you encounter one. At the end you can browse the full taxonomy.

## Parent / educator tips

- Play together. The most valuable moment is when your kid is *wrong but confident* — that's the lesson.
- After the game, try the "look for the tells" exercise on real images you scroll past together. Hands, text in signs, reflections, and jewelry symmetry are the easiest starting points.
- Talk about *why* this matters: people will try to fool them with fake images. Being able to slow down and check is a real-life skill.
- The game is short (≈10–15 scenes) on purpose. Replay it a few weeks later to see if their calibration improves.

## Run instructions

No install. No build. No server.

```
open index.html
```

or just double-click the file. Works fully offline.
