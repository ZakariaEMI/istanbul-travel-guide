# Istanbul Atlas V4 — Explore in Motion

A public-facing static Istanbul travel guide, inspired by animated city-walk experiences. Free to use on GitHub Pages; **no npm, database or build required**.

## Deploy to your existing GitHub Pages website

1. Download the ZIP and extract it.
2. In `https://github.com/zakariaemi/istanbul-travel-guide`, open **Code → Add file → Upload files**.
3. Upload **`index.html`, `style.css`, `data.js`, `app.js`** to the root of the repository. Replace existing versions of these files if present.
4. Commit to `main` and watch **Actions** for the Pages deployment.
5. Open `https://zakariaemi.github.io/istanbul-travel-guide/#/home`.

**Important:** `app.js` is new. The previous version's `script.js` is no longer used. Old GitHub commits can still contain previous personal notes; this update does not rewrite repository history.

## Features
- Dark responsive cinematic homepage
- Three self-guided animated map walks with clickable numbered stops, next/previous and autoplay
- Interactive Leaflet map using free CARTO dark tiles and OpenStreetMap attribution
- Place directory: 34 clickable destinations with dedicated detail pages
- Search by place, neighborhood or listed brands; category filters
- Shopping mall and market directories with examples from the older user-supplied Istanbul PDF reference material (not live store availability)
- Local favorites stored in browser localStorage only
- Google Maps links for each stop / point-to-point walking legs
- Accessible labels and reduced-motion support

## Accuracy and public-content policy

- **Route lines are schematic** straight segments between destination markers — not actual pedestrian paths and not a live GPS map. Visitors must use Google Maps or official maps for walking directions. Do not claim route distances or step counts as measured.
- Store directories reflect reference lists, **not confirmed current tenants**. Always verify the mall's official tenant directory.
- The images are scenic Istanbul photographs used as visual atmosphere and **may not depict the exact place shown in each card**.
- Third-party Leaflet, CARTO map tiles and Google Fonts need an internet connection.
- Before publishing a commercial website, check the photo licenses and replace illustrative stock imagery with appropriately licensed, destination-specific photos.
- All personally identifying notes, visit dates, contact details and private shopping comments have been excluded from public data.

## Content editing
- `data.js` contains the curated places, place coordinates, photos, and three tours. Change or add destinations in the `window.PLACES` array; tours reference place `id` values.
- `style.css` handles the layout, animation, typography and mobile breakpoints.
- `app.js` handles navigation, filters, favorites, map interactions and stop animations.

## Sources
The place directories began from user-supplied reference PDFs (İstinyePark, Mall of Istanbul, Capacity, Optimum AVM, A Plus, Kanyon and other Istanbul shopping notes) and the previous public website's directory. Old notes were edited into public-facing material without personal visit histories.

For transit verification: https://www.metro.istanbul/en/
For ferry information: https://www.sehirhatlari.istanbul/en
