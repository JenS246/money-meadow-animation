# Money Meadow Animation

A short, responsive homepage animation that invites viewers to see money as a physical object rather than only as transactional value.

The scene combines a macro-photographic cottage garden and hill of coins and bills with a frame-by-frame illustrated traveler. She appears in four short, fixed-location vignettes: discovering the money path, testing a large coin, tugging at a lifting bill, and pausing near the summit. She disappears between scenes, creating a gentle stop-motion rhythm instead of sliding mechanically across the landscape.

## How it works

- `index.html` contains the complete layout and CSS animation choreography.
- `garden-v4.png` is the generated photographic garden plate with distinct roses, peonies, hydrangeas, irises, tulips, lilies, alliums, snapdragons, coneflowers, and other cultivated flower families.
- `traveler-sprite-v3.png` contains twelve generated hand-painted character poses on transparency.
- A small dependency-free JavaScript timeline blends poses within four stationary scenes and fades the traveler out before each new location.
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

- Change `duration` near the end of `index.html` to adjust the full animation duration.
- Edit the `vignettes` array to change the traveler’s fixed locations, pose sequences, timing, rotation, or scale.
- Edit the coin, bill, and flower keyframes to change environmental responses.
- The scene contains no visible text; its meaning is communicated through movement.

## Asset note

The background and character sprite sheet are AI-generated original images. The animation choreography is original CSS work. The visual direction uses macro photography, hand-painted frames, and tactile miniature-world qualities without copying a named artist’s distinctive style.
