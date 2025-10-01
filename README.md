# Bronzebeard.dev

Bronzebeard.dev is my digital forge. The site hosts project notes, red-team writeups, and engineering playbooks, all published with Astro.

## What's Inside
- `src/pages/` route-level Astro files for the site shell
- `src/components/` shared UI blocks such as navigation, buttons, and cards
- `src/layouts/` page wrappers used across routes
- `src/content/blog/` Markdown entries for long-form posts
- `public/` static assets served as-is, including images and fonts

## Getting Started
Requirements: Node.js 18+, pnpm or npm, and Git.

```bash
# install dependencies
npm install

# run the dev server with hot reload
npm run dev

# build the production bundle into ./dist
npm run build

# preview the production build locally
npm run preview
```

`npm run build` performs type checks and generates the static Pagefind index used for on-site search. If you prefer pnpm, the scripts are identical (e.g. `pnpm install`).

## Configuration
- Update site metadata in `src/config.ts` (`SITE.title`, `SITE.website`, `SITE.editPost`, etc.)
- Tailor global styles in `src/styles/` (Tailwind tokens live inside the CSS files)
- Add or tweak content collections under `src/content/`

## Deployment Notes
The project produces a static bundle, so any static host (Vercel, Netlify, Cloudflare Pages, GitHub Pages) will work. Point your Porkbun DNS records to the host you choose and deploy the `dist/` directory created by `npm run build`.

## License
MIT — see `LICENSE` for details.
