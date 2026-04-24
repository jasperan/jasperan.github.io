# [jasperan.github.io](https://jasperan.github.io/)

Personal portfolio site for jasperan (AI Engineer, Oracle Developer Advocate). Static HTML served via GitHub Pages.

## Screenshots

![Hero](assets/screenshots/hero.png)

![About](assets/screenshots/about.png)

![Projects](assets/screenshots/projects.png)

![Speaking](assets/screenshots/speaking.png)

![Media](assets/screenshots/media.png)

![Contact](assets/screenshots/contact.png)

## Running Locally

```bash
git clone https://github.com/jasperan/jasperan.github.io.git
cd jasperan.github.io
python3 -m http.server 8000
# Open http://localhost:8000
```

No build step required. It's a static HTML site.

## Deployment

Pushes to `main` are served automatically by GitHub Pages at [jasperan.github.io](https://jasperan.github.io/).

## Structure

| Path | Purpose |
|------|---------|
| `index.html` | Original portfolio (dark/brutalist) — served at [`/`](https://jasperan.github.io/) |
| `v2/index.html` | Redesigned portfolio (editorial/cream) — served at [`/v2/`](https://jasperan.github.io/v2/) |
| `index-v2.html` | Intermediate redesign draft (kept for reference) |
| `assets/screenshots/` | Section screenshots used above |
| `index-original.html` | Earliest version, kept as archive |
| `dist/`, `docs/`, `old/` | Legacy build artifacts (inactive) |

Both `/` and `/v2/` deploy independently on GitHub Pages — the redesign lives side-by-side with the original rather than replacing it.
