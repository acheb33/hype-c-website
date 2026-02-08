# HYPE-C Website Prototype

Single-file HTML/CSS/JS prototype for the Hype-C e-commerce storefront. This is a **design reference and content source** for the Shopify migration — not production code.

## What's in here

`hype-c-shopify-prototype.html` — fully self-contained prototype with:
- Home, Shop, About, and Ingredient Disclosure pages
- SPA-style navigation (JS page switching, no routing)
- Mobile-responsive breakpoints (375px, 480px, 768px, 1024px)
- Product variant selector and pricing display
- Scroll-reveal animations
- SEO meta tags and JSON-LD structured data
- WCAG 2.1 AA accessibility (skip links, ARIA, keyboard nav, focus management)

## Brand specs

- **Colors:** Neon Teal `#00D2D3`, Orange `#FF6B35`, Black `#0A0A0A`
- **Fonts:** Oswald Bold (headings), Bebas Neue (taglines), Barlow Condensed (body)
- **Aesthetic:** 90s Jazz cup, matte black, sports energy

## How to preview

Open the HTML file directly in Chrome, Safari, or Firefox. For mobile testing, serve locally:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000/hype-c-shopify-prototype.html` on your phone (use your computer's local IP).

> **Note:** Opening from iOS Files won't work — the sandboxed WebKit view blocks JavaScript.

## Shopify migration

This prototype simulates multi-page navigation in a single file. The actual Shopify store will use Liquid templates, theme sections, and Shopify's cart/checkout. Use this repo as the source of truth for:
- Copy and messaging
- Section layout and ordering
- Color/font/spacing values
- Mobile breakpoint behavior

## Status

Pre-launch. Target: March 28, 2026.
