# autocare

Public website and privacy policy for the **AutoCare** mobile app (`com.innovaxons.autocare`), hosted on GitHub Pages at [https://autocare.innovaxons.com](https://autocare.innovaxons.com). Same setup as `InnovAxons-apps/salaty-site`.

## Hosting
- **GitHub Pages** from the `main` branch of this repository; custom domain in `CNAME`.
- **Cloudflare DNS:** CNAME `autocare` → `innovaxons-apps.github.io`, **DNS only** (grey cloud), so GitHub issues the HTTPS certificate. HTTPS is enforced in the Pages settings.
- **Publishing:** edit, commit and push to `main`; Pages deploys within minutes.

## Pages

| Language | Home | Privacy policy |
| :--- | :--- | :--- |
| English (default) | `/` (`index.html`) | `/privacy/` (`privacy/index.html`) |
| Arabic (RTL) | `/ar/` (`ar/index.html`) | `/ar/privacy/` (`ar/privacy/index.html`) |
| Not found | `404.html` | |

One shared `style.css` (system fonts, light and dark, logical properties for RTL). No analytics, cookies, external fonts or scripts.

## Source of truth
The English policy is `docs/PRIVACY_POLICY.md` in the app repository. Change it there first, then regenerate `privacy/index.html` (and update the Arabic translation, which defers to the English text). The Play Console privacy link is `https://autocare.innovaxons.com/privacy/`.

When the app is live on Google Play, replace the `<!-- PLAY_LINK -->` line and the "Coming soon" text on both home pages with the store link.

Contact: `innovaxons.apps@gmail.com`
