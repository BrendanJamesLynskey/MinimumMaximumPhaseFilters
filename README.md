# Minimum-Phase & Maximum-Phase Filters — An Interactive Guide

An animated, interactive visual guide to minimum-phase and maximum-phase digital filters. Built as a single self-contained HTML page with no dependencies, designed for GitHub Pages deployment.

[Guide](https://brendanjameslynskey.github.io/MinimumMaximumPhaseFilters/)

![Guide Preview](preview.png)

## What's Inside

The guide walks through the theory and intuition behind filter phase behaviour across five interactive sections:

1. **Why Phase Matters** — how two filters can share a magnitude response yet behave completely differently
2. **The Z-Plane** — drag a zero inside and outside the unit circle and watch the magnitude response, impulse response, and phase classification update in real time
3. **Minimum-Phase vs Maximum-Phase** — side-by-side comparison of impulse responses and unwrapped phase for a conjugate-reciprocal zero pair
4. **Allpass Decomposition** — demonstrates that any filter = minimum-phase × allpass, with a live z-plane showing the pole/zero mirror and a flat-magnitude proof
5. **Group Delay & Energy** — comparative group delay curves and cumulative energy bar charts showing how minimum-phase filters front-load energy

Every section includes animated sweep/flip buttons so you can sit back and watch the relationships unfold.


## Technical Details

- **Zero dependencies** — all graphics rendered with the Canvas API, no charting libraries
- **Single file** — `index.html` contains all HTML, CSS, and JavaScript
- **Responsive** — scales to mobile viewports with adapted controls
- **Accessible animations** — all animations are triggered by button press, nothing autoplays
- **~600 lines** of vanilla JS handling real-time DSP math (polynomial evaluation on the unit circle, phase unwrapping, group delay via finite differences, conjugate-reciprocal reflection)

## Topics Covered

| Concept | Where |
|---|---|
| Transfer function zeros & poles | Section 2 |
| Unit circle & frequency response | Section 2 |
| Conjugate-reciprocal zero reflection | Section 3 |
| Phase unwrapping | Sections 3, 4 |
| Allpass filters (pole/zero mirror) | Section 4 |
| Minimum-phase invertibility | Section 4 |
| Group delay | Section 5 |
| Cumulative energy distribution | Section 5 |

## Who It's For

Engineers, students, and anyone curious about digital signal processing who wants to build visual intuition for how zero placement shapes a filter's time-domain and frequency-domain behaviour.

## Licence

MIT
