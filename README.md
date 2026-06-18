# Math Draws Graphics (MDG)

An interactive, single-file **math playground**: a gallery of animated math examples — each with a plain-language explanation of the maths *and* the live code that draws it.

**Live:** https://mattdanusergrant.github.io/mathdrawsgraphics/

- Single self-contained `index.html` — vanilla JS canvas, no build, no dependencies. Mouse + touch, responsive.
- **22 examples** across geometry, fractals, chaos, number theory and signals: perspective corridors, Sound Waves, Metatron's Cube, Conway's Game of Life, Phyllotaxis, the golden/Fibonacci spiral, Lissajous, the Lorenz attractor, the Hilbert curve, the Koch snowflake, the Ulam prime spiral, the Pythagoras tree, the Mandelbrot & Julia sets, the Barnsley fern, Collatz, the dragon curve, Fourier epicycles, and Sierpiński.
- Every example shows a **"How it works"** explanation plus its **editable source** — change the code and it redraws live (globals: `ctx, w, h, t, TAU`).
- **Animate**, **Trails**, a **Speed** slider, a **Random** button, and **PNG / SVG export** (vector sketches export to SVG; raster ones like Mandelbrot to PNG).
- Keys: `Space` replay · `R` random · `S` PNG · `V` SVG · `A` animate.

## Run locally

Open `index.html` in a browser — there are no fetch dependencies. Or serve it:

```bash
python3 -m http.server 8000
```

## Deploy

Pushing to `main` triggers the GitHub Actions workflow in `.github/workflows/deploy.yml`, which publishes this repo to GitHub Pages automatically.
