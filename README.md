# lyn. — 2nd website template

A single-page portfolio for lyn.: a profile column and a bento grid of small interactive pieces, drawn live on canvas in a dithered halftone style with hairline vector details.

## Run it

It's one self-contained file. Open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
```

To publish it with GitHub Pages, set Pages to deploy from the `main` branch, root folder.

## What's inside

- **Profile**: a spinnable planet avatar (drag to spin, tap for night), intro text, and filters for worlds, toys and notes.
- **Pieces**: Pond, Baon (Filipino packed lunches), One hand (24-hour clock), Rooms, Weather, Pace, Atlas, Wind, Grow, Hollowmere, Motion, Today's slip (an activity receipt that logs what you do on the page), and Commissions.
- **Pace dial**: speeds up or slows down every animation on the page.
- **Sound**: soft chimes and an ambient wind loop, made with the Web Audio API. It can be muted from the footer.

Fonts are Public Sans and Geist Mono from Google Fonts. There are no other dependencies.

## Placeholders to fill in

- `#hello` (Say hello), `#hollowmere` and `#motion` are placeholder links.
- "Commissions are open" and the "last posted" line are sample copy.
