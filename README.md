# pos-ev-pharm

Static WebR-powered explorer for three competing drug candidates. Enter each company's success probability (0–1), release date, and patent expiry. The app computes expected market share for Company A and shows scenario timelines:

- Uses WebR to run R logic fully client-side (GitHub Pages friendly, no backend).
- Vite dev/build setup: `npm install`, `npm run dev`, `npm run build`, `npm run preview`.
- GitHub Pages workflow in `.github/workflows/pages.yml` builds on `main` and deploys `dist`.

Deploy notes:
- `vite.config.js` sets `base` to `/pos-ev-pharm/` for repo-based Pages; change to `/` for user/org root.
- WebR loads from CDN, so the page needs network access when viewed.***
