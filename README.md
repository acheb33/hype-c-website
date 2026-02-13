# HYPE-C Website Prototype

Single-file HTML/CSS/JS prototype for the **HYPE-C** e-commerce storefront — a physician-founded hypochlorous acid surface cleaner brand based in Houston, TX.

This is a **design reference and content source** for the upcoming Shopify migration, not production code.

**Live:** [hype-c.com](https://hype-c.com) | **Status:** Pre-launch (target March 28, 2026)

## Architecture

Everything lives in `index.html` — HTML, CSS, and JavaScript in a single self-contained file. Pages are swapped via JavaScript (SPA-style, no routing framework).

| Page | Description |
|------|-------------|
| Home | Hero, how-it-works, ingredients, pricing, CTA |
| Product | Bottle visual, variant selector, add-to-cart prototype |
| About | Founder bios (2 physicians + combined ops card), mission, stats |
| Ingredients | CA Cleaning Product Right to Know Act disclosure table |

## Brand system

| Element | Value |
|---------|-------|
| Primary | Neon Teal `#00D2D3` |
| Accent | Orange `#FF6B35` |
| Background | Off-Black `#0A0A0A` |
| Headings | Oswald 700 |
| Taglines | Bebas Neue |
| Body | Barlow / Barlow Condensed |
| Voice | Direct, clean, confident. No jargon, no hype. |

## Preview locally

Open `index.html` directly in a browser, or serve it for mobile testing:

```bash
python3 -m http.server 8000
```

> **Note:** Opening from iOS Files won't work — the sandboxed WebKit view blocks JavaScript.

## Deployment

Deployed via **GitHub Pages** from `main` branch root (`.github/workflows/pages.yml`).

### Custom domain DNS

| Type | Name | Value |
|------|------|-------|
| A | @ | `185.199.108.153` |
| A | @ | `185.199.109.153` |
| A | @ | `185.199.110.153` |
| A | @ | `185.199.111.153` |
| CNAME | www | `acheb33.github.io` |

Enforce HTTPS in **Settings > Pages** once DNS propagates.

## Shopify migration

This prototype simulates multi-page navigation in a single file. The Shopify store will use Liquid templates, theme sections, and native cart/checkout. Use this repo as source of truth for:

- Copy and messaging
- Section layout and ordering
- Color, font, and spacing values
- Mobile breakpoint behavior (375px, 480px, 768px, 1024px)

## Founders

| Name | Role |
|------|------|
| Dr. Kathy Nguyen | Co-Founder, Sports Medicine Physician |
| Dr. Tina Pham | Co-Founder, Pediatric Cardiologist |
| Alex Chebaro | Co-Founder, Operations & Strategy |
| Tu Duong | Co-Founder, Product & Design |

## Company

Hype Everything LLC, Houston, TX | [hello@hype-c.com](mailto:hello@hype-c.com) | [@get.hypec](https://instagram.com/get.hypec)
