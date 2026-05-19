# Letter Friends 🐻🦊🐧

A phonics + alphabet game for ages **3–5**. Every letter has a friendly animal
character, four picture words, and a silly alliterative sentence that's
freshly generated each time.

## Run it

Just open `index.html` in any browser. No build, no dependencies.

From a server, preview with:

```bash
cd ~/ai-parenting && python3 -m http.server 8765
# then open http://<host>:8765/letter-friends/ in a browser
```

Or copy `index.html` to a laptop and double-click.

## Learning goal

- **Letter recognition** — uppercase + lowercase shown together
- **Letter sounds (phonics)** — each tap speaks the name *and* the sound
  (e.g. "B says buh")
- **Word association** — 4 picture examples per letter, each tap-to-hear
- **Alliteration awareness** — silly sentences like "Bouncy Bear bakes
  buttery bagels!" make the shared-sound pattern hearable

## How to play

1. **Main grid** — 26 letter cards, each with its animal friend. Tap one.
2. **Letter screen** — the letter wiggles, the friend bounces, and the
   browser speaks the name + sound. Tap any picture word to hear it.
3. **Silly story button** — generates a fresh alliterative sentence each tap.
4. **Say it!** — replays the current sentence.
5. **Letter Hunt** (button top-right) — the app says a target letter; kid
   taps it on the grid. Wrong taps say the letter they hit, then re-ask.
6. **For Grown-Ups** — a dashboard showing per-letter visits and Hunt
   accuracy. Useful for spotting which letters need more practice.

## Parent tips

- Sit alongside for the first few letters and repeat the sound out loud.
- 3–5 minute sessions work best for this age — let your kid drive.
- Letter Hunt builds quick recognition; use it after they've explored a
  handful of letters freely.
- The silly sentences are a great way to introduce the word "alliteration"
  ("hear how they all start the same?").
- All progress is stored in your browser only (localStorage). Reset any
  time from the For Grown-Ups screen.

## Kid-friendly design

- Big tap targets, bright colors, rounded buttons with shadows
- Emoji characters — no images to load, works fully offline
- Web Speech API for narration with a graceful fallback (text is always
  visible, so the app works in browsers without speech support)
- No accounts, no network, no tracking
