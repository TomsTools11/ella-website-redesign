# Ella Website Redesign

A self-contained, static single-page redesign. The entire site — markup, styles,
and JavaScript — is bundled into [`index.html`](./index.html); there is no build
step and no server-side code.

## Deploying to Vercel

This repo is configured for zero-config static hosting on Vercel:

- `index.html` at the repo root is served as the homepage.
- [`vercel.json`](./vercel.json) sets clean URLs and sensible caching/security headers.

### Connect the repo (recommended)

1. In the [Vercel dashboard](https://vercel.com/new), import this Git repository.
2. Framework Preset: **Other**. Leave the Build Command empty and the Output
   Directory as the repo root (the defaults work — there is nothing to build).
3. Deploy. Every push to the connected branch then triggers a new deployment.

### Or deploy from the CLI

```bash
npm i -g vercel
vercel        # preview deployment
vercel --prod # production deployment
```

## Local preview

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```
