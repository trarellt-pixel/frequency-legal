# Frequency legal and support pages

Public HTTPS pages for the Frequency iOS app in App Store Connect.

Live site: https://trarellt-pixel.github.io/frequency-legal/

## Paste these URLs into App Store Connect

Do not use `https://fortresstechnologies.com` for these fields. That domain currently returns 404, which makes App Store Connect mark the Privacy Policy, Support, and Marketing URL items as failed.

| App Store Connect field | Working URL |
| --- | --- |
| Privacy Policy URL (App Privacy + app version) | https://trarellt-pixel.github.io/frequency-legal/privacy.html |
| Terms of Use / EULA (app description and/or License Agreement) | https://trarellt-pixel.github.io/frequency-legal/terms.html |
| Support URL | https://trarellt-pixel.github.io/frequency-legal/support.html |
| Optional Apple Standard EULA | https://www.apple.com/legal/internet-services/itunes/dev/stdeula/ |

Also add both links in the **app description**, for example:

```
Privacy Policy: https://trarellt-pixel.github.io/frequency-legal/privacy.html
Terms of Use (EULA): https://trarellt-pixel.github.io/frequency-legal/terms.html
```

Frequency support email (use this, not a Fortress address): `frequencyapp.support@gmail.com`

If App Store Connect asks for a custom license agreement as plain text, paste the contents of `eula.txt`.

## Why items show Failed or Rejected

Apple flags metadata when a required URL is missing, 404, or is not clearly a privacy / terms / support page. Common Frequency misses:

1. Support URL 404 — `/support` did not exist before this update.
2. Company homepage 404 — `fortresstechnologies.com` is up as a host but has no pages.
3. Terms of Use (EULA) missing from the **app description** even when a privacy URL is filled in.
4. In-app purchase / subscription products stuck on **Missing Metadata** or **Developer Action Needed** (review screenshot, localized display name, or subscription-group localization).
5. Guideline 3.1.2 — Privacy and Terms links missing **inside the iOS app** (paywall or settings). This repo cannot add those in-app buttons.

## After you update the URLs

1. Wait for GitHub Pages to rebuild this branch/main.
2. Open each URL in a private browser window and confirm it loads.
3. In App Store Connect, replace any `fortresstechnologies.com` or GitHub repo links with the table above.
4. Save the app version, then check that Privacy Policy, Support URL, and subscription items no longer show a red failed state.
