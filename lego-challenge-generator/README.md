# Lego Challenge Generator 🧱

Endless open-ended build challenges for Lego, blocks, Magna-Tiles, or whatever
building toys you've already got. Spin the wheel, build the thing, snap a
photo. No instructions, no kits, just creativity.

## Run it

Just open `index.html` in any browser. No build, no dependencies. Works
offline. Designed for tablets — double-click on a laptop also works.

```bash
cd ~/ai-parenting && python3 -m http.server 8765
# then open http://<host>:8765/lego-challenge-generator/
```

## How to play

1. **Pick filters** (or don't!) — builder age, piece limit, category.
2. Tap the giant **SPIN!** button. The wheel spins with ticky-tick sounds.
3. A challenge card pops up with the prompt.
4. Build it! Then:
   - **🔄 Reroll** for a new prompt
   - **☆ Save** the ones you love (Faves tab keeps them)
   - **⏱️ Timer** for a focused 1/3/5/10/15-min build
   - **📸 Snap Build** to save a photo to your gallery
   - **⚔️ Family Battle** for sibling vs. sibling

## Modes

- **Solo spin** — kid spins, kid builds. Loop forever.
- **Timer mode** — countdown ring + ticks in the last 5 seconds + a triumphant
  chime when time's up. Great for kids who need a stop signal.
- **Family Battle** — 2–4 builders, same prompt, same clock. When time's up,
  everyone votes 👍 for everyone else's build. Winner gets crowned, but every
  build still rocks.
- **Photo gallery** — uses your device's camera (`<input capture>`) so phones
  and tablets open the camera directly. Photos compress + save to localStorage
  tagged with the challenge.

## Why it's fun

- **Uses what you already own.** No buying sets, no following instructions.
- **150+ prompts across 6 categories** — structural, creative, constrained,
  thematic, narrative, speed. The wheel never gets stale.
- **Kid-led.** No right answer. The prompt is a starting point; the kid
  decides everything else.
- **Sibling-friendly.** Battle mode turns "I'm bored" into a family event in
  30 seconds.
- **Encouragement, never judgment.** Every build wins something. Ties get a
  "everyone built something amazing!" banner.

All faves and photos live in your browser only (localStorage). Nothing is sent
anywhere. No accounts, no tracking.
