# Trap and Skeet promo site

Static landing page, no build step. Open `index.html` or run:

    python3 -m http.server 8765

- Every store button links to `/go/garmin/`, a redirect page that counts each click as a pageview in Cloudflare Web Analytics. To change the store link, edit the URL in `go/garmin/index.html` (it appears three times on that page).
- Cloudflare Web Analytics: the token goes in `data-cf-beacon` in both `index.html` and `go/garmin/index.html`.
- Images in `img/` are resized copies of the store screenshots from the Garmin app repo.
