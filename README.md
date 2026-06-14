# sharmi-website

A personal website project — a birthday surprise for Sharmila. 🎉

A single self-contained page: a gift you tap to unwrap, an animated "Happy
Birthday" hero, a 3D photo gallery (drag your own photos in), a love letter,
and a make-a-wish candle you blow out with your mic. Built for a projector —
arrow keys / a presentation clicker glide scene to scene, `F` goes fullscreen,
and the fonts are embedded so it works with no internet.

## Contents

- `index.html` — the entire site (HTML + CSS + JS + fonts, no dependencies).

## Running locally

Just open `index.html` in a browser. Or serve the folder:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Keyboard / presentation controls

- **→ / Space / clicker** — next scene (first press unwraps the gift)
- **← / ↑** — previous scene
- **F** — toggle fullscreen
- **T** — open the Tweaks panel (name, gift number, gallery effect, colors…)

Drop photos onto any gold frame; they save in the browser (localStorage).

## Deploying

It's a static site, so any host works.

- **Vercel:** import this repo at vercel.com (framework preset "Other", no
  build step). Then add your custom domain under Settings → Domains and point
  your registrar's DNS at the records Vercel shows.
- **GitHub Pages:** enable Pages on the `main` branch in repo settings.
- **Netlify / Cloudflare Pages:** drag-and-drop the folder or connect the repo.
