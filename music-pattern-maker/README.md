# Music Pattern Maker 🎹

A piano-roll playground where kids learn music **by ear**, not by drill —
clicking colorful cells to build melodies, then predicting what comes next
in scales they're starting to hear. Single HTML file, all sound synthesized
in-browser with the Web Audio API. No samples, no libraries, no backend.

## Ages

Roughly **6–11**. Younger kids stay in Sandbox and the starter Library;
older kids work through the scale + rhythm lessons.

## Run it

Open `index.html` in any browser — double-click works.

From a devserver:

```bash
cd ~/ai-parenting && python3 -m http.server 8765
# open http://<devserver-name>:8765/music-pattern-maker/
```

## Lesson types

Three lesson tracks, each built around **predict-then-reveal** (same pedagogy
as `ai-learner` next door — predict first, hear after):

1. **🔮 Predict-the-Next-Note** — app plays the first 4 notes of a scale
   (C major → A minor → C pentatonic, progressively). Kid clicks which row
   they think the 5th note is. App reveals + plays the answer. The predict
   step is the whole point: a correct guess means the *ear* heard the pattern.
2. **🎼 Scale Builder** — app names a scale ("C major"), lights up the root
   note, kid fills in the rest on the grid. Submit to check. Wrong cells
   pulse so the kid can self-correct by ear.
3. **🥁 Rhythm Clap-Back** — app plays a 4-beat pattern on a percussion
   sound; kid taps along on screen. App scores timing accuracy in ms and
   gives a star when the average gap is tight enough.

A lesson is marked **mastered** after the kid clears its check ≥2 times.
Progress (and stars) persist in `localStorage`.

## Sandbox + share-via-URL

After (or before) any lesson, **Sandbox mode** is a 16-step × 12-note piano
roll with 4 timbres (Piano / Marimba / Bell / Synth), adjustable tempo
(40–160 BPM), and a 5-melody starter Library (Twinkle Twinkle, Mary Had a
Little Lamb, Happy Birthday, Ode to Joy, plus a tiny original). Hit **Share**
and the grid base64-encodes itself into the URL hash — paste the link to a
parent or friend, they open it, the melody is already loaded.

## Design notes

- **Web Audio synth, no samples.** Every sound is `OscillatorNode` +
  `GainNode` with a short ADSR-ish envelope. Bell and Marimba use
  layered oscillators with detune; percussion uses noise bursts.
- **Predict-then-reveal is the through-line.** Lessons never just *tell*
  the kid what a scale is — they play it, ask the kid to guess, then reveal.
- **Celebratory of any sound.** Sandbox never grades; lesson feedback is
  always paired with the correct answer audibly played, so a wrong guess
  still ends with hearing the music.
- Mobile-responsive: grid cells are touch-friendly tap targets.
