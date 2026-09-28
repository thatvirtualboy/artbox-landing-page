# Artbox website

The public landing page for [artbox.app](https://artbox.app), hosted on GitHub Pages from the root of `master`.

## Editing and preview

The home page is plain HTML in `index.html`, with its stylesheet and optimized images in `assets/site/`. No JavaScript or build step is required for the home page. The existing Jekyll configuration continues to publish the legacy supporting pages.

Run `python3 -m http.server 4173 --bind 127.0.0.1`, then open `http://127.0.0.1:4173`. This previews static files; legacy `_pages` routes require Jekyll or GitHub Pages to render.

Push to `master` to publish. Keep `CNAME` set to `artbox.app`. GitHub Pages builds should succeed before considering an update live.

## Content and assets

- App Store destination: https://apps.apple.com/app/id1557964462
- Gallery and artist images: the existing Artbox press kit, optimized as WebP.
- Photo book image: the Artbox iOS app's existing marketing asset.
- App icon: the published App Store icon.
- App Store badge and downloadable press kit: preserved from the original website.
- Free download, optional Artbox+, family sharing requirements, and device support checked against the public App Store listing and the app's FAQ.
- `/terms/` directs to Apple's standard EULA, as linked from the app.

The page includes a direct App Store link, Apple Smart App Banner, canonical URL, basic social metadata, structured app data, sitemap, responsive styles, native FAQ disclosures, keyboard focus indicators, and reduced-motion support. No tracking or analytics service is added.

## Privacy policy

`privacypolicy/index.html` is the public policy. It describes gallery/iCloud storage, optional AI and printing transfers, purchases, analytics, cloud-account deletion, and retained order data based on the app and backend source. Update it when those practices change. The backend currently has no fixed automatic deletion date for completed order records or ordered-book PDFs; do not claim one unless implemented.
