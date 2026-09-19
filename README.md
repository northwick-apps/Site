# Northwick – public site

Static public web pages for **Northwick**, a small independent studio publishing apps on the
[Atlassian Marketplace](https://marketplace.atlassian.com/). First app: **Review Due** for
Confluence Cloud (a Forge app: review dates, page owners, stale-page dashboard, reminders).

Plain HTML plus one CSS file. No framework, no build step, no analytics, no cookies.
Nothing private belongs in this repository.

## Live URLs

Published by GitHub Pages from the repository root on every push to `main`:

| Page | URL |
|------|-----|
| Home | <https://northwick-apps.github.io/Site/> |
| Privacy Policy | <https://northwick-apps.github.io/Site/privacy.html> |
| Terms of Use | <https://northwick-apps.github.io/Site/terms.html> |
| Support | <https://northwick-apps.github.io/Site/support.html> |

The Privacy, Terms and Support URLs are the ones to enter in the Marketplace listing.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Studio overview and list of apps |
| `privacy.html` | Privacy policy (covers Review Due and, by default, all Northwick apps) |
| `terms.html` | Terms of use / EULA for Marketplace apps |
| `support.html` | How to get help, what to include, response time, known issues |
| `404.html` | Not-found page (GitHub Pages serves it automatically) |
| `style.css` | The single stylesheet: system fonts, light and dark via `prefers-color-scheme` |
| `.github/workflows/pages.yml` | Deploys the repo root to GitHub Pages |

## Deployment

`.github/workflows/pages.yml` runs on every push to `main`. It uses
`actions/configure-pages@v5` with `enablement: true`, so GitHub Pages is switched on
automatically the first time the workflow runs; no manual settings change is needed.
If that step ever fails, open **Settings → Pages** in the repository and set **Source** to
**GitHub Actions**, then re-run the workflow.

## Editing

Edit the HTML files directly and push to `main`. Keep the effective date at the top of
`privacy.html` and `terms.html` current when their content changes.

## Known issues

Known issues with Northwick apps are tracked in this repository's
[GitHub Issues](https://github.com/northwick-apps/Site/issues).

## Contact

Northwick.apps@gmail.com
