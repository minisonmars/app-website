# minisonmars apps website

Plain static website for the Android apps, served at **apps.minisonmars.co.uk** by Cloudflare Pages. No build step: every file is served as it is.

## Pages

| File | What it is |
| --- | --- |
| `index.html` | Home page: a card for each app |
| `apps/toddler-launcher.html` | Toddler Launcher and the Toddler Parent app (incl. the accessibility service explanation) |
| `apps/toddler-doodle.html` | Toddler Doodle |
| `apps/toddler-camera.html` | Toddler Camera |
| `apps/caravan-leveller.html` | Caravan Leveller (repo `android-test`) |
| `privacy.html` | One privacy policy covering every app, with a section per app |
| `contact.html` | Contact email |
| `404.html` | Shown for unknown addresses |
| `style.css` | Shared styles (light and dark mode, phone-friendly) |
| `favicon.svg` | Browser tab icon |

App icons are small SVGs written straight into each page.

## Privacy policy links for Google Play

Use the section for each app:

- Toddler Launcher: `https://apps.minisonmars.co.uk/privacy#toddler-launcher`
- Toddler Parent: `https://apps.minisonmars.co.uk/privacy#toddler-parent`
- Toddler Doodle: `https://apps.minisonmars.co.uk/privacy#toddler-doodle`
- Toddler Camera: `https://apps.minisonmars.co.uk/privacy#toddler-camera`
- Caravan Leveller: `https://apps.minisonmars.co.uk/privacy#caravan-leveller`

When an app changes what it does with data, permissions or the network, update its section in `privacy.html` and the "Last updated" date.

## Hosting

Cloudflare Pages project connected to this repo, production branch `main`, no framework preset, no build command, output directory `/`. Every push to `main` goes live in about a minute. Custom domain `apps.minisonmars.co.uk` is added in the Pages project's Custom domains tab.
