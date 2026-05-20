# Joke Lab 😂

A silly little workshop where a kid and a grown-up invent jokes together, score them with a deterministic "AI rater," and grow a family joke book worth reading at dinner.

## What it is

Five joke shapes (Knock-knock, What-do-you-call, Riddle, Pun, Why-did), a topic picker (animals, food, school, sports, weather, family), a bank of 200+ seed jokes, and a tiny rater that hands out 1–5 stars with a one-line note. Saved jokes pile up into a Family Joke Book you can flip through or perform in big-text "Present" mode at the table.

## Run it

No build, no internet, no dependencies. Single file.

```
open joke-lab/index.html
```

Or just double-click the file.

## How to play (the collaborative invention loop)

1. Pick a **category** (Knock-knock, Pun, etc.) and a **topic** (animals, food, school…).
2. The Lab deals you **3–5 seed jokes** drawn from a curated bank — they're already pretty funny, but they're starting points.
3. Pick one. The setup and punchline drop into editable textareas. Kid edits, parent suggests, both giggle.
4. Tap **Rate this joke**. The AI rater gives 1–5 stars and one line of feedback.
5. Tap **Save to Joke Book** when you've got a keeper. Try again with a different seed.

## The rater (deterministic, not magic)

There is no API, no model, no network. The rater is pure JavaScript pattern-matching on three signals:

- **Surprise** — does the punchline introduce words the setup didn't? More twist, more stars.
- **Punch** — is the punchline short? Brevity is the soul of funny.
- **Length-fit** — is the setup ~1.5–4× the punchline? Classic joke shape.

It then composes a friendly one-liner like *"Great twist! Try trimming the punchline by a word or two."* Same joke text always gets the same score, so kids can iterate and watch the stars go up.

## Family Joke Book + Present mode

- **Joke Book** — every saved joke, paginated like a real comic-book joke collection, tagged with date, author ("Kid" / "Parent" / "Together"), category, and rating. Print-friendly stylesheet — print it, staple it, gift it to grandma.
- **Present mode** — fullscreen single joke, huge type, *"tap to reveal punchline"* button. Made for the dinner-table delivery.
- **Joke of the Day** — landing-page widget pulls a curated classic from a built-in bank of ~50 kid-safe groaners. Inspiration, not pressure.

Everything lives in your browser's localStorage. Nothing leaves the device.

## Why it's fun

Humor is a real literacy — noticing the rules of language so you can break them. A kid who writes a pun has practiced word-sense, syllable-play, and audience-awareness in one move. And because the joke book *grows*, the artifact gets better than any single joke: it becomes a record of a family figuring out what makes each other laugh.

Groan-worthy puns enthusiastically encouraged.
