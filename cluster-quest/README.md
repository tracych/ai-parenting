# Cluster Quest 🔮

A hands-on intro to **unsupervised clustering** for tweens. The kid plays the role of the k-means algorithm — picking how many groups they see, placing the starting centroids, and watching the algorithm finish the job.

## What it is

An interactive 2D plot of 30 cartoon creatures, each with 5 traits (size, fluffiness, spikiness, legs, loudness). The kid chooses two traits as the X and Y axes, picks `k`, drops centroids onto the plot, then iterates k-means step-by-step or auto-runs to convergence.

## Age

**9–11** (tween-friendly UI, but no jargon — every term is introduced visually).

## Learning goal

Build intuition for:

- **Unsupervised learning** — finding structure without being told the right answer.
- **k-means clustering** — the iterative "assign → re-center → repeat" loop.
- **Feature selection matters** — swap the axes and the same creatures form completely different groups. There is no single "right" clustering; it depends on what you measure.
- **Picking k** — too few clusters merge different things; too many split natural groups into noise.

## How to play

1. Open `index.html` in any modern browser. No install, no internet needed.
2. Look at the scatter of cartoon creatures. **How many groups do you see?**
3. Pick that number as `k` (1–5).
4. Press **📍 Place Centroids** — predict first, then click on the plot to drop each centroid wherever you think the middle of a group is.
5. Press **▶ Iterate** to advance one round at a time, or **⏩ Auto-Run** to watch.
6. Drag any centroid around at any time to see assignments update live.
7. Try the **mini-challenges** in the right panel.
8. **Swap an axis** (e.g. Y from Fluffiness to Spikiness) and re-run — same creatures, brand new clusters. That's the AHA moment.

## What kids learn about AI

- A computer doesn't "see" creatures — it sees **numbers**. Clustering is just geometry on those numbers.
- Algorithms don't always give one right answer — different starting points or different features lead to different clusters.
- AI loops: most ML is **predict → measure → update → repeat** until things stop changing. K-means is one of the simplest examples.
- Why **feature engineering** matters: choosing what to measure shapes what the model can discover.

## Parent / teacher tips

- The **"Predict first!"** modal is the most important part. Encourage the kid to commit to a guess before running the algorithm — this is how scientific intuition is built.
- After running with default axes (Size vs Fluffiness, k=3), ask: *"What if there's actually a 4th group hiding? How would we find it?"* Then swap axes.
- Try **k=1** and **k=5** to discuss under/over-clustering. K=1 is "everything is the same"; k=5 might split a real group in two.
- The **👪 Parent View** button shows challenges completed and prediction accuracy across sessions (saved to localStorage on this device only).
- Talk about real-world clustering: how streaming apps group similar songs, how schools sort students into reading levels, etc.

## Run instructions

Just open the file:

```
open cluster-quest/index.html      # macOS
xdg-open cluster-quest/index.html  # Linux
start cluster-quest/index.html     # Windows
```

Or drag it into any browser tab. Works offline. No accounts, no APIs, no data leaves the device.

## Tech notes

- Single `index.html` — inline CSS + JS, ~700 lines.
- Pure-JS k-means (Euclidean distance, reassign → recompute mean, ~40 lines).
- SVG plot with draggable centroids and clickable creature info.
- `localStorage` persists challenge progress and predictions.
- No build step, no dependencies, no network calls.
