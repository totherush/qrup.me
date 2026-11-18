# qrup.me agent guide

Static Astro landing page for qrup, deployed to GitHub Pages at https://qrup.me. See README.md for the structure. The qrup CLI itself lives in `../qrup` (`totherush/qrup`).

Planned work lives in `PLAN.md`, a local file that is gitignored. When it is present, read it before starting, and update it when you finish or discover work.

## Commands

- `bun run check`: Astro type check and Biome. Run it before every commit.
- `bun run build`, then `bunx astro preview`: serves the built site on port 4321.

## Conventions

- Explicit types for props, variables, and functions; Biome bans `any`.
- Plain CSS with the custom properties in `src/styles/global.css`. The page follows the system color scheme, dark first.
- Claims on the page (platforms, options, security behavior) must match the qrup README. Check it when either changes.
- Keep client JavaScript to small `<script>` blocks; the page must work without it except for the Copy buttons.
- Check layout changes in a browser at desktop and phone widths (390 px), in dark and light.
