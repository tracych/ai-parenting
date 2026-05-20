# Drawing Telephone 🎨📞

The classic party game "telephone" — but with sketches. One player types a silly
prompt, the next draws it, the next guesses what the drawing is, the next draws
*that*, and on it goes. At the end, the **Big Reveal** walks the family through
the whole chain step by step. That's where the laughing happens.

Designed for 3–8 players on a single shared phone, tablet, or laptop.

## Run it

Just open `index.html` in any browser. No build, no dependencies, no internet
needed.

```
open drawing-telephone/index.html
```

Or copy the file to a laptop and double-click.

## How to play

1. **Setup** — enter 3 to 8 player names. Pick how many turns each person gets
   (1–4; "2" is a sweet spot).
2. **First turn** — Player 1 types a wacky scene ("a wizard cat ordering tacos").
   Then taps "Hide and Pass."
3. **Pass the device** — a big handoff screen shows whose turn is next and what
   they'll be doing (draw, or guess). The previous content stays hidden until
   they tap "Ready."
4. **Drawing turns** — see the phrase, draw it on the canvas (6 colors, 3 brush
   sizes, eraser, undo), hide and pass.
5. **Guessing turns** — see only the drawing, type what you think it is, hide
   and pass.
6. **The Big Reveal** — when everyone's done, an animated slideshow walks
   through every step in order. Confetti at the start and finish.
7. **Save** the best chains to the Gallery — they live in this browser and you
   can replay them anytime.

## Why it's fun

- **The reveal is the payoff.** Half the joy is *waiting* for the reveal, then
  seeing how "a panda eating spaghetti" became "an octopus in a hammock" four
  turns later.
- **Drawings stay hidden.** Each player only sees the *previous* step — never
  the original prompt, never the chain. The mutations are pure.
- **Big tap targets, mobile-friendly canvas.** Touch and mouse both work; the
  drawing area resizes for phones.
- **No one is bad at it.** Stick figures, scribbles, and pure abstract art all
  produce great chains — sometimes the worst drawings make the best games.

## Design notes

- **Single file**, vanilla JS, no frameworks, no CDN, fully offline.
- Drawings are stored as PNG data URLs inside `localStorage` (gallery capped at
  20 chains to keep storage in check).
- The handoff screen between every turn is deliberate friction — it gives the
  current player time to actually pass the device before the next person sees
  anything.
- Family-friendly throughout: no chat, no accounts, no network, nothing leaves
  the device.
