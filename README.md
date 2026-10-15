# TxB Technologies website

A responsive, photo-led multi-page website for GitHub Pages or another static host. Original TxB-themed commercial visuals are in `assets/txb-fleet-hero.png`, `assets/txb-installation.png`, and `assets/txb-fleet-monitoring.png`.

## Pages

- `index.html` — Home
- `services.html` — Service capabilities
- `about.html` — Company story with proposed motto, vision, mission and values
- `shop.html` — Quote-based tracker catalog with search and category filters
- `contact.html` — Quote request form
- `faq.html` — Common questions
- `privacy.html` — Draft privacy notice (review before publishing)

## Before launch

1. Open `assets/config.js` and verify the quote inbox, company name, phone and service location. The current email came from the supplied site and has not been confirmed.
2. The quote form is static and opens a prefilled email draft. It does not send or store submissions on its own. For direct server-side submissions, connect a form backend and update the privacy wording.
3. The shop is a product catalog with quote requests, not a payment checkout. Confirm stock, reseller status, product variants, local regulatory requirements, mobile-network bands and prices before advertising or accepting orders.
4. The homepage satellite map and moving marker are a demo route around Kampala, not real tracking data. Map imagery requires an internet connection and is served by Esri. Google Fonts, Leaflet and Material Design Icons also load from external CDNs.
5. Review the proposed About-page copy and draft privacy notice with TxB before launch. Add the company’s verified history, support hours and certifications only when confirmed.

## Add or edit products

Edit `assets/products.js`. Add another object to `window.TXB_PRODUCTS` with these fields: `id`, `name`, `brand`, `category`, `summary`, `highlights` (array), `bestFor`, and `manufacturerUrl`. The catalog builds cards and filters from this list.

## Deploy with GitHub Pages

1. Extract the website package.
2. Copy the **contents of the `txb-website` folder** into the root of the GitHub repository serving the site. Keep `assets` alongside `index.html`.
3. Commit and push the files, then configure GitHub Pages to deploy from the repository root (or the `main` branch root, depending on repository settings).
4. Open the published URL and check navigation, quote handoff and map loading over HTTPS.

Product references point to manufacturer pages. Product artwork is illustrative and does not claim to depict the exact unit. Features, regional variants and availability can change; confirm details at quote time.



Branding: The supplied TxB logo is used in the shared headers and footers. Shared CSS colors follow the orange, green, and charcoal palette in the logo. Replace ssets/txb-logo.png to update the logo sitewide.
