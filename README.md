# qrup.me

The landing page for [qrup](https://github.com/totherush/qrup), served at https://qrup.me.

Built with [Astro](https://astro.build) as a static site. GitHub Actions deploys every push to `main` to GitHub Pages.

## Development

Requires [Bun](https://bun.sh) and Node 24 (see `.nvmrc`).

```bash
bun install
bun run dev      # http://localhost:4321 with live reload
bun run check    # Astro type check and Biome
bun run build    # static site in dist/
```

## Structure

- `src/pages/index.astro`: the page, composed from the sections in `src/components/`
- `src/site.ts`: links and the install command used across sections
- `src/assets/`: screenshots, optimized to WebP at build time
- `public/`: favicon and the Open Graph image (`og.png`, 1200×630)

The screenshots come from the qrup repo (`.github/screenshots/`). Copy them again when they change there.
