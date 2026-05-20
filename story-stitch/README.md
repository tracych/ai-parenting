# Story Stitch ✍️

A round-robin story your family writes together — one sentence at a time — and
keeps as a printable storybook page.

## What it is

Pass the laptop (or tablet) around the table. 2–6 players take turns adding
1–3 sentences to a shared story. When someone gets stuck, an **Idea Spark**
panel offers gentle, curated nudges. When the story feels finished, it's
rendered as an illustrated storybook page you can print and stick on the fridge.

No accounts. No internet. No "AI generates your story for you." The story is
*yours* — Story Stitch just hands you the next pen.

## Run it

Just open `index.html` in any modern browser. No build, no dependencies,
nothing sent anywhere.

Or from a server:

```bash
cd ~/ai-parenting && python3 -m http.server 8765
# then open http://<host>:8765/story-stitch/ in a browser
```

## How to play

1. **Setup** — type in 2–6 player names and pick a **genre**:
   Mystery 🔍 · Adventure 🗺️ · Silly 🤪 · Gentle Scary 🕯️ · Sci-Fi 🚀 · Fairy Tale 🏰.
2. **Round-robin** — Player 1 sets the scene with 1–3 sentences, taps
   **Add to story →**, and the turn passes. Player 2 reads the story so far,
   then adds their bit. And so on.
3. The avatar in the corner of each turn says who's up.
4. **End story** when it feels finished (the app gently asks "are you sure?"
   if it's still very short).
5. Read the **final reveal** — your story becomes a real-looking storybook
   page, with an auto-generated title, a genre badge, and tiny initials in
   the margin showing who wrote what.
6. **Print** it, or **save to library** to re-read later.

## Idea Spark + Twist mechanics

- **Idea Spark sidebar** has 12 collapsible categories — *Introduce a stranger,
  Reveal a secret, Describe the setting, Add a problem, Skip ahead in time,
  Bring back something from before, Add a sound or smell, Let someone speak,
  Force a choice...* Each has 10+ curated prompts. Tap a category to reveal one;
  tap "↻ another one" to reroll. Totally optional — kids who are flowing don't
  need it.
- **🌀 Throw in a twist** button pulls from a bank of 50+ plot-twist nudges
  ("suddenly it starts raining frogs", "their reflection waves first", "a door
  appears in a wall that used to be solid"). Cycles deterministically so you
  don't get the same one twice in a row.

## The printable storybook

The final page is designed to look like an actual page from a children's book:
italic title, a drop cap, indented paragraphs, small SVG flourishes between
paragraphs, players' initials in tiny margin text, and a "·· THE END ··"
flourish. It prints clean (no UI chrome, just the page) on standard letter or
A4 paper.

## Library

Every saved story stays in your browser's localStorage, named by genre and
date. Open it anytime, re-read it, or re-print it. Nothing leaves the device.

## Why it's special

Most "AI storytelling" tools generate a story *for* you. This one does the
opposite — it gets out of the way, gives everyone a turn, and quietly offers
help only when someone asks. The result is a story your family actually wrote
together, and because it prints as a real page, it becomes a small artifact
you can keep — a snapshot of how your six-year-old ended a chapter, how the
story nobody planned ended exactly where it needed to.

Treat every contribution as gold. That's the whole game.
