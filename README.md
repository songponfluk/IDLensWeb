# IDlens website (GitHub Pages)

Static pages for the App Store listing: `index.html` (marketing), `support.html` (Support URL),
`privacy.html` (Privacy Policy URL) and `terms.html` (Terms of Use / EULA). No build step.

## Before publishing

Replace the placeholder email in all pages:

```bash
grep -rl "YOUR_EMAIL@example.com" docs | xargs sed -i '' 's/YOUR_EMAIL@example.com/you@yourdomain.com/g'
```

## Deploy

1. Create a public GitHub repository named `idlens` and push this project (or only the `docs/` folder).
2. GitHub → repository → **Settings › Pages** → Source: **Deploy from a branch** → Branch: `main`, folder: **/docs** → Save.
3. After about a minute the site is live at `https://<github-username>.github.io/idlens/`.

## URLs for App Store Connect

| Field | URL |
|---|---|
| Support URL | `https://<github-username>.github.io/idlens/support.html` |
| Marketing URL | `https://<github-username>.github.io/idlens/` |
| Privacy Policy URL | `https://<github-username>.github.io/idlens/privacy.html` |
| Terms of Use (in the app description) | `https://<github-username>.github.io/idlens/terms.html` |
