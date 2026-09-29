# Dycers Site

Static GitHub Pages site for `www.dycers.com`. Open `index.html` through a local HTTP server; no build step, package installation or external fonts are required.

```sh
python3 -m http.server 8085
```

## Product focus

The site leads with existing pre-match arbitrage opportunities: find an opportunity in Radar, calculate each stake in Prepare, place the bets with the bookmakers, and follow the saved bets. Compare, Freebets, live tracking and History remain supporting features. The visual palette matches the app, including signature red `#ff1a1a` and mint profit highlights.

`index.html` contains the page, responsive CSS, keyboard-accessible screenshot tabs, native FAQ disclosures and SEO metadata. App Store, Google Play and existing legal-center destinations are preserved. Contact uses the app's support email.

## Screenshots

`assets/screens/radar.jpg`, `prepare.jpg`, `compare.jpg`, `freebets.jpg`, `my-bets.jpg`, `insights.jpg` and `upcoming.jpg` are 780×1688 captures of the updated app's actual React components. They were rendered using React Native Web with illustrative match/account data and the real UI calculations and assets. They are **not physical-iPhone screenshots** or current odds; the page identifies the data as illustrative. No customer data or real ad clicks were used. `insights.jpg` and `upcoming.jpg` are included as additional screenshots for future content.

The older `homescreen.jpg`, `choose-bet.jpg` and `history.jpg` remain available but are no longer used on the landing page. `assets/logo.png` remains the favicon/app icon.

The landing page references content-hashed copies of the five displayed captures (for example, `radar-9ba3bd30c414.jpg`). Whenever a capture changes, create a new filename based on its SHA-256 hash and update both HTML and gallery data. This prevents browsers from reusing an older UI screenshot cached under the same URL. Keep previous assets available for visitors with cached HTML.

## Verification

Local browser checks passed at 320, 390, 768, 1024 and 1440px: no horizontal page overflow, all images decoded, screenshot tabs and arrow/Home/End keyboard controls worked, FAQs expanded, download anchors reached their section, and reduced-motion preferences were respected. App Store, Google Play and legal destinations were compared with the previous page. No production deployment was performed by these checks.

## Hosting files

Keep `CNAME`, `.nojekyll` and `app-ads.txt` intact. Google AdMob uses the root `app-ads.txt` for app validation:

```txt
google.com, pub-2841348104860357, DIRECT, f08c47fec0942fa0
```
