# CreatoVault — editable digital product library page

A complete static sales-page draft with original copy and a blue/white brand direction, based on the section flow of the reference supplied by Mohan. No reference creator photographs, assets, testimonials or code were copied.

## Current status

This is a product-preview draft. Product contents and the $19 / ₹999 prices are proposals, not approved live offers. Checkout is disabled. No payments, customer details or analytics are collected. There are no fabricated testimonials, sales counters, urgency deadlines or resale-rights promises.

## Edit the site

- `site-config.js`: brand, hero, proposed prices, resource previews, features, FAQs, policies and checkout links.
- `styles.css`: colors, fonts, spacing and responsive layouts.
- `index.html`: section structure and founder story.
- `assets/vault-mockup.webp`: original concept product image.
- `app.js`: filtering, accessible resource dialogs, FAQs, checkout selection and policy dialogs.

For full rebranding, also update the static footer, founder story, page description, favicon and no-JavaScript text in `index.html`. The primary brand color is configured in `site-config.js`; companion shades are in `styles.css`.

## Enable a real offer

1. Create and inspect the actual product files.
2. Replace preview concepts and compatibility disclaimers with verified deliverables.
3. Set final prices and licensed-use permissions.
4. Publish accurate privacy, terms and refund policies; update the related FAQs.
5. Enter your HTTPS purchase links under `checkout.indiaUrl` and `checkout.internationalUrl`.
6. Change `checkout.enabled` to `true`.
7. Update the preview labels and launch text throughout `index.html` and `site-config.js`.
8. Test both purchase paths and actual delivery with your provider.
9. Remove the `noindex,nofollow` meta tag when you want search engines to index the site.

The page does not deliver files or implement a payment processor. Those services belong to the configured checkout destination. Keep secrets and payment-provider API keys out of this public static repository.

## GitHub Pages

Live preview: https://mono444.github.io/creatovault-library/

Repository: https://github.com/Mono444/creatovault-library

Pages source is set to GitHub Actions. Pushes to `main` deploy automatically. The included workflow deploys only the public website assets and excludes the README and business plan.

No compilation is required. All asset links are relative, so GitHub project-site subpaths work without editing a base URL. External Google Fonts are optional; fallback fonts work without that request.

If editing locally, serve this folder with `python3 -m http.server 8000`, then open the local address on your own computer.

## Validation

JavaScript syntax, local asset references and configuration passed validation. Interactive logic passed isolated DOM checks for initial hydration, category filtering, preview dialogs, focus restoration, policy dialogs, disabled draft checkout and HTTPS-only live links. The GitHub Pages deployment succeeded. The live desktop page, original image, category filtering, resource preview and privacy dialogs, and disabled checkout notice were verified in a browser. No horizontal overflow was observed at the checked desktop width. Responsive CSS is included; a separate mobile browser visual inspection has not been completed.
