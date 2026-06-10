# CLAUDE.md

Personal portfolio site for jasperan. Static HTML served via GitHub Pages. No build step.

## Tech Stack

- Plain HTML + Tailwind CSS (CDN)
- GitHub Pages (hosting, auto-deploys from `main`)
- No static site generator, no package manager, no build pipeline

## Run Locally

```bash
python3 -m http.server 8000
# Open http://localhost:8000
```

## Deploy

Push to `main`. GitHub Pages picks it up automatically at [jasperan.github.io](https://jasperan.github.io/).

## Structure

| Path | Purpose |
|------|---------|
| `index.html` | Main portfolio page (self-contained), served at `/` |
| `v1/index.html` | Archived brutalist version, served at `/v1/` |
| `index-v2.html` | Intermediate redesign draft, kept for reference |
| `index-original.html` | Earliest version, kept as archive |
| `assets/screenshots/` | Portfolio section screenshots |
| `old/` | Archived legacy Mobirise output |
