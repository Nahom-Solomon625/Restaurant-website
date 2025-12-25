# Crimson Rooster Kitchen — Restaurant Website (HTML + CSS)

A visually appealing, multi-page restaurant website with a soft white background and red/yellow theme. Built with **only HTML and CSS** (no JavaScript).

## Pages

- `index.html` — Homepage (hero + signature picks)
- `menu.html` — Menu page using **CSS Grid** with **CSS-only filters**
- `gallery.html` — Gallery with a **CSS-only lightbox** (`:target`)
- `contact.html` — Contact page with a form and a **CSS-only “Thanks” state**

## How to Run

### Option A: Open directly

Double-click `index.html`.

### Option B: Run a local server (recommended)

From the project folder:

```bash
python -m http.server 5500
```

Then open `http://localhost:5500`.

## Editing Images (Single Place)

All Unsplash image URLs are listed in:

- `data/unsplash-images.json`

This file is meant to be your **edit hub** (so you can swap invalid images easily).

Important: because this project is **HTML/CSS only**, the site cannot automatically load JSON at runtime. After you change a URL in the JSON, copy/paste it into the relevant HTML file.

### What’s inside the JSON

Each key includes:

- `query` — the search term used to pick the image
- `raw` — Unsplash CDN raw URL
- `hero` — large cropped image (good for hero backgrounds)
- `card` — medium cropped image (good for cards)
- `square` — square crop (used by menu item images)
- `full` — large crop (used by the gallery lightbox)

## CSS-only Interactions

- **Mobile nav**: checkbox + label toggle in the header
- **Menu filters**: radio buttons + CSS selectors to hide/show items
- **Gallery lightbox**: anchor links + `:target`
- **Contact “Thanks”**: form `action="#thanks"` + `#thanks:target`

## Theme / Styling

- Main styles: `css/style.css`
- Fonts: Google Fonts (`Inter` + `Playfair Display`)
- Palette: soft white background with red/yellow accents

## Notes

- If images don’t show, verify you have internet access and that the URL you’re using is reachable.
- The previous `source.unsplash.com` style links can return errors; this project uses `images.unsplash.com` CDN links instead.

