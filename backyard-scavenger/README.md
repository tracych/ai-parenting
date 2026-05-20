# Backyard Scavenger 🔍

A pocket-sized excuse to get outside. Pick a season, get a fresh hunt card,
and snap a photo of every find. Designed for muddy hands and short attention
spans — ages **4 and up**.

## Run it

Just open `index.html` in any browser. No build, no dependencies.

From a server, preview with:

```bash
cd ~/ai-parenting && python3 -m http.server 8765
# then open http://<host>:8765/backyard-scavenger/ in a browser
```

Or copy `index.html` to a phone (or AirDrop it) and open it. Add to home
screen on iOS/Android for a one-tap app.

## How to play

1. **New Hunt** — pick a season (auto-set from today's date), pick Easy
   (10 items) or Adventure (20 items, includes a couple of rare finds), add
   players if you want. Hit **Start the hunt!**
2. **Hunt Card** — your list of finds, organized across Plants, Bugs, Sky,
   Textures, Sounds, Colors, Shapes, and Signs of Life.
3. Tap **?** on any item for a kid-friendly ID hint
   ("If the leaves are needle-shaped and clustered in pairs, you might have
   found a Pine!").
4. Tap **📷 Found it!** — opens your phone camera, snap the find, photo is
   saved to that item's slot.
5. When every item is found: confetti, total time, and your streak ticks up.

## Modes

- **Family team mode** — add 2+ players from setup. Each item gets an
  "assign to" dropdown — leave on *Anyone* or hand it to a specific kid.
- **Print mode** — tap **🖨️ Print** on the hunt card for a paper-friendly
  checklist with all hints visible. Perfect for road trips, classrooms, or
  unplugged afternoons.

## Why it works

- **Gets kids outside.** That's the whole point.
- **Season-aware.** The Spring hunt is different from the Fall hunt — buds
  vs. acorns, bees vs. crunchy leaves. Things they can actually find right
  now.
- **Photo + ID hint = a real learning moment.** Naming the thing, looking
  for it, recognizing it, and capturing it locks the concept in better than
  a flashcard ever will.
- **Streak counter** rewards the habit, not the number of items found.

## Design notes

- **No live AI, no internet calls.** All ID hints are curated by hand —
  ~60 items across plants, bugs, sky, textures, sounds, colors, shapes,
  and signs of life. Kid-readable, naturalist-friendly tone.
- **No GPS, no account, no tracking.** Region-agnostic items only (common
  things in most yards and parks).
- **Photos stay on the device** in localStorage — automatically downscaled
  so a full hunt fits comfortably. History keeps your last 20 hunts.
- Mobile-first layout, big tap targets, works one-handed while the other
  hand is holding a stick.
