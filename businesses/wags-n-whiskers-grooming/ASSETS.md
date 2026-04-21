# Wags 'N' Whiskers Grooming — Asset Requirements

Placeholder photo blocks, a map placeholder, and a home-visit request form stub throughout. Here's what we need from the client.

## Photography

Replace each placeholder block with a real image in a new `assets/` subfolder.

### Priority 1 — Home Visits (`home-visits.html`)
- **`assets/home-setup.jpg`** — A real home grooming setup: portable table on a porch or in a garage, dog being toweled off, natural light. This image carries the differentiator of the whole site. **Target:** 1000x1250px, portrait.

### Priority 2 — Home (`index.html`)
- No photos on the homepage right now by design (the layout is text-first and uses a stylized map radius graphic). If the client wants a hero image later, we'd add it above the visit-type selector as a single landscape band. **Target:** 1600x900px.

### Priority 3 — Nice to have
- **`assets/groomer-portrait.jpg`** — Portrait of the groomer at a table with a calm dog. For a future About section. **Target:** 1000x1250px.
- **`assets/shop-interior.jpg`** — Interior of the small shop space in Athens — shows the "family home setting" claim. **Target:** 1200x900px.
- **`assets/pet-gallery/`** — 6–10 before/after shots (small, medium, large, long-coat breeds). Client-owned dogs only, with owner permission.
- **`assets/logo.svg`** — Proper vector wordmark to replace the Petrona type-based brand lockup.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons.

## Maps

Two placeholders to replace:
- `index.html` — stylized service-radius graphic. Replace with either a static SVG of the radius around Athens or a Google Maps static-map image styled to fit the palette.
- `visit.html` — small map block. Replace with a Google Maps iframe embed once the street address is confirmed (see below).

## Forms

The home-visit request form on `home-visits.html#book` currently triggers `alert()` on submit. Wire to send to **hello@wagsnwhiskersgrooming.com** with subject prefix `[Home Visit Request]` via Cloudflare Pages Functions + an email backend (Resend, Postmark), Formspree, or a Google Form embed.

## Content to confirm with client

- **Exact street address** — the live site does not publish a street address. We've used "Athens, GA" as the visible location and noted on Visit that the exact address is shared on booking. Confirm whether they want a public address or to keep it by-appointment-only.
- **Phone** — we used **(706) 255-5191** (sourced from the Wags 'N' Whiskers in-home petsitting Facebook page, which appears to be the same operator). Confirm this is the correct number for grooming inquiries.
- **Email** — we used **hello@wagsnwhiskersgrooming.com** as a placeholder. Confirm the real inbox. The live site does not publish one.
- **Service area pill list** — we listed Athens, Five Points, Normaltown, Boulevard, Cedar Shoals, Eastside, Watkinsville, Bogart, Bishop, Winterville, and Oconee County. Confirm and correct — especially whether they travel as far as Winder, Jefferson, Commerce, or Madison.
- **Groomer name(s) / team** — not surfaced on the live site. Ask if they want the groomer credited on Home or a future About page.
- **Hours** — we used Mon 8:30–7, Tue–Wed 8–7, Thu 8–5, Fri 8–4, Sat 8–3, Sun closed (sourced from search snippets citing the live site). Confirm. Also confirm whether those are shop hours, home-visit hours, or both.
- **All grooming prices** — every `$ —` cell on `services.html` is intentional. A sister salon (Moorhead, MN) publishes Small $70–80 / Medium $85+ / Large $125–135+ / XL $150+ for full grooms; do not copy those numbers to Athens without confirmation.
- **Long-coat modifier** — we listed a flat coat fee for doodles/retrievers/shepherds. Confirm this exists and the amount.
- **Travel fee** — we reference a small travel fee for home visits outside central Athens. Confirm amount and radius.
- **Puppy / senior / cat groom offerings** — we listed these on services.html as plausible defaults. Confirm they actually offer each.
- **Vaccine requirements** — we said "rabies required" on visit.html. Confirm full vaccine policy (Bordetella? DHPP?).
- **Payment methods** — we listed card, cash, Venmo. Confirm.
- **"Insured. Experienced. Patient with anxious pets." trust line** — confirm each claim is accurate before publishing.
- **Pet Care Campus tag** — used in the brand sub-line across header and footer. Confirm this is current business language.

## Copy to double-check

Content was extracted from wagsnwhiskersgrooming.com, the Wags 'N' Whiskers in-home petsitting Facebook page, and general Athens-area search results on 2026-04-20. Before going live:
- Confirm the business is still operating and that the home-visit offering is still active
- Confirm address handling (public vs by-appointment)
- Confirm phone, email, and hours
- Confirm service area
- Fill in all `$ —` prices on `services.html`
