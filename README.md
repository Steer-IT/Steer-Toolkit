# Steer IT Security Toolkit

Free security and IT checks from [Steer IT Solutions](https://steerits.co.uk), built as a single-page web app that can be added to an iPhone Home Screen.

**Domain and email:** Full domain report · My domains · Email security (SPF, DKIM, DMARC, MTA-STS) · Record builder · Blacklist check · Website scan · DNS lookup · Expiry check

**Security:** Breach check · Password check and generator

**Services and network:** Service status (Microsoft 365, TeamViewer, Cloudflare and more) · Speed test with connection details

## Hosting

Served with GitHub Pages from the `main` branch. Open the site in Safari on iPhone and choose **Share → Add to Home Screen** to install it.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app |
| `manifest.webmanifest` | App name, icons and Home Screen settings |
| `sw.js` | Keeps the app available offline (live checks are never cached) |
| `apple-touch-icon.png`, `icon-*.png` | App icons |
| `preview/` | Test copy for trying changes before they go live |
| `.github/workflows/status-relay.yml` | Copies Microsoft's public status to the `status-data` branch every 5 minutes, because the app can't read Microsoft's feed directly |

All checks run in the visitor's browser against public services (XposedOrNot, Have I Been Pwned's Pwned Passwords, Google and Cloudflare DNS, Mozilla HTTP Observatory, crt.sh, RDAP, public status pages and Cloudflare's speed test). Saved domains and service choices stay on the device.
