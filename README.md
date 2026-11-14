# Istanbul Atlas · Static multi-page travel guide

A responsive static website with clickable destination cards, deep-linkable detail views, shopping malls, outlet stores, markets, sights, metro/ferry advice, five trip ideas, browser-based favorites, and search.

## Deploy on existing GitHub Pages repository

1. Download and unzip the project.
2. In `https://github.com/zakariaemi/istanbul-travel-guide`, upload **index.html**, **style.css**, **data.js**, and **script.js** to the **repository root**, replacing previous files. Do not upload only `index.html`: it needs the other three files.
3. Commit to `main`.
4. If your GitHub Pages source is **GitHub Actions** with the **Static HTML** workflow, ensure it publishes the root directory (`.`) through `actions/upload-pages-artifact` and `actions/deploy-pages`. If it is already working, no workflow change is necessary.
5. Check the Actions tab, then open `https://zakariaemi.github.io/istanbul-travel-guide/#/home`.

No Node, npm, framework build, backend or external API keys are required.

## URL routes

- `#/home` homepage
- `#/explore` searchable directory
- `#/shopping` shopping directory
- `#/place/istinye` destination detail
- `#/transport` public transit
- `#/planner` daily routes
- `#/favorites` saved places

The old `#home` URL still opens the homepage, but navigation now uses `#/home` and `#/place/…` routes.

## Edit information

Edit `data.js` to update destination details, notes, brands or add a new destination. `script.js` generates separate navigable hash-route pages from the data. Detail pages are client-rendered (not separate HTML files), but have unique URLs and work on GitHub Pages without server-side routing.

Notes marked **Personal PDF** came from the user's historical 2024 personal reference documents. They are not verified current tenants or transport instructions. Other destination descriptions are curated general guidance. Check up-to-date official websites.

The homepage image is loaded from an external tourism photography URL and may not load offline. All other visuals use CSS/emoji illustrations and work without image hosting.

Favorites use browser `localStorage`, remain on the same browser/device, and aren't synced across devices.
