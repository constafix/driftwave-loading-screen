# Driftwave Loading Screen

An animated ocean loading screen — a ship riding sinusoidal waves through a 16-second day/night cycle. No frameworks, no build step. One HTML file.

![preview](https://raw.githubusercontent.com/constafix/driftwave-loading-screen/master/preview.png)

## Demo

Open `driftwave.html` in any modern browser.

## What's inside

- **Wave physics** — cubic Bézier SVG path, phase-shifted each frame via GSAP. Binary search on `getPointAtLength()` finds the exact Y position and tangent angle at the ship's contact point.
- **Ship rotation** — follows the wave tangent with 0.92 damping for a natural feel.
- **Day / night cycle** — pure CSS keyframe animations: sky gradients, sun arc, moon arc, stars, glow layers — all on a 16-second loop.
- **Drifting scenery** — city skyline, island with palm tree, lighthouse scroll past in the background.
- **Loading phrases** — 35 nautical one-liners, cycling with GSAP fade transitions.
- **Reduced motion** — respects `prefers-reduced-motion: reduce`, skips GSAP animation entirely.

## Stack

- [GSAP 3](https://gsap.com/) via CDN — wave tween + phrase transitions
- Vanilla JS + SVG + CSS — everything else

## Structure

```
driftwave.html   — the entire project
```
