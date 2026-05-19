# Animal Quiz Detective 🕵️

A friendly Detective tries to guess the animal your kid is thinking of by asking simple yes/no questions — a magical first peek at how AI uses branching logic.

## What it is
A single-file HTML game (no install, no build, no internet needed after first load). A cartoon Detective greets your kid, then asks 5-8 yes/no questions ("Does it live in water?", "Can it fly?", "Is it bigger than a grown-up?") and dramatically reveals its guess. Big tap targets, spoken narration, and emoji animals make it pre-reader friendly.

## Target age
**Ages 4-5** (also fun for 6-7). No reading required — every question is read aloud.

## Learning goals
- **Animal categorization** — fur vs. feathers, water vs. land, big vs. small.
- **Yes/no logic** — kids see how each answer narrows down possibilities.
- **Vocabulary** — ~35 animals with proper names and one fun fact each.
- **A first peek at AI** — kids experience how a "computer brain" can guess things by asking the right questions. Real AI uses millions of these tiny decisions.

## How to play
1. Open `index.html` in any modern browser (Chrome, Safari, Firefox, Edge).
2. Tap **Start Game**.
3. The Detective asks a yes/no question. Tap the big green **YES** or red **NO** button.
4. After a handful of questions, the Detective reveals its guess: *"Is it a… GIRAFFE?!"*
5. Tap 👍 if right or 👎 if wrong.
6. If wrong, your kid types or taps the real animal — the Detective learns about it.
7. A fun fact about the animal is shown and read aloud.
8. Play again!

### Extras
- **🔥 Streak counter** — correct guesses in a row.
- **📒 My Album** — every animal encountered earns a sticker (35 to collect).
- **👨‍👩‍👧 For Grown-Ups dashboard** — games played, Detective accuracy, best streak, and a list of animals that stumped the Detective.

## Parent tips
- **Play together the first few rounds.** Read the question aloud and let your kid press the button.
- **Ask "why" after each game.** *"How did the Detective know it was a dog?"* This is the AI lesson hiding in plain sight.
- **Stump the Detective on purpose.** Pick a rare animal and watch what happens — show your kid that the Detective only "knows" what it has been taught. (Real AI is the same!)
- **Use the album as a sticker book.** Try to fill it together over a week.
- **Talk about the "questions tree."** For older siblings, sketch a tiny decision tree on paper and let them invent their own.

## Run instructions
No build, no dependencies, no server needed:

```
open animal-quiz-detective/index.html
```

…or just double-click `index.html` in your file browser. Works fully offline. Progress is saved in your browser's localStorage (per-device).

## Tech notes
- Pure HTML/CSS/JS in one file.
- Web Speech API for narration with text-always-visible fallback (some browsers/devices may not have a voice installed — the game works either way).
- No tracking, no network calls, no API keys.
- Decision tree is a plain JS object — easy for parents to peek at, modify, or extend.
