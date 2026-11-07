# Raghu Bhai Telugu – VIP Channel Landing Page

A single-page, mobile-first landing page that invites visitors to join the official VIP Telegram channel. It shows a gold-themed card with a "Join Now Telegram" button and a 15-second circular countdown that redirects visitors to the Telegram invite link automatically.

## Technologies

- Plain HTML, CSS and vanilla JavaScript (no build step)
- Google Fonts (Cinzel, Plus Jakarta Sans) and Font Awesome icons, loaded from CDNs
- Hosted on Netlify as a static site

## Running locally

Open `index.html` in a browser, or serve the folder with any static server, e.g.:

```bash
npx serve .
```

## Editing

- Telegram invite link: change it in two places in `index.html`, the `href` of `#joinBtn` and `destinationURL` in the script.
- Countdown length: `totalSeconds` in the script.
- Channel name and tagline: the `.brand-title` and `.tagline` elements.
