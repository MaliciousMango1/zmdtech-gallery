# Barbers & the Salon — Asset Requirements

Placeholder portrait blocks on `team.html` and map placeholders on `visit.html`. The homepage chooser hero is pure type — no photo dependency — but photography will strengthen the team and visit pages significantly. Here's what we need from the client.

## Photography

Replace each placeholder block with a real image in a new `assets/` subfolder.

### Priority 1 — Team (`team.html`)

Each barber/stylist needs a simple vertical portrait in front of their chair or a clean neutral wall. Consistent framing across both locations.

- **`assets/team/william.jpg`** — Co-owner, Alps. **Target:** 900×1200px.
- **`assets/team/matt.jpg`** — Master barber, Alps. **Target:** 900×1200px.
- **`assets/team/angie.jpg`** — Barber/stylist, Alps. **Target:** 900×1200px.
- **`assets/team/mary.jpg`** — Stylist, Alps. **Target:** 900×1200px.
- **`assets/team/hannah-j.jpg`** — Stylist, Epps Bridge. **Target:** 900×1200px.
- **`assets/team/hannah-c.jpg`** — Stylist, Epps Bridge. **Target:** 900×1200px.
- **`assets/team/grace.jpg`** — Stylist, Epps Bridge. **Target:** 900×1200px.
- **`assets/team/kinzy.jpg`** — Stylist, Epps Bridge. **Target:** 900×1200px.
- **`assets/team/michelle.jpg`** — Stylist, Epps Bridge. **Target:** 900×1200px.

Team list is assembled from public sources (Facebook, Yelp, directory pages). Final roster, spelling, and role titles need client confirmation before shoot.

### Priority 2 — Location identity (optional on current layout)

The homepage hero is type-only by design. These aren't required by the current layout but would work well if we add a future location-detail page or convert one of the panels into a background image version.

- **`assets/alps-interior.jpg`** — Barber chairs at Alps, warm morning light. **Target:** 1600×1000px.
- **`assets/epps-interior.jpg`** — Salon chairs / color station at Epps Bridge. **Target:** 1600×1000px.
- **`assets/alps-exterior.jpg`** — Storefront from the Alps Shopping Center lot. **Target:** 1600×1000px.
- **`assets/epps-exterior.jpg`** — Storefront on Epps Bridge Pkwy. **Target:** 1600×1000px.

### Priority 3 — Brand

- **`assets/logo.svg`** — Proper vector wordmark to replace the Alegreya-set "Barbers & the Salon" text lockup.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons.

## Maps

Placeholders are on `visit.html` (two of them). Replace with Google Maps iframe embeds for:
- **Alps**: 1310 Baxter St, Athens, GA 30606
- **Epps Bridge**: 1880 Epps Bridge Pkwy #111, Athens, GA 30606

## External integrations (already linked, confirm)

- **Fresha — Epps Bridge**: https://www.fresha.com/lvp/barbers-and-the-salon-epps-bridge-parkway-athens-QvwGMg
- **Fresha — Alps**: https://www.fresha.com/lvp/alps-barbers-the-salon-baxter-street-athens-2G0JV0

The primary "Book" CTA across all pages currently points to the Epps Bridge Fresha page, since the Fresha listing for Alps is sometimes branded "Alps Barbers & The Salon." Confirm the client wants a single unified booking URL, a location picker in the nav, or per-location routing (as on the panels on `index.html` and `visit.html`).

## Content to confirm with client

- **Pricing** — All service prices are shown as `$ —` placeholders. The live site does not publish prices and Fresha pricing varies by stylist. We need the current service menu with starting prices (or a clear "set at the chair" note) before publishing.
- **Founding year** — "Since 1969" used in footers, based on a public mention that the shop has been part of the community since 1969. Confirm; adjust to the true founding year if different.
- **Tagline** — We used "Sharp cuts, honest prices, two chairs worth sitting in." as the footer tagline per the agreed voice direction. Client should sign off on this as the public tagline.
- **Staff roster** — Names on `team.html` (William, Matt, Angie, Mary, Hannah J., Hannah C., Grace, Kinzy, Michelle) are drawn from public directories and Facebook. Confirm spelling, location assignments, current employment, roles, and bios. Remove anyone who is no longer with the shop and add anyone missing.
- **Service menu completeness** — The full list on `services.html` is an educated composite for a barber+salon (cuts, shave, beard work, color, highlights, balayage, blowout, brows, deep conditioning). Confirm against the client's current internal price sheet. Add/remove items.
- **Hours** — We used hours consistent with current directory listings:
  - Alps: Mon/Tue/Thu/Fri 8:30–6, Wed 8:30–5, Sat 8:30–3, Sun closed.
  - Epps Bridge: Mon/Tue/Thu/Fri 9–6, Wed 9–5, Sat 9–3, Sun closed.
  Confirm current hours at both locations, especially holiday variations and UGA home-game Saturdays.
- **Phone numbers** — Alps: (706) 354-0360. Epps Bridge: (706) 354-0316. Confirm both are the live shop lines (not the owner's mobile).
- **Parking** — "Free lot parking" (Alps) and "Free surface parking" (Epps Bridge) are assumptions based on typical shopping-center setups. Confirm or edit.
- **"What's here" differentiation** — We positioned Alps as barber-forward (hot shave, beard work, kids) and Epps Bridge as salon-leaning (color, blowouts, styling). Both locations actually do both; this framing sharpens the location-chooser pitch. Confirm the client is comfortable with this split, or adjust to "same service menu, same team rotation at both."
- **Social links** — Facebook pages exist separately per location (`EppsBarbersAndSalon` and `barbersandsalon`). No site links are wired yet. Decide whether to show one, both, or neither in the footer.

## Copy to double-check

Content was composed and extracted from public sources (live site `barbersandthesalon.com`, Yelp, Fresha, Facebook, directory listings) on 2026-04-20. Before going live, confirm every name, phone, address, hour, and service against the client's current records.
