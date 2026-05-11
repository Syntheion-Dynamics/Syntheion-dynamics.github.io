# Syntheion-dynamics.github.io

Astro-based portfolio for Syntheion Dynamics.

## Stack

- Astro (static output)
- Plain CSS with design tokens and mode-based accent layers
- Self-hosted fonts: Inter + JetBrains Mono
- GitHub Actions deploy to GitHub Pages

## Requirements

- **Node.js 22.12+** (Astro 6 refuses older versions; use `nvm`, `fnm`, or the installer from nodejs.org.)

## Local Development

```bash
npm install
npm run dev
```

Open `http://localhost:4321`.

## Build

```bash
npm run build
npm run preview
```

## Project Structure

```text
.
├── public/
│   └── images/                  # normalized project assets
├── src/
│   ├── components/              # reusable UI blocks
│   ├── layouts/                 # page shell + meta tags
│   ├── pages/                   # Astro routes
│   └── styles/                  # global tokens + mode overrides
├── .github/workflows/deploy.yml # GitHub Pages deployment
├── astro.config.mjs
└── package.json
```

## Routes (v1)

- `/` landing
- `/gooblerator`
- `/engine`
- `/planner`
- `/astrum-invictum`
- `/photography`
- `/about`
- `/404`

## Deployment

Push to `main` triggers `.github/workflows/deploy.yml`.

GitHub repository settings required:

1. Go to **Settings -> Pages**
2. Set **Source** to **GitHub Actions**
3. Keep branch workflow-driven (no manual `gh-pages` publishing needed)
