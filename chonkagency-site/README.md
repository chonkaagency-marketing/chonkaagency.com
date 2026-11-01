# chonkagency.com

Chonka Agency website — a static, hand-coded one-pager. No build step, no framework, no dependencies: `index.html` + `img/`.

**Big ideas. Bigger strategy. No fluff.**

## Local preview

Open `index.html` in a browser, or:

```bash
npx serve .
```

## Deploy (Cloudflare Pages)

1. In the [Cloudflare dashboard](https://dash.cloudflare.com) → **Workers & Pages → Create → Pages → Connect to Git**, pick this repo.
2. Build settings: **no framework**, build command empty, output directory `/`.
3. Deploy — you'll get a `*.pages.dev` URL immediately.
4. **Custom domain:** in the Pages project → Custom domains → add `chonkagency.com` (and `www.chonkagency.com`). Cloudflare shows you the DNS records; update the domain's nameservers/records at GoDaddy as instructed. HTTPS is automatic.

Every push to `main` redeploys the site automatically.

## Before go-live (TODOs)

- **Contact + newsletter forms:** replace `YOUR-EMAIL-HERE` in `index.html` (two places) with the inbox that should receive enquiries, then submit each form once to confirm the FormSubmit activation email.
- **Social links:** add LinkedIn / Instagram URLs to the footer.
- **Favicon:** currently an inline "C" — drop in a real logo file if preferred.
