# Wei-Hsun Wang — CV website

A self-contained, single-page CV website for Wei-Hsun Wang (王偉勳),
ready to host on **GitHub Pages** (or any static host).

## Deploy on GitHub Pages

1. Create a repository and upload **all files in this folder to the repository root**
   (keep the filenames as-is, including the leading-dot `.nojekyll`).
2. In the repo: **Settings → Pages**.
3. Under *Build and deployment*, set **Source = Deploy from a branch**, then choose
   your branch (e.g. `main`) and **folder = `/ (root)`**. Save.
4. Wait ~1 minute. Your site goes live at
   `https://<your-username>.github.io/<your-repo>/`.

> Tip: for a *user/organization* site, name the repo `<your-username>.github.io`
> and it will be served from `https://<your-username>.github.io/`.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The CV page (all CSS, JS, fonts refs, photo & logos are embedded). |
| `icon.svg` | Scalable favicon (modern browsers). |
| `favicon.ico` | Classic favicon, 16/32/48 px (older browsers, `/favicon.ico` requests). |
| `apple-touch-icon.png` | 180×180 home-screen icon for iOS/iPadOS. |
| `icon-192.png`, `icon-512.png` | App icons referenced by the web manifest (Android / PWA). |
| `site.webmanifest` | Web app manifest (name, icons, theme colors). |
| `robots.txt` | Search-engine rules (see *Search visibility* below). |
| `404.html` | Themed "page not found" page served by GitHub Pages. |
| `.nojekyll` | Tells GitHub Pages to serve files as-is (no Jekyll build). |
| `logo_cch.png`, `logo_nchu.png` | Transparent institution logos (already embedded in the page — included here as reusable assets; optional). |

## Customize before/after going live

- **Social-share previews & canonical URL.** `index.html` currently points the
  Open Graph / Twitter tags at `https://wangwhmd.com/`. Update these three lines
  in `<head>` to your live URL so link previews show the right address and image:
  `og:url`, `og:image`, `twitter:image`.
- **Search visibility.** The page is set to **not** be indexed by search engines
  (noindex meta tags + `robots.txt`). To make it discoverable, remove the
  `robots`/`googlebot`/`bingbot` meta tags in `index.html` and change
  `Disallow: /` to `Disallow:` in `robots.txt`.
- **Custom domain (optional).** To use your own domain, add a file named `CNAME`
  (no extension) at the repo root containing only the domain, e.g.
  `www.example.com`, then set the DNS records as described in GitHub's
  "Managing a custom domain" docs.

## License / assets

The institution logos (National Chung Hsing University; Changhua Christian
Hospital / Changhua Christian Medical Foundation) are the property of their
respective owners and are used here for affiliation/identification only.
