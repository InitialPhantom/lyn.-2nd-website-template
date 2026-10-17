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
- **Pieces**: Pond, Baon (Filipino packed lunches), One hand (24-hour clock), Rooms, Weather, Pace, Atlas, Wind, Grow, Hollowmere, Motion, Today's slip (an activity receipt that logs what you do on the page), Message me (a small chat box), and a serene.aiart gallery: portrait cards you drag sideways, shown dithered until you hover, each opening in a blurred in-page viewer.
- **Pace dial**: speeds up or slows down every animation on the page.
- **Sound**: soft chimes and an ambient wind loop, made with the Web Audio API. It can be muted from the footer.

Fonts are Public Sans and Geist Mono from Google Fonts. There are no other dependencies.

## Layout editor (owner only)

You can rearrange and resize the grid yourself, straight on the site.

1. Make a GitHub token: **Settings → Developer settings → Fine-grained tokens → Generate new token**. Under **Repository access**, pick only this repo. Under **Permissions → Contents**, choose **Read and write**.
2. Open the site with `?edit` at the end of the address, for example `https://your-site/?edit`.
3. Paste the token. The page asks GitHub whether that token can write to this repo, and only then turns editing on. The token is kept in that browser only (localStorage). "Forget token" removes it.
4. Drag a tile to move it, and drag its blue corner to resize it. Everything snaps to the 4-column grid. Tiles that overlap turn red, and Save stays off until nothing overlaps.
5. **Save** commits `layout.json` to this repo. The site reads that file on load, so visitors see the new arrangement once your host serves the new commit.

Notes:
- The editor works on desktop and tablet widths. Phones keep the built-in stacked order.
- It needs the site served from a real address or a local server (`python -m http.server`). The Claude preview link can't reach GitHub and can't pass `?edit`.
- Delete `layout.json` to go back to the default arrangement.

## Placeholders to fill in

- **Message me**: set `CONTACT_EMAIL` near the bottom of `index.html` to your address. "Send" then opens a pre-filled email to you. Until it's set, the tile tells visitors their message wasn't sent.
- **serene.aiart gallery**: three reels from @serene.aiart live in `art/` and are listed in the `ART` array near the bottom of `index.html`, with their caption and post link. To add or swap one, drop a video or image into `art/` and add an entry.
- `#hollowmere` and `#motion` are placeholder links.
- The "last posted" line is sample copy.
