# Plinth

Turn an SVG logo into a styled 3D render. Pick a style (metal, glass, clay, wood, marble, plastic, neon, cartoon, retro, low poly), set the background, orbit to any angle, and export PNG, JPG, GLB or an animated video.

Everything runs in the browser. There is no build step and nothing to install: the whole app is `index.html`, which loads Three.js and fonts from a CDN.

## View it locally

Double-click `index.html`, or drag it into Chrome, Edge, Safari or Firefox. You need an internet connection for the CDN scripts.

## Host it on GitHub Pages

1. Create a new repository on GitHub (for example `plinth`).
2. Upload `index.html`, `README.md` and `.nojekyll` to the repository root.
3. Go to **Settings, then Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose the `main` branch and the `/ (root)` folder, then save.
5. After a minute, your site is live at `https://<your-username>.github.io/<repo-name>/`.

## Notes

- Input is SVG only. Strokes, live text and embedded images are skipped, so outline them in your design tool first.
- GLB export saves the shape and base materials. Glow, outlines and studio reflections don't carry over.
- Video export uses MP4 where the browser supports recording it, otherwise WebM.
- Three.js is pinned to r147 and loaded from jsDelivr.
