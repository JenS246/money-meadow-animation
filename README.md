# Money Meadow Animation

A short, responsive homepage animation that invites viewers to see money as a physical object rather than only as transactional value.

The scene combines a macro-photographic cottage garden and hill of coins and bills with a frame-by-frame illustrated traveler. She climbs, braces against a large coin, slips, recovers, tugs at a lifting bill, and continues uphill while flowers and loose paper move softly in the wind.

## How it works

- `index.html` contains the complete layout and CSS animation choreography.
- `garden-v2.png` is the generated photographic garden plate.
- `traveler-sprite-v2.png` contains twelve generated hand-painted character poses on transparency.
- The animation uses no JavaScript and has no runtime dependencies.
- A `prefers-reduced-motion` mode presents a still composition.
- `.github/workflows/pages.yml` publishes the site to GitHub Pages.

## Run locally

Open `index.html` directly in a modern browser, or run a small local server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Publishing

Push to the `main` branch. The included GitHub Actions workflow deploys the repository to GitHub Pages.

Public site: `https://jens246.github.io/money-meadow-animation/`

Source repository: `https://github.com/JenS246/money-meadow-animation`

Hosting: GitHub Pages. Backend services: none.

In the repository settings, **Pages → Build and deployment → Source** should be set to **GitHub Actions**.

## Customization

- Change `--loop` in `index.html` to adjust the full animation duration.
- Edit the `journey` keyframes to change the traveler’s route.
- Edit the performance, coin, bill, and flower keyframes to change individual movements.
- The scene contains no visible text; its meaning is communicated through movement.

## Asset note

The background and character sprite sheet are AI-generated original images. The animation choreography is original CSS work. The visual direction uses macro photography, hand-painted frames, and tactile miniature-world qualities without copying a named artist’s distinctive style.
