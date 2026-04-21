# Porterhouse Grill — Asset Requirements

Placeholder photo blocks, a map placeholder, and an inquiry form stub throughout. Here's what we need from the client.

## Photography

Replace each placeholder block with a real image in a new `assets/` subfolder.

### Priority 1 — Home (`index.html`)
- **`assets/hero-porterhouse.jpg`** — Hero shot of the signature Porterhouse steak on plate with sautéed mushrooms, moody low-light styling. **Target:** 1200×1500px, portrait.
- **`assets/feature-porterhouse.jpg`** — Tighter crop of the Porterhouse for the signature card. **Target:** 1000×750px.
- **`assets/feature-crabcakes.jpg`** — Jumbo lump crab cakes with scallion aioli. **Target:** 1000×750px.
- **`assets/feature-saltimbocca.jpg`** — Chicken saltimbocca plated. **Target:** 1000×750px.
- **`assets/dining-room.jpg`** — Dining room at dusk, low light, occupied tables (or empty if privacy is a concern). Shows ambiance. **Target:** 1000×1250px.

### Priority 2 — Private Dining (`private-dining.html`)
- **`assets/private-room.jpg`** — Private dining room set for a group. Shows the room without identifying guests. **Target:** 1000×1250px.

### Priority 3 — Nice to have
- **`assets/menu-detail/`** — 4–6 plated food shots for a future gallery section (desserts, starters, wine pours, etc.).
- **`assets/exterior.jpg`** — Evening exterior shot of the East Broad Street storefront.
- **`assets/logo.svg`** — Proper vector logo to replace the Cormorant Garamond wordmark.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons.

## Maps

Placeholder is in `visit.html`. Replace with a Google Maps iframe embed for **459 E Broad St, Athens, GA 30601**.

## Forms

The private dining inquiry form on `private-dining.html#inquire` currently triggers `alert()` on submit. Wire to send to **contactus@porterhousegrillathens.com** with subject prefix `[Private Dining Inquiry]` via Cloudflare Pages Functions + an email backend (Resend, Postmark), Formspree, or a Google Form embed.

## External integrations (already linked, just confirm)

- **Resy** reservations: https://resy.com/cities/athens-ga/venues/porterhouse-grill
- **OrderBulldawgFood.com** for online ordering

Confirm both URLs are current and active.

## Content to confirm with client

- **Founding year** — "Since 1997" is a reasonable guess; confirm the actual founding year. Used on brand subtitle in every header and footer.
- **Owner / chef names** — not on the live site. Ask if they want to credit a chef or owner on the About/Home page.
- **Menu accuracy** — full menu was extracted from allmenus.com. Some prices may be out of date; confirm against their current printed menu. Also add/remove items as needed (seasonal specials, wine list).
- **Wine list + cocktail menu** — not on the live site in any browsable format. If the client wants these featured on the site, we need the PDFs or list.
- **Hours** — we used live-site hours (Mon–Tue 5–9, Wed 4–9, Fri–Sat 11–10, Sun brunch 11–3, Sun dinner 4–8). Thursday is listed as closed. Confirm.
- **Valet service claim** — we wrote "complimentary valet on Friday and Saturday evenings" in Visit. Confirm whether Porterhouse actually offers this or remove.
- **Private dining capacity** — we said "12 to 40" and "60 or more for buy-outs." These are plausible for a downtown steakhouse but should be confirmed with actual room dimensions.
- **Catering scope** — mentioned catering but no specifics. Confirm they actively do this and what the minimum order is.
- **Julia Child quote** — used verbatim from the live site. Assume permission is fine; confirm.
- **"Three decades" claim** — we said "almost three decades" on the private dining page; this tracks with a 1997 opening as of 2026. Confirm founding year.

## Copy to double-check

Content was extracted from porterhousegrillathens.com and allmenus.com on 2026-04-20. Before going live:
- Confirm address: 459 E Broad St, Athens, GA 30601
- Confirm phone: (706) 369-0990
- Confirm email: contactus@porterhousegrillathens.com
- Confirm every menu item and price on `menu.html`
