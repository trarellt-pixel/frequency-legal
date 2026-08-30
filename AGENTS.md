# Frequency legal pages

Public HTTPS pages for the Frequency iOS app (App Store Connect privacy, terms, and support). See `README.md` for the live GitHub Pages URLs.

## Cursor Cloud specific instructions

This repository is static HTML/CSS only. There is no package manager, lockfile, linter, test runner, or application backend. Future agents should treat Frequency legal pages as the whole product in this repo — not an iOS app workspace.

### Run the Frequency site locally

From the repository root:

```bash
python3 -m http.server 8000
```

Then open:

- Home: `http://localhost:8000/`
- Privacy Policy: `http://localhost:8000/privacy.html`
- Terms of Use (EULA): `http://localhost:8000/terms.html`
- App Support: `http://localhost:8000/support.html`

Pretty paths (`/privacy/`, `/terms/`, `/support/`, `/eula/`) are directory indexes and also return 200.

If port 8000 is already bound, reuse that server instead of starting a second one.

### Lint, test, and build

None are defined. Validate by loading the four Frequency pages and confirming:

- Branding is Frequency (not another app)
- Support inbox is `getfrequency.help@gmail.com`
- Subscription copy lists Frequency Monthly ($14.99) and Frequency Annual ($59.99)
- App Store Connect URLs in `README.md` match the served files
