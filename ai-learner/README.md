# AI Learner 🤖

A kid-friendly intro to how AI works, tailored across three age groups, with
built-in checks for whether the child is *actually* understanding the concepts
(not just clicking through).

## Run it

Open `index.html` in any browser. No build, no dependencies.

From a devserver:

```bash
cd ~/ai-parenting && python3 -m http.server 8765
# open http://<devserver-name>:8765/ai-learner/
```

## Age tracks

Each track has 2 lessons, with concepts and interactions chosen for the age:

### 🌱 Sprouts (ages 5–7)
Concepts: AI learns from examples; AI looks at patterns it can see.
- **Teach the Robot** — sort fruits into RED / NOT RED, then watch Robot make
  predictions on new fruits. Robot trips up on a carrot (orange) → teaches
  that AI can't recognize what it's never seen.
- **Find the Pattern** — Robot sees 3 happy faces, then guesses on new ones.
  Trips on 😬 (teeth showing) → teaches that AI looks at *parts* of an image
  and can be fooled by surface similarity.

### 🔍 Explorers (ages 8–10)
Concepts: features, training data, bias.
- **Feature Detective** — toggle which clues (`has_wings`, `color`, etc.) the
  AI is allowed to use. Live accuracy bar updates. Then predict what AI says
  about a 🦇 bat using only `has_wings` (it'll wrongly say "bird") → teaches
  that good *features* matter.
- **Bias Lab** — pick a training dataset (red-only fruits vs. mixed). See AI
  fail on bananas/blueberries when trained one-sided. Predict what happens
  to face-recognition AI trained only on adults.

### 🔧 Builders (ages 11–13)
Concepts: weights, neural-net basics, prompts, hallucinations.
- **Tiny Brain** — three sliders for weights + threshold, classify
  cat/not-cat over 5 animals. Real-time accuracy. Must hit ≥80% to advance.
- **Prompt Lab + Hallucination Hunter** — tweak prompt modifiers (e.g. "for
  a 5-year-old", "as a poem", "like a scientist") and see canned LLM outputs
  change. Then spot the made-up fact in an AI summary about the Moon.

## How understanding is validated

Same philosophy as `math-quest` next door — beyond just "did they click the
right button":

1. **Predict-then-reveal** — the kid predicts what the AI will do *before*
   seeing the result. A correct prediction is the strongest evidence the
   child has built a working model of how the AI behaves.
2. **Failure-mode checks** — comprehension MCQs where the wrong choices are
   designed as plausible misconceptions ("Robot is broken", "AI hates
   bananas"). Choosing the right one means the child can rule out the bad
   mental models.
3. **Apply-to-new** — quizzes that extend the concept to a fresh scenario
   (bats with the bird-classifier, face-recognition with adult-only training
   data) so the child can't pass by pattern-matching the lesson.
4. **Parent dashboard** — per-lesson breakdown of prediction accuracy and
   comprehension-check accuracy. A lesson is marked **mastered** only when
   both are ≥70%.

## Design notes

- Single-file HTML, ~60KB, no dependencies.
- Progress and stars persist in `localStorage`.
- Big tap targets, audio feedback, animal buddy picker.
- All "AI" behavior is simulated by simple rules in JS (a real LLM would be
  overkill — and unsafe — for kids). The simulations are designed to make
  the *concept* visible, not to be realistic at scale.
