# roshambo.cloud

Static site for RoShamBo's Android apps, hosted on Cloudflare Pages (and
mirrored by GitHub Pages at oreonl.github.io/website/ for older app builds
that still link there). No build step: every file is served as-is.

```
index.html                 home: links to both apps
styles.css                 shared styles; each page picks a theme on <body>
domnpcs/index.html         Deck of Many NPCs landing page
domnpcs/privacy/           Deck of Many NPCs privacy policy
domnpcs/img/               icon + three Play Store phone screenshots
firstroll/index.html       First Roll landing page
firstroll/privacy/         First Roll privacy policy
firstroll/img/             icon + three Play Store phone screenshots
3d3t.html                  3D Tic Tac Toe privacy policy
domnpcs.html               old policy locations: redirect stubs for GitHub
firstroll.html             Pages; _redirects does the same on Cloudflare
```

The apps link to `https://roshambo.cloud/<app>/privacy` and the Play
Console privacy-policy field for each app should point there too. The
screenshots under `*/img/` are copies of `app/src/main/play/listings/en-US/
graphics/phone-screenshots/` from each app repo, resized to 480px wide.
