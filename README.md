# elysa-fit

Static legal site for [elysa.fit](https://elysa.fit). Hosts the marketing landing, Terms of Service, and Privacy Policy referenced by the App Store, Play Console, and RevenueCat.

## Pages

- `/`         — landing
- `/terms`    — Terms of Service
- `/privacy`  — Privacy Policy

Pretty URLs (no `.html`) are served via Cloudflare Pages' `_redirects` file.

## Deploy

Cloudflare Pages, auto-deploys on push to `main`. No build step. The canonical source markdown lives in `elysa-meta/legal/`; the HTML here is hand-converted from those files. If you change the legal copy, update the markdown first, then port the changes here.

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```
