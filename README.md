# Comeback Blueprint v0.1.0

A validated, mobile-first PWA for the fixed Weeks 0–12 comeback calisthenics program.

## Run locally

```bash
npm test
npm run serve
```

Then open `http://localhost:8080`.

## Deploy to GitHub Pages

Upload the contents of this folder to the repository root and enable Pages from the main branch. The included `.nojekyll`, manifest, and service worker support static hosting.

## Source of truth

- `docs/specification.md`
- `data/program.json`
- `data/exercises.json`
- `data/progression.json`

The current production UI is the validated single-file application in `index.html`. The structured data files and tests establish the maintainable v0.1.0 baseline for the next refactor.
