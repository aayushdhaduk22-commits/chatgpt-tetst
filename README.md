# Reform · Urban Material Bank

A responsive, animated React marketplace frontend for reclaimed construction materials.

## Develop

Requires Node.js 22 or newer.

```sh
npm ci --cache /tmp/urban-npm-cache
npm run dev
```

## Production

```sh
npm run build
npm run preview -- --port 4173
```

The deployable static site is `dist/`.

## Deploy on Render

1. Push this project to your GitHub repository.
2. Sign into Render and choose **New > Static Site**.
3. Connect `aayushdhaduk22-commits/chatgpt-tetst` and select the branch containing this code.
4. Set the build command to `npm ci && npm run build` and the publish directory to `dist`.
5. Create the site. Render will provide the public HTTPS URL.

Alternatively use **New > Blueprint**, connect the repository, and select `render.yaml`.

## Frontend scope

Search, category and condition filters, price sorting, saved items, detail dialogs, and listing creation are interactive. Saved items and new listings persist in this browser's localStorage only. Sample inventory and prices are illustrative. The seller contact action clearly explains its demo status. This frontend does not provide real authentication, public listing persistence, messaging, payments, or verified material suitability. These require a backend before launching a live marketplace.

Animation uses Motion with reduced-motion support. Fonts are self-hosted. Material imagery bundled in `public/images` avoids third-party image requests at runtime.
