# History Time Machine ⏳

A history app for kids that teaches the **single most under-taught history
skill: simultaneity across civilizations**. Most kids learn one civilization
at a time — Egypt one week, Rome another, China later — and never realize
they were all *happening at the same time*.

## Ages

Designed for ~8–13. Younger kids can use the easy difficulty; older kids
can be challenged by events only decades apart.

## Run it

Just open `index.html` in any browser. No build, no dependencies, no
internet needed.

From the devserver, preview with:

```bash
cd ~/ai-parenting && python3 -m http.server 8765
# then open http://<devserver-name>:8765/history-time-machine/ in a browser
```

Or `scp index.html` to a laptop and double-click.

## The three modes

1. **🔀 Sort it!** — The app scrambles 5–8 event cards from across
   civilizations (e.g. Confucius, the Maya inventing rubber, the Magna
   Carta, Apollo 11). Kid drags them into chronological order. Score =
   number correctly placed. Best score saved per device.

2. **🌍 Meanwhile, in…** — App shows one famous event (e.g. "Egyptians
   built the Great Pyramid"). Kid clicks three covered cards to reveal
   what was happening *at the same time* in other parts of the world.
   Pure exploration — no scoring, just wow moments. Bookmark the most
   surprising pairings to a "Mind-Blown" gallery.

3. **🎯 Year Explorer** — Kid types or scrolls to any year from 3000 BCE
   to 2025 CE. App shows a snapshot card per civilization with what was
   happening then. Try 1000 CE. Try 500 BCE. Try 1492.

## Why it matters

Standard history curricula teach civilizations **vertically** (Egypt's
whole 3,000-year arc, then Rome's, then China's) which buries the
**horizontal** reality: while Rome was building the Colosseum, the Maya
were already playing rubber-ball games, Tang China was printing books,
and the Kingdom of Aksum was minting coins. Kids who only ever see one
civilization at a time develop a quietly Euro-centric "main timeline +
side characters" mental model.

This app is built as deliberate anti-Eurocentrism: 13 civilization lanes,
all weighted equally — Maya math, African empires, Islamic Golden Age,
Indus Valley plumbing, Inca mountaintop cities — sit on the same timeline
as Greece, Rome, and Europe.

## What's inside

- **Curated event bank: 85 events** across 13 civilizations, each with
  year, civilization, kid-friendly description, and emoji
- Scrollable visual timeline with color-coded era bands
  (Stone / Bronze / Classical / Medieval / Renaissance / Industrial / Modern)
- Mobile-responsive — timeline scrolls horizontally on small screens

## All offline

Single HTML file. No tracking, no network calls, no accounts. Bookmarks
and best scores saved in browser localStorage.
