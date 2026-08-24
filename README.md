# POLARØID website

Static website prepared for **Cloudflare Pages**.

## Cloudflare Pages settings

- Production branch: `main`
- Framework preset: `None`
- Build command: `exit 0`
- Build output directory: `public`
- Root directory: repository root

The site has no framework and no dependency installation step.

## Structure

- `public/index.html` — website
- `public/assets/images/` — release + gallery images
- `public/POLAROID_EPK_2026_EN.pdf` — EPK download
- `public/favicon.svg` — favicon
- `public/site.webmanifest` — web manifest
- `public/robots.txt` — crawler rules
- `public/_headers` — Cloudflare Pages response headers

After the Cloudflare Pages project has been created, connect the custom domain in **Workers & Pages → your Pages project → Custom domains**.

Once the final domain is known, the canonical URL can be added to `public/index.html`.
