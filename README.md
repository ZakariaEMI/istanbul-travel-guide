# Istanbul Atlas V3 — Public Istanbul visitor guide

A responsive, free static website for **everyone**. No personal travel history or private preferences appear in the shipped application data, pages, or README.

## Features
- 26 clickable destination cards with shareable `#/place/SLUG` URLs
- Editorial photography for selected locations, graceful visual fallback for others
- Seven sample day itineraries, shopping and brand suggestions, official transport links
- Search and filters, browser-local favorites, mobile menu, transitions and scroll animations
- Reduced-motion accessibility support

## Deploy to GitHub Pages
1. Extract this zip.
2. Replace these four files in the root of your `istanbul-travel-guide` repository: `index.html`, `style.css`, `data.js`, `script.js`.
3. Commit to your `main` branch. Keep your existing working Static HTML GitHub Pages workflow.
4. Visit `https://zakariaemi.github.io/istanbul-travel-guide/` and hard-refresh if your browser retains the old site.

## Accuracy and image notes
- Store names are **examples of brands to look for**, not confirmed current tenants. Verify official directories.
- Suggested routes are not live navigation; operators' current maps and timetables take priority.
- Editorial photography is loaded from Unsplash; cards without imagery use a designed illustration.
- Favorites use localStorage and do not sync between devices.
- **Important privacy note:** replacing public site files does *not* erase older personal information from git history or previously published snapshots. If the old repository contains sensitive personal references, delete or rewrite history via a new clean repository and/or Git history cleanup before treating them as permanently removed.

## Edit content
Destinations are defined in `data.js`. UI routes and rendering are defined in `script.js`; visual styling is in `style.css`.
