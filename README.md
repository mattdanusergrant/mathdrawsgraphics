# Math Draws Graphics (MDG)

A browser-based "coding art" studio for line animations and spirograph-style curves. Write live canvas sketches in **Code** mode, or shape spirographs and friends with visual controls.

**Live:** https://mattdanusergrant.github.io/mathdrawsgraphics/

- Single self-contained `index.html` — vanilla JS canvas, no build step, no dependencies. Mouse + touch, responsive.
- **Code** mode: a live JavaScript sketch editor (`ctx`, `w`, `h`, `t`, `TAU`) that recompiles as you type, seeded with a first-person door-corridor sketch and example buttons (Doors / Side Doors / Turning Hall / Swinging Doors).
- **Parametric** modes: Spirograph, Harmonograph, Rose, String Art — each a parametric line drawing sharing one render/animation/colour pipeline.
- Shared colour + motion controls (solid/gradient, neon glow, animate, trails), a **Surprise** randomiser, and **PNG + SVG export**.
- Keys: `Space` replay · `R` surprise · `S` PNG · `V` SVG · `A` toggle animate.

## Run locally

Just open `index.html` in a browser — there are no fetch dependencies. Or serve it:

```bash
python3 -m http.server 8000
```

## Deploy

Pushing to `main` triggers the GitHub Actions workflow in `.github/workflows/deploy.yml`, which publishes this repo to GitHub Pages automatically.
