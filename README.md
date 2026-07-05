# Blacksoil International — deployable website

This folder is ready to publish on GitHub Pages (or Netlify, Vercel, any static host).

## How to deploy on GitHub Pages
1. Create a new GitHub repository.
2. Upload **the contents of this `site/` folder** to the repository root — that means
   `index.html`, all the other `.html` files, `support.js`, `image-slot.js`, `.nojekyll`,
   and the `data/` and `images/` folders. (Upload the files *inside* `site/`, not the
   `site` folder itself.)
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   pick branch `main` and folder `/ (root)`, then Save.
4. Wait ~1 minute, then open the URL GitHub shows you. `index.html` loads automatically.

## Enquiry form (email + anti-spam)
The enquiry form on every page is wired to **Web3Forms**, which delivers submissions to
**sales@blacksoilintl.com** (the address your Web3Forms access key is registered to). It has:
- inline validation (required fields + valid email) with error messages,
- a success message when it sends and an error message if it fails,
- an **invisible honeypot** field (no checkbox for visitors) that Web3Forms checks automatically.

No extra setup is required — the access key is already embedded in the pages.

**Optional free spam hardening:** if you create a free Web3Forms account with
`sales@blacksoilintl.com`, open your form → Security Settings and turn **Advanced Spam Filter
ON** (leave "Captcha Protection" = None). This adds more invisible filtering at no cost.
Note: Google reCAPTCHA and Cloudflare Turnstile in Web3Forms are **paid (Pro)** features — you
do not need them; the honeypot + Advanced Spam Filter cover a contact form well.

## Notes
- The site needs an internet connection the first time it loads (it pulls React from a CDN).
- `index.html` is the home page; the other pages are linked from the nav, footer, and product cards.
- To edit content later, the per-page text lives in the `data/*.js` files.
