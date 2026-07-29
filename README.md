# cloudinnovationnetwork.com

Premium informational / demonstration site for **cloudinnovationnetwork.com**.

Built as a fully static Astro project optimized for **Cloudflare Workers Static Assets**.

## Stack

- **Astro 5** (static output, no adapter)
- **TypeScript** (strict)
- **Tailwind CSS**
- **Content Collections**
- **@astrojs/sitemap**
- Full Open Graph + Twitter Card + JSON-LD structured data
- Mobile-first responsive design
- Cloudflare-ready headers & robots.txt

## Development

```bash
npm install
npm run dev
```

## Build & Deploy (Cloudflare Workers Static Assets)

```bash
npm run build
npx wrangler deploy
```

Or simply:

```bash
npm run deploy
```

### wrangler.toml notes

This project uses pure static assets (no Worker script / no `@astrojs/cloudflare` adapter):

```toml
name = "cloudinnovationnetwork-com"
compatibility_date = "2026-07-29"

[assets]
directory = "./dist"
```

After the first deploy, attach the custom domain `cloudinnovationnetwork.com` in the Cloudflare dashboard (or via zone routes).

## Domain Acquisition

All sales and acquisition inquiries:

**sales@desertrich.com**

## Disclaimer

This website is for demonstration and informational purposes only. It does not constitute an offer of services, a commitment to deploy, or a guarantee of outcomes. All statistics, projections, and references to specific technologies are based on publicly available information as of the date shown and are subject to change.
