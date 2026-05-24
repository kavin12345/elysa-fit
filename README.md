# elysa-fit

Static legal site for [elysa.fit](https://elysa.fit). Hosts the marketing landing, Terms of Service, and Privacy Policy referenced by the App Store, Play Console, and RevenueCat.

## Pages

- `/`         — landing (`index.html`)
- `/terms`    — Terms of Service (`terms/index.html`)
- `/privacy`  — Privacy Policy (`privacy/index.html`)

Pretty URLs work natively because each page is its own directory with an `index.html`. No build step, no rewrite rules, works the same locally and on Cloudflare Pages.

## Deploy

Cloudflare Pages, auto-deploys on push to `main`. No build step. The canonical source markdown lives in `elysa-meta/legal/`; the HTML here is hand-converted from those files. If you change the legal copy, update the markdown first, then port the changes here.

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```
