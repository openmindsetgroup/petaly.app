# petaly.app

Single-page landing for Petaly — a beautiful, private intimacy tracker for Android. Deployed via GitHub Pages with a custom domain. Styled to the **Midnight Bloom** brand system (plum gradient, Quicksand + Fredoka, blossom-pink accents).

## File structure

```
petaly.app/
├── CNAME                  ← contains "petaly.app" — GitHub Pages reads this
├── index.html             ← entire page (HTML + inline CSS, no build step)
├── icon.png               ← app icon — favicon + hero logo
└── screenshots/
    ├── 01-home.png        ← Home — "track your moments beautifully"
    ├── 02-calendar.png    ← Calendar — "log, view, discover"
    └── 03-privacy.png     ← New entry — "custom notes, activities, tags"
```

## Page sections

The page is a single `index.html` with inline CSS (no build step, no JS). In order:

1. **Hero** — app icon, brand, headline, and a "Free to use · $8.99 once to go further" line + Play badge.
2. **Positioning chips** — Beautiful · Private · Free to use · No accounts · No ads.
3. **Screenshots** — three Play Store frames in soft, haloed cards.
4. **Capabilities** — six cards covering what the app does (unlimited entries, calendar, stats, custom activities, app lock, free export).
5. **Private by design** — four privacy cards + the Play "Data safety: no data collected, no data shared" line.
6. **Pricing (free-first)** — the free tier as the hero ("the whole tracker is free, forever"), with Premium ($8.99 one-time) framed as an optional upgrade that adds depth, not access.
7. **About** + **Footer** (Privacy Policy, Terms, Contact).

## Editing notes

- **Copy is governed by `../../FACTS.md`** — the verified claims sheet. Every marketable claim on this page must trace to it. Keep the free/premium split precise (free = up to 5 custom activities, basic stats, dark mode; premium = unlimited activities, advanced graphs, themes). Never reintroduce forbidden wording (e.g. "doesn't connect to the internet" / "no INTERNET permission").
- **Brand:** Midnight Bloom style guide. Colors and type are defined as CSS variables in the `:root` block of `index.html`. One accent per headline — closing word in blossom pink.
- The hero uses the real `icon.png`. Screenshots are the finished Play Store marketing frames (plum background + captions already baked in), shown as-is.
- Privacy + Terms link to the combined page at `openmindsetgroup.com/privacy-terms.html` (with anchors). Contact routes to `info@openmindsetgroup.com`.

## Local preview

Just double-click `index.html` to open in your browser. No server needed.

## Deploy

GitHub Pages serves `main` from this repo on the custom domain (see `CNAME`). A `git push origin main` publishes the live site within a minute or so.
