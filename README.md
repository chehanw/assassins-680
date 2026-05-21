# The Fallen — Senior Assassins 2026

Hunger Games style tribute page for eliminated players.

## Files
- `index.html` — structure. Each `<article class="tribute">` is one fallen player.
- `style.css` — all styling. Design tokens at `:root`.
- `images/` — extracted headshots, one PNG per player (filename = lowercase last name).

## Iteration ideas
- **Date / time of elimination**: add a `<p class="eliminated">Day 12 · 11:42 PM</p>` under each `.name`.
- **Killer attribution**: add `<p class="killer">Eliminated by Jane Doe</p>` per tribute.
- **Sort modes**: chronological vs. alphabetical vs. by killer (would need JS + data).
- **Hover detail card**: expanded info on hover with method, location, witnesses.
- **Sound**: add a soft cannon-boom on page load or scroll into view (Hunger Games callback).
- **Animation polish**: scroll-triggered reveals instead of all on load (IntersectionObserver).
- **Data-driven**: extract the tribute list into a JS array and template render. Easier to maintain than HTML duplication.
- **District numbers**: assign each tribute a "district" (dorm, frat, etc.) and show below name.

## Missing photos
Ana, Nisha, Fionn, Armando — no photos in the source roster screenshots. Currently shown with `?` silhouette placeholder. Drop a PNG into `images/` and swap the `<article class="no-photo">` block for a regular one.

## Design tokens (style.css :root)
- `--gold`, `--gold-soft`, `--gold-dim` — accent palette
- `--bg`, `--bg-deep`, `--ash` — background palette
- `--display` (Cinzel), `--body` (EB Garamond) — fonts
- `--frame-radius` — currently 2px (very sharp). Try 0 for raw or 8px for softer.

## To preview locally
Open `index.html` directly in a browser (no build step).
