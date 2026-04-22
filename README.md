# Tempus Presentation

A slideshow for **Dhruva's Work** — architectures, cloud processes, and deployments. React, Vite, Tailwind, Framer Motion.

## Run locally

```bash
npm install
npm run dev
```

Open [http://localhost:5176](http://localhost:5176). Use **← →** to change slides.

## Build

```bash
npm run build
```

Output: `dist/`.

## GitHub Pages

1. Repo **Settings → Pages → Source:** **GitHub Actions**.
2. Push to **`main`**. [.github/workflows/deploy-github-pages.yml](.github/workflows/deploy-github-pages.yml) builds with `VITE_BASE=/<repo>/` so assets load correctly.
3. Site: **`https://dhruva7102.github.io/tempus-presentation/`**

`public/.nojekyll` disables Jekyll processing on Pages.

## Vercel (optional)

Import this repo, build `npm run build`, output `dist`, leave `VITE_BASE` unset. [vercel.json](vercel.json) has SPA rewrites.

## Content

Edit `src/components/slides/` and register slides in `src/App.jsx`.
