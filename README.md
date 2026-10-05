# StogieLog Website

This repository contains the official public-facing website for **StogieLog**, a
social cigar journal and rating app for iOS. The site is used to introduce the
app, and to host the Privacy Policy, Terms of Use, and Support pages required
for the Apple App Store listing.

Live domain: [https://stogielog.app](https://stogielog.app)

## About This Site

This is a **simple static website** — plain HTML, CSS, and minimal vanilla
JavaScript only. There is no JavaScript framework (no React, Next.js, Vue,
Angular, etc.), no npm dependencies, and no build step. The files in this
repository can be served directly by any static file host or web server.

## Pages

| File           | Description                                                        |
|----------------|---------------------------------------------------------------------|
| `index.html`   | Landing page introducing StogieLog and its core features, with a call-to-action for the iOS app. |
| `privacy.html` | Privacy Policy covering data collection, use, storage, sharing, and user rights. |
| `terms.html`   | Terms of Use covering account responsibilities, acceptable use, content, and subscriptions. |
| `support.html` | Support page with contact addresses for general help, bugs, suggestions, security, privacy, and abuse reports. |
| `styles.css`   | Shared stylesheet providing the site's dark, sophisticated visual design and responsive layout. |

All pages share the same header navigation and footer for consistency.

## Local Testing

No build tools or package installation are required. To preview the site
locally, serve the folder with any simple static file server, for example:

```bash
# Python 3
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) in your browser.
Alternatively, you can open `index.html` directly in a browser, though some
relative-link behavior is best verified via a local server.

## Deployment

This site is a static site and can be deployed to any static hosting provider
that serves plain files, such as GitHub Pages, Netlify, Vercel (static mode),
or Cloudflare Pages. Deployment generally only requires pointing the host at
the repository root — no build command is necessary.

When deploying:

1. Confirm the custom domain is configured to `https://stogielog.app`.
2. Confirm HTTPS is enabled.
3. Update the App Store link placeholder in `index.html` once the app is live
   on the Apple App Store.
4. Update the effective date placeholders in `privacy.html` and `terms.html`
   when those documents are finalized or revised.

## Notes

- This repository contains no secrets, API keys, or credentials.
- No analytics, tracking, advertising, or third-party scripts are included.
