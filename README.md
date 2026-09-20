# Gafat Art Painting and Design Works — Website

## How to use

Just `index.html` — no `images/` folder needed. Upload your artwork photos
to the **same folder** as `index.html` (repo root), using these exact filenames:

- **Collection One:** `art1.jpg` → `art20.jpg`
- **Collection Two:** `art1_01.jpg` → `art1_20.jpg`
- **Collection Three:** `art2_01.jpg` → `art2_20.jpg`
- **Collection Four:** `art3_01.jpg` → `art3_20.jpg`

Open `index.html` directly in a browser, or upload the repo to any static host
(GitHub Pages, Netlify, Vercel, etc.) — `index.html` should stay at the top level
of the repo for GitHub Pages to find it automatically.

If a photo is missing or not yet uploaded, that card shows an elegant placeholder
instead of breaking — so the site works even before every artwork is in place.

## Editing content

Open `index.html` and find the `section1` / `section2` / `section3` / `section4`
arrays near the top of the `<script>` block — these list every filename directly.
Each collection also has an `en` (English title), `am` (Amharic title), and `intro`
line you can edit. Titles for individual pieces ("Artwork 01", etc.) are set in the
`toImages()` function — edit there, or per-image, to add real titles later.

## Routing

Collection pages use hash-based routes, so the site works as a single static file
with no server config: `index.html#/gallery/collection-1`, `#/gallery/collection-2`, etc.
