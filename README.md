# ai-parenting

A collection of small web apps and experiments built to help with parenting —
mostly things that teach, entertain, or quietly check whether a kid is actually
learning vs. just clicking around.

## Projects

### 🦊 [math-quest](./math-quest/) — Math game for ~6-year-olds

A fun browser game covering **+, −, ×, ÷** across four themed worlds. Designed
to verify *conceptual understanding* — not just answer correctness — by asking
each fact in multiple formats (numeric, visual, word problem) and only marking
it "mastered" once the child has demonstrated it in at least two ways. Ships
with a parent dashboard showing per-fact mastery.

Open [`math-quest/index.html`](./math-quest/index.html). Details in
[math-quest/README.md](./math-quest/README.md).

### 🤖 [ai-learner](./ai-learner/) — How AI works, for kids ages 5–13

Three age tracks (🌱 Sprouts 5–7, 🔍 Explorers 8–10, 🔧 Builders 11–13), each
with hands-on lessons that teach the basics of AI: training from examples,
features, bias, weights, prompts, and hallucinations. Built around
**predict-then-reveal** interactions — the child predicts what the AI will do
*before* seeing it, so the parent dashboard can show whether they actually have
a working mental model of the system.

Open [`ai-learner/index.html`](./ai-learner/index.html). Details in
[ai-learner/README.md](./ai-learner/README.md).

---

## Shared design philosophy

All projects here follow the same principle: a kid clicking the right answer
isn't proof of understanding. Each app is designed so the activities themselves
generate evidence of comprehension — through multi-representation, prediction,
failure-mode reasoning, or application to new cases — and surfaces that
evidence in a parent dashboard.

Single-file HTML, no build, no dependencies. Just open in a browser.
