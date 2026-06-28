# Normal by Addition

An interactive demonstration of §4.1.1 from *Statistical Rethinking* (2nd ed.) by Richard McElreath.

A thousand people line up on the halfway line of a football pitch. Each flips a coin sixteen times — heads, step left; tails, step right — then stands still. Measure everyone’s distance from the halfway line and a bell curve appears, every single time. Nothing about the normal distribution is built into the coin; it emerges from the summing of many small independent nudges.

## Features

- **Animated walkers** — 1,000 people step across the pitch in real time, then drop into a histogram
- **Two step models** — coin ±1 (binomial) or uniform −1…1 (McElreath’s original R code)
- **Stacking runs** — the faint bars show the running average across all rounds dropped; stack 10, 20, or 50 rounds and watch the average press towards the red theoretical normal curve. Use **Stack ×10** to add ten rounds at once without animation
- **Live stats** — empirical mean, SD, predicted σ, and run count after each round

## Usage

Open `index.html` in any modern browser. No build step required. Assets (design tokens, signature figure) are loaded from the [Tunnel CDN](https://github.com/nihilisticiconoclast/cuddly-lamp).

## Design

Styled with the [Tunnel aesthetic](https://github.com/nihilisticiconoclast/cuddly-lamp) — a cartography × phase-space design system. The pitch contour lines are generated client-side with seeded value noise and the marching squares algorithm, giving each render the texture of an OS topographic map.
