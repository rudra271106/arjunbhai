# AGENTS.md

## Architecture
A static, single-file site. Everything (markup, styles, script) lives in `index.html` at the repo root. There is no framework, package.json or build step. `netlify.toml` publishes the repo root as-is.

## Key files
- `index.html`: the landing page (gold "luxury card", CTA button, 15s countdown that redirects to Telegram).
- `netlify.toml`: publish directory `.`, empty build command.

## Conventions and notes
- Keep it dependency-free; external assets are limited to Google Fonts and Font Awesome CDN.
- The Telegram invite URL is duplicated: the `#joinBtn` href and `destinationURL` in the inline script. Update both together.
- The SVG timer circle geometry (`cx`, `cy`, `r`) is set in CSS. If the radius changes, update `stroke-dasharray` and the `circumference` constant in the script to match.
- The page content was supplied by the site owner. The `<title>` says "RAGHU BHAI TELGU" but the on-page heading says "ARJUN BHAI". Don't change branding unless the owner asks.
