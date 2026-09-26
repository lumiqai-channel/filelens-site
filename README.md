# FileLens Website

Static verification/landing website for FileLens.

## Option A — GitHub Pages

1. Create a public repository, for example `filelens-site`.
2. Upload all files from this folder to the repository root.
3. In **Settings → Pages**, set **Source** to **GitHub Actions**.
4. Push to `main` (or run the included Pages workflow manually).
5. GitHub publishes the site at a URL such as:
   `https://<owner>.github.io/filelens-site/`

The included `.github/workflows/pages.yml` handles deployment.

## Option B — Cloudflare Pages

This same folder can be deployed as a static site.

### Direct Upload
1. In Cloudflare, go to **Workers & Pages**.
2. Create a Pages application using **Direct Upload**.
3. Upload this folder or the ZIP archive.
4. Choose a project name such as `filelens`.
5. Cloudflare provides a URL such as:
   `https://filelens.pages.dev`

No framework build command is required.

## Custom domain

A custom domain is optional. You can start with the free `github.io` or `pages.dev`
address and attach a custom domain later without redesigning the site.

## Stripe verification

Use the final public HTTPS URL in Stripe's **Business website** field.

The site contains:
- Public business name: FileLens
- Description of the downloadable Windows software
- $49 one-time FileLens Pro pricing
- Customer support contact
- Refund/dispute policy
- Privacy policy
- Terms/EULA

## Before public sales

- Replace the support email if desired.
- Wire the real checkout URL after Stripe Managed Payments is active.
- Replace the release-status note when FileLens 1.0 is available.
- Have the legal text reviewed if appropriate.
