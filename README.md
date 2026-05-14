# Math Quest 🦊

A fun math game for ~6-year-olds covering **+, −, ×, ÷** — designed to actually
verify whether kids *understand* the math, not just guess or memorize.

## Run it

Just open `index.html` in any browser. No build, no dependencies.

From the devserver, preview with:

```bash
cd ~/ai-parenting && python3 -m http.server 8765
# then open http://<devserver-name>:8765 in a browser
```

Or `scp index.html` to a laptop and double-click.

## How understanding is validated

Most math apps ask `3 + 2 = ?` and call it a day — a kid can guess or memorize
the answer without grasping addition. This game builds in three checks:

1. **Multi-representation requirement** — every fact (e.g. `3+2`) is asked in
   three formats: numeric (`3 + 2 = ?`), visual (count the apples), and word
   problem ("you had 3, got 2 more"). A fact is only marked **mastered** after
   the kid gets it right in **at least 2 of the 3 formats**. Memorizing one
   form isn't enough.

2. **Concept probes** — ~30% of the time after a correct numeric answer, the
   game flips to: *"Which picture shows 3 + 2?"* with 4 visuals to pick from.
   Catches kids who landed on the right number without understanding what
   addition actually does.

3. **Teach moments after wrong answers** — wrong answers always show the
   visual representation (counting objects, crossed-out items, groups) so the
   kid sees *why* the answer is what it is, instead of just "wrong, try again".

A **Parent Dashboard** (button: "For Grown-Ups") shows per-fact mastery with
a breakdown of which formats the child has demonstrated, so you can see what's
genuinely understood vs. lucky.

## Kid-friendly design

- Big tap targets, bright colors, friendly animal characters
- Audio feedback for right/wrong/star
- Number ranges scaled to age: + and − up to 10, × and ÷ only 1–5 with visuals
- ÷ is generated from × so answers are always whole numbers
- Progress saved in browser localStorage
