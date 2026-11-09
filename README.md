# FareMap

A single-file, self-contained HTML demo of a flight-price-comparison map. Pick a departure city, add destinations, and compare mock fares on an infinitely-scrolling world map.

**[Live view](index.html)** — open `index.html` directly in a browser, or enable GitHub Pages on this repo (see below) to get a shareable link.

> This is a demo. Routes, prices, and airlines are illustrative mock data generated on the fly — not real fares.

## Features

- Infinite horizontally-scrolling world map (pans/wraps around the globe) with hand-drawn continent outlines
- Search-and-select departure and destination cities, or click a city dot directly on the map
- When no departure city is set, the first click on any city sets it as your departure
- Auto-fitting zoom that frames whichever routes are selected, plus manual zoom/pan controls
- Per-destination mock fare comparison (price, duration, stops, airline) with a focused drawer view
- Foldable date picker with a one-way / round-trip switch
- Light and dark theme toggle
- Zero build step and zero dependencies — it's one HTML file with inline CSS/JS

## Usage

Just open `index.html` in any modern browser. There's nothing to install or build.

```bash
git clone <this-repo-url>
cd faremap
open index.html   # or just double-click it, or use `python3 -m http.server` and visit localhost
```

## Deploying with GitHub Pages

1. Push this repo to GitHub (see below if you haven't yet).
2. In the repo on GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**.
3. Pick the `main` branch and `/ (root)` folder, then save.
4. GitHub will publish `index.html` at `https://<your-username>.github.io/<repo-name>/`.

## Project structure

```
.
├── index.html   # the entire app — markup, styles, and logic in one file
├── README.md
└── LICENSE
```

## Notes on the map art

There's no live network access baked into the page — the coastlines are simplified, hand-authored outlines (not a surveyed GIS dataset), so treat the geography as approximate/stylized rather than precise.

## License

MIT — see [LICENSE](LICENSE).
