# jtwox.github.io

The JtwoX website, served by GitHub Pages at <https://jtwox.github.io/>.
Plain HTML and one stylesheet — no build step, no dependencies.

## Why this repo is public

GitHub Pages cannot serve from a private repo without a paid plan. Nothing
proprietary lives here: only the public-facing pages below. The Galilee
application source stays in its own private repo.

## Pages

| Path | Purpose |
|---|---|
| `/` | JtwoX landing |
| `/galilee/` | About Galilee |
| `/galilee/privacy/` | Privacy Policy — **required** by App Store Connect and Play Console |
| `/galilee/support/` | Support page — **required** as the listing's Support URL |

## Not yet published

`/galilee/terms/` is written but held back until the governing-law
jurisdiction is decided. Publishing it before then would put a visible
placeholder on a public page.

## Custom domain

To serve from `jtwox.com` instead:

1. Add a `CNAME` file at the repo root containing the domain.
2. At your DNS provider, point the domain at GitHub Pages — an `ALIAS`/`A`
   record at the apex, or a `CNAME` record for a subdomain pointing to
   `jtwox.github.io`.
3. Settings → Pages → Custom domain, then tick **Enforce HTTPS** once the
   certificate is issued.

Paths do not change, so the store listings only need the host swapped.

## Keeping the text honest

These pages describe what Galilee actually does: no accounts, no analytics,
no network calls, all data on-device. If that ever stops being true — a sync
feature, crash reporting, any telemetry — the Privacy Policy here and the App
Privacy declaration in App Store Connect must be updated in the same release.
