# sharmi-website

A personal website project — a birthday surprise for Sharmila. 🎉

A single self-contained page that plays as a guided journey you drive with a
clicker: tap to unwrap the gift → the "Happy Birthday" hero → a fly-down to
"our place" → doors swing open → a party room of balloons and your hanging
photos (with a fireworks welcome) → a love letter → a bright cake you cut to
set off fireworks. Built for a projector — arrow keys / a presentation clicker
glide scene to scene, `F` goes fullscreen, `M` toggles music, and the fonts +
everything else are embedded so it works with no internet.

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
- **F** — toggle fullscreen · **M** — music on/off
- **T** — open the Tweaks panel (name, gift number, greeting, colors…)

In the party room, drop your photos onto the hanging frames (they save in the
browser via localStorage). In the finale, tap the cake to blow out the candles,
then drag the knife down to cut it — and tap anywhere for fireworks.

## Add your song

Open `index.html`, find `var SRC = '';` near the top of the script, and set it to
your audio — a filename like `'music.mp3'` next to this file, or a
`data:audio/mpeg;base64,…` URI to keep everything in one file. It fades in on the
gift unwrap; `M` mutes.

## Deploying

It's a static site, so any host works.

- **Vercel:** import this repo at vercel.com (framework preset "Other", no
  build step). Then add your custom domain under Settings → Domains and point
  your registrar's DNS at the records Vercel shows.
- **GitHub Pages:** enable Pages on the `main` branch in repo settings.
- **Netlify / Cloudflare Pages:** drag-and-drop the folder or connect the repo.
