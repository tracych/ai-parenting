# Code Critters 🐣

A drag-and-drop block-coding puzzle game that teaches sequencing, loops, and basic conditionals — the building blocks of programming.

## What is it?

Kids guide a baby chick to its egg by dragging instruction blocks (Forward, Turn Left, Turn Right, Repeat, If Wall) into a "program strip," then pressing Play to watch the critter walk it. A friendly **Hint Owl** 🦉 gives Socratic nudges (not answers) when the kid is stuck.

## Age

- **Sweet spot:** 7–8 years old
- Fun for 5–6 with a parent reading the block labels
- Still engaging for 9+ as levels get into nested loops and conditionals

## Learning goal

- **Sequencing** — order matters; instructions run top to bottom
- **Loops** — recognize repeating patterns and use `Repeat 3×`
- **Conditionals** — decide "what if" with `If Wall → Turn Right`
- **Debugging mindset** — watch the critter, see what went wrong, try again

These are *pre-coding* skills aligned with how kids first encounter Scratch, Blockly, or Hour of Code.

## How to play

1. Open `index.html` in any modern web browser.
2. Press **Play** from the home screen, then pick a level.
3. **Drag blocks** from the Blocks panel into the program strip at the bottom.
4. **Drop blocks inside** the Repeat or If-Wall containers to nest them.
5. Press **▶ Play** to run the program. Press **👣 Step** to go one instruction at a time. Press **↺ Reset** to put the critter back.
6. **Drag a block to the trash** 🗑 to delete it.
7. Reach the egg 🥚 to win!

## The Hint Owl 🦉 (the "AI" part)

The Owl watches what the kid builds. After 30 seconds with no action OR 2 failed attempts on a level, it **glows**. Tap it to get a hint that's a *question*, not an *answer*:

- Missing forward steps? → "Count the squares to the goal."
- Walking into a wall? → "What should the critter do BEFORE that wall?"
- Same block 3 times in a row? → "There's a smarter way — could you use Repeat?"
- Conditional level? → "What if you don't know how many walls? Could the critter decide?"

The kid does the thinking; the Owl just nudges.

## Parent tips

Open **👪 For Grown-Ups** from the home screen to see:

- Which levels are completed
- How many hints were used
- Time on task per level

Use the dashboard to spot which concepts (sequencing vs. loops vs. conditionals) clicked easily and which need a chat over snacks.

A few things to try together:

- **Don't fix it for them.** Watching the critter bump is half the learning.
- **Ask "what does it do first?"** Reading a program out loud is a real skill.
- **Celebrate hint use.** Asking a smart question is what good engineers do.
- **Spot the pattern.** Around level 5, ask "do you see anything that repeats?"

## Run instructions

This is a single static HTML file — no build, no install, no server, no internet required.

```
open code-critters/index.html
```

Works on desktop, tablet, and phone. Drag-and-drop is implemented with pointer events so it works on touch screens too.

Progress is saved in your browser's `localStorage`.

## Levels

10 hand-tuned levels that ramp:

1. **First Steps** — straight line
2. **Around the Corner** — one turn
3. **Long L** — more squares
4. **Zig Zag** — multiple turns around walls
5. **The Long Road** — loops introduced
6. **Spiral Steps** — pattern-finding with loops
7. **Bumpy Hall** — go around an obstacle
8. **Wall Sense** — conditionals introduced
9. **Auto Pilot** — Repeat with If-Wall inside
10. **Critter Maze** — a real little maze
