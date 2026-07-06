# Mapbox App

A React + Vite app that renders an interactive [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/) map.

## Setup

This project requires **your own** Mapbox access token — it is **not** included in the repo.

1. Create a free account at [mapbox.com](https://account.mapbox.com/) and copy your **default public token** (starts with `pk.`).
2. In the project folder, create a `.env` file (see `.env.example`):

   ```env
   VITE_MAPBOX_TOKEN=pk.your_token_here
   ```

3. Install dependencies and start the dev server:

   ```bash
   npm install
   npm run dev
   ```

> The `.env` file is gitignored, so your token is never committed. Vite only reads it at startup — **restart the dev server** after changing it. Tip: add URL restrictions to your token in the Mapbox dashboard before deploying publicly.

## Licensing & Attribution

- **Mapbox GL JS is proprietary** (v2.0+), governed by the [Mapbox Terms of Service](https://www.mapbox.com/legal/tos) — not an open-source license. Using it requires a Mapbox access token and acceptance of those terms.
- Usage is billed on a **map-loads / sessions** model with a monthly free tier. Check current limits and pricing at [mapbox.com/pricing](https://www.mapbox.com/pricing).
- The Mapbox logo and map **attribution must remain visible** (added by default). Do not remove them unless your Mapbox plan explicitly permits it.
- Prefer a fully open-source stack? [MapLibre GL JS](https://maplibre.org/) (BSD-3) is a near drop-in alternative that needs no token, though you supply your own tile source.

---

## React + Vite Template Notes

This project was bootstrapped with a template that provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
