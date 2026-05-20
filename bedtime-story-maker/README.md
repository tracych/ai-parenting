# Bedtime Story Maker 🌙

A magical bedtime ritual for ages **4–9**. Your kid tells the app three
"ingredients" (a tiny dragon, a cozy sock, a swimming pool…), and the app
spins them into a 6-page illustrated bedtime story where *your kid is the
hero*. Every story ends the same way: safe, warm, tucked back in bed.

## Run it

Just open `index.html` in any browser. No build, no dependencies, no
internet, no API keys.

```
open bedtime-story-maker/index.html
```

Or copy the file to a laptop and double-click.

## How to use

1. Type your kid's **name** (the hero of tonight's story).
2. Fill the **3 ingredient slots** — anything from "a singing teapot" to
   "a marshmallow cloud." Tap suggestion chips if you're stuck. Blank slots
   get a friendly default.
3. Tap **Tuck me in & tell the story**.
4. Page through one short paragraph at a time with the ◀ ▶ buttons. The
   page softly flips. Tap 🔊 to have the page read aloud in a calm voice.
5. Love this one? Tap **💛 Save** to keep it in **My Storybook** for
   re-reading. Tap **🎲 New story** to re-roll with the same ingredients
   for a totally different tale.

## Why it's special

- **Your kid is the hero.** Their name appears in the story, in gold, on
  every page. They aren't watching — they're *in* it.
- **Built for the nightly ritual.** Calming dusk-blue palette, warm-lamp
  yellows, big serif body text, soft page-flip animation, and a read-aloud
  voice slowed to 0.85x. Nothing flashy, nothing jarring.
- **Every story ends safe.** The final beat *always* tucks the hero back
  into bed. No cliffhangers. No scary endings. Ever.
- **Re-readable.** Save the favourites to **My Storybook**. The next time
  the same kid asks for "the dragon-and-sock story," it's right there.

## Design notes

- **Template variation.** Six story-arc beats (Setup → Wish → Journey →
  Surprise → Resolution → Goodnight) each have 6–10 hand-written variants,
  combined with rotating curated banks of 15 dreamy locations, 12 sleepy
  side-characters, 9 sounds, and 10 smells. That's well over **200,000
  unique story combinations** before counting the ingredient substitutions
  — every night feels fresh, no API required.
- **No-scary rule.** Every beat in the bank is checked for tone: warm,
  gentle, curious, never scary, never sad. The Goodnight beat *always*
  returns the hero home safely to bed.
- **Offline read-aloud.** Uses the browser's built-in `SpeechSynthesis`
  API (no network), at a calm 0.85x rate, preferring softer female voices
  when the OS offers them. Text is always visible as a fallback.
- **Inline-SVG illustrations.** Each page paints a small dusk scene — sky
  gradient that deepens then warms across the story, a drifting moon,
  twinkling stars, and motifs drawn from your kid's ingredients (dragons,
  sock-shapes, pool waves, cookies, lanterns, mountains…). No external
  images, fully offline.
- **Storage.** Saved stories live in `localStorage` — nothing leaves the
  device, no accounts, no tracking.
