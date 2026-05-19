# Fraction Forge 🔨

A blacksmith-themed fractions playground. Kids forge target fractions by tapping fraction tiles onto an anvil, then watch the sum simplify in real time. An "AI Hint Bot" classifies the type of mistake the kid keeps making and serves a targeted micro-lesson instead of a generic "try again."

## What it is
A single-file HTML app. No build, no server, no accounts. Drop the file on any device with a browser.

## Age range
- **Target:** 9-10 (4th-5th grade)
- **Also works for:** 8-11 (motivated 3rd graders through middle school review)

## Learning goals
- **Equivalent fractions** (3/4 = 6/8 = 9/12)
- **Adding/subtracting fractions** with unlike denominators (1/2 + 1/3 = 5/6)
- **Fraction-to-decimal conversion** (live readout while building)
- **Comparing fractions** with different denominators (3/5 vs 5/8)
- **Estimation** (will 2/3 + 1/4 be more or less than 1?)

## How to play

Four game modes — pick from the menu:

1. **🎯 Forge a Target.** A target like 5/6 appears. Tap fraction tiles (1/2, 1/3, 1/4, 1/6, 1/8, 1/12) to drop them on the anvil. The live readout shows the running sum, simplified, with a decimal and a progress bar pointing at the target. Hit "Check forge" when you're ready.

2. **⚖️ Find Equivalents.** Given 3/4, tap the option that's equal (e.g. 6/8 or 9/12). Distractors include the flipped fraction (4/3), the "added 1 to top and bottom" trap (4/5), and scaled-only-numerator (6/4).

3. **🔮 Predict & Reveal.** "Will 2/3 + 1/4 be MORE or LESS than 1?" Kid picks first — the prediction is stored before they forge. Then they build the sum on the anvil and reveal the answer. Builds estimation intuition.

4. **📏 Which is Bigger?** Compare two tricky fractions (different denominators). Decimal values are revealed after picking so the kid can self-check.

## The AI Hint Bot

The app tracks every wrong answer and classifies it into one of four error categories:

- **Added num + den together** (1/2 + 1/3 = 2/5) — the classic "I added both tops and both bottoms" mistake
- **Wrong common denominator** — used a denominator that isn't actually a common multiple
- **Flipped numerator/denominator** — picked 4/3 when looking for 3/4
- **Compare-with-bigger-denominator** — picked 1/8 over 1/4 because "8 is bigger"

If the kid makes the same kind of mistake **2 or 3 times in a row**, Hint Bot pops up with a targeted SVG mini-lesson about THAT specific misconception — not a generic hint.

## Parent dashboard

From the main menu, tap **👨‍👩‍👧 Parent Dashboard** to see:
- Mastery percentage per skill (forge, equivalents, predict, compare)
- A bar chart of which error categories show up most often
- A log of the last 5 predict-then-reveal attempts (prediction vs. actual)

All progress saves to `localStorage` in the browser. Use the "Reset progress" button to clear.

## Parent tips

- **Don't rush past the predict mode.** Estimation is a separate skill from computation — many kids can compute 2/3 + 1/4 but can't tell you if it's near 1 or near 2. Predict mode builds that intuition.
- **The "added top + bottom" mistake is the #1 fraction error.** If Hint Bot keeps surfacing it, that's worth a 5-minute conversation: a fraction's *bottom* tells you the SIZE of each slice, not a count of slices. Adding two halves doesn't make the slices smaller.
- **Equivalent fractions click via the tile visual.** When 3/4 of the bar is colored and 6/8 of a 2×-tile-count bar covers exactly the same length, the equivalence becomes *visual*, not memorized.
- **Don't pre-explain.** Let the kid make a wrong move first; the in-context "your sum is 7/8, target was 5/6" feedback is more powerful than a lecture.
- **Use the dashboard once a week.** If one error category dominates after ~30 attempts, that's the skill to revisit (with worksheets, manipulatives, or just a chat).

## Run instructions

```
# Local
open fraction-forge/index.html   # macOS
# or just double-click the file in your file browser

# Or serve it
cd fraction-forge && python3 -m http.server 8000
# then visit http://localhost:8000
```

Works offline. Works on phones (tap-to-place tiles), tablets, and computers. No installation, no signup, no data leaves the device.
