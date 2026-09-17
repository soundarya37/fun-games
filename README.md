# Chroma Echo

A memory-sequence reflex game. Watch the pattern light up across four colored pads, then repeat it back — each round adds one more step to the sequence, and the pace gets faster as you go.

## How to play

1. Tap the center core to start.
2. Watch the sequence of pads light up (each has its own tone).
3. Repeat the sequence by tapping the pads in the same order.
4. Get it right and the round advances with one extra step added. Get it wrong and the run ends.

Your longest run is saved automatically in the browser, so it persists between sessions on the same device.

## Controls

- **Mouse / touch**: tap the pads directly.
- **Keyboard**: `1`/`q` (top-left), `2`/`w` (top-right), `3`/`a` (bottom-left), `4`/`s` (bottom-right). `Enter` or `Space` starts a new run.

## Running it

This is a single self-contained HTML file — no build step, no dependencies, no internet connection required.

- **Locally**: open `chroma-echo.html` in any modern browser.
- **Hosted**: the same file can be dropped into any static file host (GitHub Pages, Netlify, a plain web server, etc.) with no changes.

## Tech notes

- Pure HTML, CSS, and vanilla JavaScript — no frameworks or external assets.
- Sound is generated on the fly with the Web Audio API (a short sine tone per pad, a sawtooth tone on failure); no audio files are loaded.
- High score is stored via `localStorage` under the key `chroma-echo-best`.
- Respects `prefers-reduced-motion` and includes basic accessibility labels on the pads.
