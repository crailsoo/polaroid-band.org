# POLARØID website

Static website prepared for **Cloudflare Workers Static Assets** via Git integration.

## Cloudflare build/deploy settings

- Production branch: `main`
- Build command: none required
- Deploy command: `npx wrangler deploy`
- Root directory: repository root
- Static asset directory: `public`

Wrangler reads `wrangler.jsonc` from the repository root and deploys the complete `public/` directory as static assets.

## Structure

- `wrangler.jsonc` — Cloudflare Workers static-assets configuration
- `public/index.html` — website
- `public/assets/images/` — release + gallery images
- `public/POLAROID_EPK_2026_EN.pdf` — EPK download
- `public/favicon.svg` — favicon
- `public/site.webmanifest` — web manifest
- `public/robots.txt` — crawler rules
- `public/_headers` — response-header rules where supported

The website has no framework and no dependency-installation step. Cloudflare can deploy it directly with `npx wrangler deploy`.

Once the final custom domain is connected, the canonical URL can be added to `public/index.html`.
