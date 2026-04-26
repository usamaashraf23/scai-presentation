# SCAI Presentation

A single-file slide deck for SCAI Content AI. Built as a self-contained `index.html` — no build step, no framework, no node_modules.

## Files

- `index.html` — the entire presentation (HTML + CSS + JS, all inline)
- `scai-logo.svg` — standalone SCAI logo asset (the logo is also inlined in `index.html`, so this file is optional)
- `netlify.toml` — deployment config for Netlify (caching headers, security headers)

External resources loaded at runtime:
- Google Fonts (Inter, JetBrains Mono) via `fonts.googleapis.com`

## Deploy to Netlify

### Option 1 — Drag & drop (fastest)
1. Go to https://app.netlify.com/drop
2. Drag this folder onto the drop zone
3. Done — Netlify gives you a live URL

### Option 2 — Netlify CLI
```bash
npm install -g netlify-cli
netlify deploy --dir=. --prod
```

### Option 3 — Git-based deploy
1. Push this folder to a GitHub repo
2. In Netlify: New site -> Import from Git -> pick the repo
3. Build command: leave empty
4. Publish directory: `.` (root)

## Local preview

Just open `index.html` in any browser, or run a tiny static server:
```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Controls

- `Right Arrow` / `Space` — next slide
- `Left Arrow` — previous slide
- `Home` / `End` — first / last slide
