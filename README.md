# Voxxo — Public Pages

Static GitHub Pages site for the Voxxo iOS app, hosting the legal and support pages required by the Apple App Store.

## Pages

| Path | Purpose |
|------|---------|
| `index.html` | Landing page that links to all sub-pages. |
| `privacy.html` | Privacy Policy (GDPR + Apple App Privacy aligned). |
| `terms.html` | Terms of Service (incl. auto-renewing subscription disclosure & EULA reference). |
| `support.html` | Support / FAQ — required as the App Store "Support URL". |
| `account-deletion.html` | Account & data deletion instructions — required by App Store guideline 5.1.1(v). |
| `404.html` | Friendly 404 fallback. |

## How to publish

1. Create a new public GitHub repository named `voxxo-app-github-page` under the `Lorem-Software` organisation.
2. Commit the contents of this folder to the repo's `main` branch.
3. In **Settings → Pages**, set the source to `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. Wait ~1 minute for the first deploy. Pages will be live at:

   ```
   https://lorem-software.github.io/voxxo-app-github-page/
   ```

5. Update the URLs in the iOS app (`src/config/legal.ts`) if you switch to a custom domain.

## App Store Connect — required URLs

When submitting Voxxo, paste these into App Store Connect:

- **Privacy Policy URL:** `https://lorem-software.github.io/voxxo-app-github-page/privacy.html`
- **Support URL:** `https://lorem-software.github.io/voxxo-app-github-page/support.html`
- **Marketing URL** (optional): `https://lorem-software.github.io/voxxo-app-github-page/`
- **EULA:** leave blank to use Apple's standard EULA — our Terms reference it explicitly.

## Owner / contact

Lorem Software · Mert Zeybek<br/>
Değirmendere, Kuşadası, Aydın, Türkiye<br/>
info@loremsoftware.com
