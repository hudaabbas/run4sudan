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
Open the local URL (http://localhost:4321/run4sudan).


## Update content
Homepage content is in `src/pages/index.astro`. Main design tokens and responsive styling are in `src/styles/global.css`.

## Deploy
This static Astro site is deployed with GitHub Pages. Use:
- Build command: `npm run build`
- Build output directory: `dist`

TODO: add `run4sudan.ca` as a custom domain in the hosting dashboard and follow the provider's DNS instructions.