# uplyfire.github.io

Static landing page for **Uplyfire**, served via GitHub Pages at <https://uplyfire.github.io/>.

Used as the developer website URL in the Google Play Console listing.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Landing page — hero, apps grid, about, contact |
| `app-ads.txt` | AdMob authorized sellers declaration (required for ads.txt verification in Play Console) |
| `robots.txt` | Crawler directives |
| `sitemap.xml` | Sitemap for search engines |
| `assets/hero.jpg` | Hero background image |

## Deployment

GitHub Pages auto-deploys from `main`. After pushing, the live URL refreshes within ~60 seconds.

To verify after a change:
```
curl -I https://uplyfire.github.io/
curl https://uplyfire.github.io/app-ads.txt
```

## Updating app-ads.txt

The line `google.com, pub-5582308507713606, DIRECT, f08c47fec0942fa0` is the AdMob publisher declaration. Do not change unless AdMob explicitly provides a new line — and even then, **add** the new line rather than replacing existing ones (multiple sellers can be declared).
