# Periodic Table Pets 🐶

A "gotta-catch-'em-all" periodic table for ages **7–12**. Every one of the 118
elements is a cartoon pet whose personality maps to its real chemistry.
Reactive alkali metals are excited puppies. Noble gases are aloof cats.
Halogens are grumpy lizards. Transition metals are sturdy bears.

## Run it

Just open `index.html` in any browser. No build, no dependencies.

From a server, preview with:

```bash
cd ~/ai-parenting && python3 -m http.server 8765
# then open http://<host>:8765/periodic-table-pets/ in a browser
```

Or copy `index.html` to a laptop and double-click.

## How to play

1. **Full periodic table** — 118 elements, color-coded by family, laid out
   correctly with the lanthanide and actinide rows tucked below.
2. **Tap any element** to open its pet card: a hand-drawn inline-SVG portrait,
   the element's archetype ("Super Excited Puppy", "Floaty Balloon Cat"), real
   properties (state, family, what it's used for), and one **Did-you-know**
   fact.
3. **Pokédex** — every pet you open gets caught (star badge + count in the
   header). Use the **Caught only** chip to see your collection.
4. **Filter chips** — Metals, Non-metals, Gases at room temp, Common 30, Caught
   only. Plus a free-text search by name, symbol, or atomic number.

## The Compound Babies mechanic

The fun part. Tap **🧪 Compound Babies** and pick any two pets.

- If they form a real compound from our curated bank of **35 famous ones**
  (NaCl, H₂O, CO₂, NH₃, CH₄, CaCO₃, Fe₂O₃, NaOH, HCl, H₂SO₄, NaHCO₃, CuSO₄,
  TiO₂, Al₂O₃, SiO₂, KNO₃, and more), the app shows the formula, a cute baby
  name ("Salty the Sea Sprinkle", "Fizzy the Bubble"), and what it is.
- If they don't, the app gently explains why: *"Noble gases don't make
  babies — they're too independent."* *"Two halogens both want to GRAB
  electrons — they argue more than they pair up."*
- Every match has a **🤔 Why?** button that explains the bond in
  age-appropriate terms: *"Sodium really wants to GIVE AWAY one electron,
  and Chlorine really wants ONE more. Perfect match!"*

You can also pick straight from the famous-compound bank to jump-start it.

## Why it works

- **Real chemistry drives the personality.** Reactivity isn't a sticker on a
  cute drawing — it *is* why the puppy is excited and the cat is aloof. Kids
  internalize family behavior by association.
- **Collectibles motivate exploration.** Pokédex counts make a kid want to
  open every cell, including the obscure rare-earths they'd otherwise skip.
- **Compound formation is the payoff.** Pairing two elements gives a tangible
  "did it work?" moment — and the *Why?* answer reuses the family vibe they
  already absorbed from the pet cards.

## Design notes

- Single self-contained HTML file. No CDN, no backend, no build step. All SVG
  portraits are inline; all data is in-file.
- Curated bank of **35 real compounds** (not generated). Each carries its own
  kid-readable chemistry explanation.
- The first ~30 most-common elements have hand-written archetypes and fun
  facts; the rest fall back to family-default templates with the element's
  symbol on a pet badge.
- 11 family-themed SVG motifs (dog, cat, lizard, bear, bee, rabbit, sloth,
  chameleon, unicorn, dragon, blob) — so even the unfamiliar elements still
  feel like distinct creatures.
- Pokédex persists in `localStorage`. Reset from the header.
- Mobile: table scrolls horizontally; pet cards open as a full-screen modal.
