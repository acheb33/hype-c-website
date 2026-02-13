# CLAUDE.md

Project context for AI-assisted development on the HYPE-C website prototype.

## Architecture

This is a **single-file website**. Everything (HTML, CSS, JS) lives in `index.html`. Do not create additional HTML, CSS, or JS files. Do not introduce build tools, bundlers, or package managers.

Pages (Home, Product, About, CA Disclosure) are toggled via the `showPage()` JavaScript function. There is no router — just `display: none / block` with fade transitions.

## Copy rules

- No em dashes. Use periods, commas, or parentheses instead.
- "Gym bags" is not a valid surface example (not a hard surface). Use: counters, highchairs, doorknobs, toys.
- The product has exactly three ingredients: water, salt, and hypochlorous acid. Never say "electricity" in user-facing copy.
- Brand voice: direct, clean, confident. No jargon, no filler, no superlatives.
- Each claim should live in one place. Don't repeat the same message across sections.

## Brand system

- **Teal** `#00D2D3` — primary, links, accents
- **Orange** `#FF6B35` — hover states, secondary accents (never on the nav logo)
- **Off-Black** `#0A0A0A` — backgrounds
- **Fonts:** Oswald (headings), Bebas Neue (taglines), Barlow / Barlow Condensed (body)
- All fonts loaded from Google Fonts — no local font files.

## Founder structure

- Dr. Kathy Nguyen and Dr. Tina Pham each get their own full card (physician founders).
- Alex Chebaro and Tu Duong share a single combined card (operations founders).

## Mobile / accessibility

- Breakpoints: 375px, 480px, 768px, 1024px
- All touch targets must be at least 44px (WCAG 2.1 AA)
- Body scroll must be locked when mobile hamburger nav is open
- Skip link, ARIA labels, focus management on page transitions are already in place — preserve them.

## Deployment

GitHub Pages from `main` branch root. The workflow is at `.github/workflows/pages.yml`. Live at hype-c.com.

## What not to do

- Don't create new files unless absolutely necessary.
- Don't add npm, webpack, or any build tooling.
- Don't remove accessibility features (skip links, ARIA, focus management, keyboard nav).
- Don't use `alert()` for production UX — the current add-to-cart alert is a placeholder for Shopify.
- Don't commit secrets, API keys, or credentials.
