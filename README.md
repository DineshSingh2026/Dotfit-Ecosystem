# FIT Ecosystem — View Website

Static, view-only landing page for the FIT ecosystem (BodyBank, FitChef, Beyond The Body). No forms, no user data, no database.

## Run locally

- **Option 1:** Open `index.html` in a browser (some features may need a local server for correct paths).
- **Option 2:** Serve the folder with any static server, e.g.:
  - `npx serve .`
  - `python -m http.server 8080` (then open http://localhost:8080)

## Assets

- Place logo images in `assets/logos/`: `bodybank.png`, `fitchef.png`, `btb.png`.
- Place hero background in `assets/`: `hero-bg.png`.

## Deploy

Upload the project folder to any static host (GitHub Pages, Netlify, Vercel, etc.) or point the host’s root to this directory.

### Deploy on Render

This repo must be deployed as a **Static Site**, not a Web Service or Docker app (there is no Dockerfile).

1. In [Render Dashboard](https://dashboard.render.com), click **New +** → **Static Site**.
2. Connect the repo: `DineshSingh2026/Dotfit-Ecosystem`, branch `master`.
3. **Build command:** `echo 'No build step'` (or leave empty).
4. **Publish directory:** `.` (repo root).
5. Click **Create Static Site**.

If you previously created a **Web Service** (Docker) by mistake, delete it and create a **Static Site** as above. The repo includes a `render.yaml` blueprint so Render can use these settings when you connect the repo via **Blueprint** (New + → Blueprint).
