# petaly.app

Single-page landing for Petaly. Deployed via GitHub Pages with a custom domain.

## File structure

```
petaly.app/
├── CNAME                  ← contains "petaly.app" — GitHub Pages reads this
├── index.html             ← entire page (HTML + inline CSS, no build step)
├── icon.png               ← (you drop in) — favicon + optional hero icon
└── screenshots/
    ├── 01-home.png        ← Play Store screenshot slot 1 (Home — "track your moments beautifully")
    ├── 02-calendar.png    ← Play Store screenshot slot 2 (Calendar — "log, view, discover")
    └── 03-privacy.png     ← Play Store screenshot slot 4 (Privacy — "private by design")
```

## Before pushing to GitHub

1. Drop your Play Store icon PNG in as `icon.png` (the cherry-blossom flower).
2. Copy 3 of your 5 existing Play Store screenshots into `screenshots/` with those exact filenames.
   - Recommended: slot 1 (home), slot 2 (calendar), slot 4 (privacy). They give the best 3-up story.
   - If you'd rather use different slots, just rename them to `01-home.png` / `02-calendar.png` / `03-privacy.png`.

## Local preview

Just double-click `index.html` to open in your browser. No server needed.

## Notes

- The hero icon is currently an inline SVG of a cherry blossom (matches your brand). If you'd rather use the actual app icon, swap the `<svg class="hero-icon">…</svg>` block in `index.html` for `<img class="hero-icon" src="./icon.png" alt="Petaly">`.
- Privacy + Terms link to the existing combined page at `openmindsetgroup.com/privacy-terms.html` (with anchors).
- Contact email currently routes to `cltready@openmindsetgroup.com` — replace with a Petaly-specific address if you want.
