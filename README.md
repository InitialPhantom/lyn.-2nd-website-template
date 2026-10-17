# lyn. — 2nd website template

A single-page portfolio for lyn.: a profile column and a bento grid of small interactive pieces, drawn live on canvas in a dithered halftone style with hairline vector details.

## Run it

It's one self-contained file. Open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
```

To publish it with GitHub Pages, set Pages to deploy from the `main` branch, root folder.

## What's inside

- **Profile**: a spinnable planet avatar (drag to spin, tap for night) and a short intro.
- **Pieces**: Pond, Bento (packed lunches from anywhere; a hand swaps the lid), One hand (24-hour clock), Rooms, Weather, Pace, Atlas, Wind, Grow, Hollowmere, Motion, Today's slip (an activity receipt that logs what you do on the page), Message me (a small chat box), and a serene.aiart gallery: portrait cards you drag sideways, shown dithered until you hover, each opening in a blurred in-page viewer.
- **Pace dial**: speeds up or slows down every animation on the page.
- **Sound**: soft chimes and an ambient wind loop, made with the Web Audio API. It can be muted from the footer.

Fonts are Public Sans and Geist Mono from Google Fonts. There are no other dependencies.

## Placeholders to fill in

- **Message me**: set `CONTACT_EMAIL` near the bottom of `index.html` to your address. "Send" then opens a pre-filled email to you. Until it's set, the tile tells visitors their message wasn't sent.
- **serene.aiart gallery**: three reels from @serene.aiart live in `art/` and are listed in the `ART` array near the bottom of `index.html`, with their caption and post link. To add or swap one, drop a video or image into `art/` and add an entry.
- `#hollowmere` and `#motion` are placeholder links.
- The "last posted" line is sample copy.
