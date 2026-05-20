# Coding Story Builder 📖

A block-based authoring tool where kids program their own playable choose-your-own-adventure story — then **export it as a standalone HTML file** they can email to a grandparent, share with a friend, or post on a class blog.

Programming as authoring. The kid is the writer *and* the engineer.

## What is it?

A Scratch-lite, drag-and-drop story engine. Kids snap together blocks — SCENE, CHOICE, IF, LOOP, VARIABLE, END — to build interactive fiction. A live preview pane plays the story as they build it, and a scene-graph view shows the branching shape of their world. When they're ready, one click downloads a self-contained `.html` file of their game.

## Age

- **Sweet spot:** 8–13
- 8–10 with a parent reading block labels and helping debug
- 11–13 can build deeply branching stories with variables solo

## Run it

Open `index.html` in any modern browser. No build, no install, no server, no internet.

```
open coding-story-builder/index.html
```

Works on desktop and tablet. Saves projects to browser `localStorage`.

## The building blocks

- **SCENE** — a title, body text, and an optional emoji "illustration"
- **CHOICE** — 2–4 buttons; each one leads to a different scene
- **IF / ELSE** — branch based on a variable (*"if has_key then Door else Locked"*)
- **LOOP** — repeat a sub-sequence N times (*"knock 3 times"*)
- **VARIABLE** — set, add to, or check a value (`gold`, `hp`, `has_sword`)
- **END** — an ending scene, with an optional "Achievement Unlocked" label

Blocks live in a palette on the left. Drag them into the script. Edit fields inline.

## Live preview + scene graph

- **▶ Preview** plays the kid's story in a panel beside the editor. Buttons work. Variables update in real time in the **variable inspector** (a tiny debugger so kids can see what their code is doing).
- **🕸 Scene Graph** opens a node-link diagram of every scene with arrows showing how choices connect them — kids can literally *see the shape of their story*.

## Templates + tutorial

Start from scratch, or remix one of three starter stories:

- 🌲 **The Magic Forest** — 3 scenes, 1 choice (gentle intro)
- 🐉 **Dragon's Cave** — 5 scenes, 2 choices, 1 variable (`has_sword`)
- 🤖 **Robot Pet** — 7 scenes, full branching with variables (`hunger`, `happy`)

**Tutorial mode** walks first-timers through building *The Magic Forest* step by step with hints.

## The export — the wow moment

Click **📤 Export Story** and the browser downloads a standalone `.html` file containing the kid's whole story. The grandparent double-clicks it; the game plays. No app, no login, no internet. **That file is the kid's first shipped piece of software.**

## Why it works

Most "kids coding" apps teach the *syntax* of programming and stop there. This one treats programming as the lever that makes the story possible. The kid isn't solving the teacher's puzzle — they're building their own world, and the IF block is the only way to make the locked door work.

The export is the win. Seeing your game open in another window, played by someone you love, is the moment a kid decides they're a maker.
