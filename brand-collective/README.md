# Brand Collective Studio legal and support pages

Public HTTPS pages for Brand Collective Studio (shown in the UI as **The Brand Collective**), a Mac App Store app from Fortress Technologies.

These pages live in a subdirectory of the Frequency GitHub Pages site because a separate `brand-collective-legal` repo could not be created from this agent. Frequency pages and Frequency emails are unchanged.

Live GitHub Pages URLs:

- https://trarellt-pixel.github.io/frequency-legal/brand-collective/privacy.html
- https://trarellt-pixel.github.io/frequency-legal/brand-collective/terms.html
- https://trarellt-pixel.github.io/frequency-legal/brand-collective/support.html

Privacy and Terms also already exist on Railway. App Store Connect can use either for those two. Railway `/legal/support` is a client 404 — use the Pages Support URL below.

## Paste these URLs into App Store Connect

| App Store Connect field | Working URL (GitHub Pages) | Also live on Railway |
| --- | --- | --- |
| Privacy Policy URL (App Privacy + app version) | https://trarellt-pixel.github.io/frequency-legal/brand-collective/privacy.html | https://brandcollectivemedia-production.up.railway.app/legal/privacy |
| Terms of Use / EULA (app description and/or License Agreement) | https://trarellt-pixel.github.io/frequency-legal/brand-collective/terms.html | https://brandcollectivemedia-production.up.railway.app/legal/terms |
| Support URL | https://trarellt-pixel.github.io/frequency-legal/brand-collective/support.html | Not published (`/legal/support` 404s) |
| Optional Apple Standard EULA | https://www.apple.com/legal/internet-services/itunes/dev/stdeula/ | — |

Also add both links in the **app description**, for example:

```
Privacy Policy: https://trarellt-pixel.github.io/frequency-legal/brand-collective/privacy.html
Terms of Use (EULA): https://trarellt-pixel.github.io/frequency-legal/brand-collective/terms.html
```

Support email (from the live Railway privacy and terms pages): `support@brandcollectivemedia.com`

If App Store Connect asks for a custom license agreement as plain text, paste the contents of `eula.txt`.

## Product reference (not for the App Store listing)

| Field | Value |
| --- | --- |
| Product name in UI | The Brand Collective |
| Product | Brand Collective Studio |
| Company | Fortress Technologies |
| Bundle ID | com.fortresstechnologies.brandcollectivestudio |
| Apple Team | FJ33KW7YNH |
| App Store Connect Apple ID | 6806247366 |
| Live origin | https://brandcollectivemedia-production.up.railway.app |

Do not use brandcollectivemedia.com as the Support URL. That custom domain is not live. Do not use the Railway `/legal/support` path.
