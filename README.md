# Blacksoil International — website (single-folder version)

Every file in this folder sits at the same level — **there are no sub-folders**.
This is the easiest version to upload to GitHub.

## How to put it on GitHub (clean method)
1. In your repo, delete the old messy files first (all the loose images + pages from the
   previous upload). Keep only: `CNAME`, `robots.txt`, `sitemap.xml`, and your `favicon`
   folder if you added them.
2. Click **Add file → Upload files**.
3. Select **ALL** the files inside this folder and drag them in together.
4. Commit. Wait for the deploy to finish (Actions tab → green check).
5. Open your site and hard-refresh (Ctrl+F5).

Because nothing is in a sub-folder, there is no folder structure to preserve — this avoids
the problem you hit before.

## What's here
- 8 pages: `index.html` (home) + the 7 product pages
- `support.js`, `image-slot.js` — required runtime
- the 7 `*.js` data files (product content)
- all images (photos, logos, technology images, icons) — all flat
- `favicon.png` + `apple-touch-icon.png` — browser-tab icon (already linked in every page)
- `sitemap.xml` — lists all 8 pages for Google (uses https://blacksoilintl.com)
- `robots.txt` — allows search engines + points to the sitemap
- `CNAME` — keeps your custom domain **blacksoilintl.com** connected
- `.nojekyll` — tells GitHub Pages to serve every file as-is

## Custom domain note
`CNAME` contains `www.blacksoilintl.com` — matching your existing setup. Uploading it keeps
your domain linked, so after the new upload check **Settings → Pages** still shows
www.blacksoilintl.com as the custom domain (re-enter it there if it was cleared). Your existing
DNS at the domain registrar does not need to change.

## Favicon note
This folder includes a fresh `favicon.png` + `apple-touch-icon.png` (your mountain logo on
brand green), already linked in every page — no sub-folder needed. If you'd rather keep your
previous favicon design, tell me and I'll match it instead.

## Enquiry form
Already wired to Web3Forms → delivers to sales@blacksoilintl.com, with validation,
success/error messages, and an invisible honeypot for spam. No setup needed.
