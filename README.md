# Gafat Art Painting and Design Works — Website

## How to use

1. This folder contains `index.html` and an empty `images/` folder.
2. Drop your 80 artwork files directly into `images/` — no subfolders — using these exact names:

   - **Collection One:** `art1.jpg` → `art20.png`
   - **Collection Two:** `art1_01.jpg` → `art1_20.jpg`
   - **Collection Three:** `art2_01.jpg` → `art2_20.jpg`
   - **Collection Four:** `art3_01.jpg` → `art3_20.jpg`

3. Open `index.html` directly in a browser, or upload the whole folder to any static host
   (Netlify, Vercel, GitHub Pages, cPanel, etc.).

If an image file is missing, that card shows an elegant placeholder instead of breaking —
so you can launch the site before every artwork is in place and fill images in over time.

## Editing content

Open `index.html` and find the `collections` array near the top of the `<script>` block.
Each collection has an `en` (English title), `am` (Amharic title), and `intro` line you can edit directly.
Each artwork's `title` is generated automatically as "Artwork 01", "Artwork 02", etc. — edit the
`toImages()` output, or the `title` field per image, to add real titles, descriptions, year, or medium later.

## Routing

Collection pages use hash-based routes so the whole site works as a single static file with
no server config needed: `index.html#/gallery/collection-1`, `#/gallery/collection-2`, etc.
