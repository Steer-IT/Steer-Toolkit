# Steer IT Security Toolkit

Free security and IT checks from [Steer IT Solutions](https://steerits.co.uk), built as a single-page web app that can be added to an iPhone Home Screen.

**Tools:** Breach check · Email security (SPF, DKIM, DMARC, MTA-STS) · Password check · Website scan · DNS lookup · Speed test

## Hosting

Served with GitHub Pages from the `main` branch. Open the site in Safari on iPhone and choose **Share → Add to Home Screen** to install it.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app |
| `manifest.webmanifest` | App name, icons and Home Screen settings |
| `sw.js` | Keeps the app available offline (live checks are never cached) |
| `apple-touch-icon.png`, `icon-*.png` | App icons |

All checks run in the visitor's browser against public services (XposedOrNot, Have I Been Pwned's Pwned Passwords, Google and Cloudflare DNS, Mozilla HTTP Observatory, crt.sh and Cloudflare's speed test). Nothing is stored.
