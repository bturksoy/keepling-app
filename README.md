# Keepling — website

The public page for **Keepling: Baby Memory Journal**, served by Firebase Hosting
(project `keepling-bd31b`) at <https://keepling.btrinteractive.de/>. GitHub Pages
still mirrors it at <https://bturksoy.github.io/keepling-app/>.

It exists partly because Google's OAuth consent screen requires an application
home page before it will let the app publish, and partly because the app
deserved somewhere to point at.

- `index.html` — the whole page; no build step, no dependencies
- `assets/` — app icon and screenshots, copied from the app repo's `store/`

- `privacy/`, `support/` — privacy policy and support pages (the App Store and
  Play listings link here)
- `app-ads.txt` — authorises Google AdMob (publisher pub-5739429543010636) to sell
  ads in the Keepling apps. AdMob reads it from the root of the developer website
  listed in the stores, so it must stay at `/app-ads.txt` on this domain.

To change something, edit the files, push to `main`, then deploy:
`firebase deploy --only hosting` (pushing alone only updates the Pages mirror).
