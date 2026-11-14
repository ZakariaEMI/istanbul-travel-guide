# Istanbul Atlas — Static GitHub Pages website

A responsive, build-free travel guide. Includes category filters, search, Google Maps links, favorites (saved in the current browser), a sample walking day, and transit tips.

## Deploy to your existing GitHub Pages repository

1. Open https://github.com/zakariaemi/istanbul-travel-guide
2. Select **Add file → Upload files** and upload the **index.html** file from this folder to the **repository root** (not into another folder). Replace any existing index.html, or edit it with the new contents.
3. Commit to the branch used by your GitHub Pages workflow (usually `main`).
4. Since your existing deployment uses a **Static HTML** GitHub Actions workflow, it should publish automatically after the commit.
5. In the **Actions** tab, confirm the latest Pages deployment succeeded; then open https://zakariaemi.github.io/istanbul-travel-guide/.

If the repository does not yet have a Static HTML deployment workflow, go to **Settings → Pages**, select **GitHub Actions**, and configure the **Static HTML** starter workflow. Commit it to the default branch.

## Customize

Everything is inside `index.html` so it works without Node.js or a build step.

- Update the `<title>`, hero copy and other HTML text.
- Edit `const places = [...]` near the bottom of `index.html` to add or remove locations. Each location has `id`, `name`, `category`, `area`, `emoji`, `bg`, `desc`, `tags`, `source`, and `map`.
- Keep ids unique and categories aligned with the `categories` array.
- Favorites persist only in the visitor's browser via localStorage, not across devices.
- The Google Fonts CDN and third-party map/source links require internet access; the main site otherwise runs without external assets.

## Important content note

The shared ChatGPT conversation at https://chatgpt.com/share/6af878a4-a868-83ea-894f-3499511ad465 did not expose its actual text to the available browser. This is therefore a **starter edition**, not a claim to have imported the user's full personal source material or PDF notes. The locations and generic summaries have been assembled from publicly accessible information. Opening hours and fares are intentionally omitted because they change. Review locations and links before relying on them.

## Public source references

- https://istinyepark.com.tr/en/
- https://istinyepark.com.tr/en/stores
- https://istanbul.ktb.gov.tr/
- https://www.metro.istanbul/
- https://sehirhatlari.istanbul/en
- https://istanbul.travel/en/grand-bazaar?gruppe=basare
- https://istanbul.travel/en/spice-bazaar?gruppe=basare

This is an independent guide and is not affiliated with the destinations above.
