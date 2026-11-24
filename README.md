# Run4Sudan website

A responsive, static Astro homepage for https://run4sudan.ca.

## Requirements
- Node.js 20.3+ (or a current supported Node LTS)
- npm

## Run locally
```bash
npm install
npm run dev
```
Open the local URL printed by Astro (usually http://localhost:4321).

## Build
```bash
npm run build
npm run preview
```

## Replace the visual assets
The current design includes intentional image placeholders. Add your approved event photography to `public/images/` using these exact filenames:
- `run4sudan-hero.jpg` — wide hero image, ideally 2200×1400 or larger; a strong group/race-day photo works best.
- `run4sudan-event.jpg` — vertical or portrait event photograph.
- `run4sudan-community.jpg` — wide community/team photograph for the final call-to-action.

Replace the temporary text logo in `src/pages/index.astro` with your official logo. If your logo is SVG, put it at `public/images/logo.svg` and use an `<img src="/images/logo.svg" ...>` element in the header and footer.

## Update content
Homepage content is in `src/pages/index.astro`. Main design tokens and responsive styling are in `src/styles/global.css`.

Before publishing, verify the public contact email, Instagram URL, charity partner naming/links, impact figures and any future event details. The current contact email and Instagram path are editable placeholders based on the project brief.

## Deploy
This is a static Astro site and can be deployed to Cloudflare Pages or another static host. For Cloudflare Pages, connect the GitHub repository and use:
- Build command: `npm run build`
- Build output directory: `dist`

Then add `run4sudan.ca` as a custom domain in the hosting dashboard and follow the provider's DNS instructions. Keep existing GoDaddy MX/TXT records if you use GoDaddy email; do not replace all DNS records blindly.
