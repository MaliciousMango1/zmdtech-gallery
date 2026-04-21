# LMM Detailing Services — Asset & Content Requirements

Content was extracted from the live Wix site (`lmmdetailingsvcs.com`), Google/Yelp listings, and reviews on 2026-04-20. Prices and packages below flag anything that was inferred rather than lifted verbatim so the client can confirm before going live.

---

## Photography

All placeholders on the site are styled `<div>` blocks on a dark diagonal-stripe base. Each carries a `data-label="PHOTO — ..."` attribute explaining what belongs there. Swap them with real images in a new `assets/` subfolder once we have them.

### Priority 1 — Home (`index.html`)

The homepage was rebuilt around a configurator-style layout — no traditional hero photo block. It now uses four stylized "before/after" slash tiles instead of a photo gallery. When real photography is available, swap the CSS slash blocks for real paired images.

- **`assets/compare-paint-correction.jpg`** (and `-before.jpg` / `-after.jpg` pair) — Close swirl/scratch panel before correction, paired with a corrected mirror-finish panel. Diagonal composite preferred, 1:1 aspect ratio. **Target:** 1000×1000px per side.
- **`assets/compare-ceramic-coating.jpg`** — Bead/sheeting shot after coating, paired with a non-beading panel before. 1:1. **Target:** 1000×1000px per side.
- **`assets/compare-interior-deep-clean.jpg`** — Stained carpet / seat before, clean after. Close, well-lit. 1:1. **Target:** 1000×1000px per side.
- **`assets/compare-wheel-restoration.jpg`** — Brake-dust-caked wheel before, polished restored wheel after. 1:1. **Target:** 1000×1000px per side.

> Currently these four slots on the home page are **CSS-only placeholders** — diagonal-split panels with "Before" / "After" tag pills. They are not photos. Replacing them with actual before/after images is a priority for launch.

### Priority 1b — Supporting photos (carried over from earlier home layout, still useful)
- **`assets/hero-vehicle.jpg`** — The flagship photo. Low 3/4 angle, deep black or dark-colored vehicle, fresh ceramic reflection. **Not currently used** — the rebuilt homepage hero is typographic (no photo). Keep on hand for future landing-page variations or for the top of services.html.
- **`assets/sig-exterior.jpg`** — Close-up of hand-wash or wheel/tire detail. Soap suds, brush, or drying towel visible. **Target:** 1200×900px.
- **`assets/sig-interior.jpg`** — Steam-cleaning or extraction shot. Blue steam, a vacuum, or an extractor wand in action. **Target:** 1200×900px.
- **`assets/sig-ceramic.jpg`** — Ceramic coating being applied (applicator block on paint) OR a beading shot. **Target:** 1200×900px.
- **`assets/owner-at-work.jpg`** — Larry mid-detail. Polisher in hand, or bent over a fender buffing. Candid, unposed. **Target:** 1200×1440px.

### Priority 2 — Services &amp; Packages pages
- **Before/after gallery** — If Larry has before/after pairs from jobs (pet hair, paint correction, waterspots), they would slot in nicely as an optional gallery section we can add. Ask if he has an Instagram/phone library of these.
- **Ceramic tier hero** — A beading or sheeting shot we can use as the visual anchor for the ceramic coating section.

### Priority 3 — Nice to have
- **`assets/logo.svg`** — A proper vector logo to replace the text wordmark in the header (`/LMM Detailing`). Current favicons were carried over from the placeholder build and should also be replaced.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons.

---

## Maps

The Visit page has a map placeholder block. Replace with a Google Maps embed:

```html
<iframe
  src="https://www.google.com/maps/embed?pb=..."
  width="100%" height="100%" style="border:0;"
  allowfullscreen loading="lazy"
  referrerpolicy="no-referrer-when-downgrade"></iframe>
```

Get the embed code from **[Google Maps → Share → Embed a map]** for **163 Westchester Cir, Athens, GA 30601**.

> Note: a secondary address surfaces in directories — **1290 Oconee St, Athens, GA 30605** (per Nicelocal, FindOpen). Confirm with client which is current so we use the right one on the site and map.

---

## Quote form wiring

The quote form on `visit.html#quote` currently calls `alert()` on submit and clears the fields — same pattern as Bee's Knees `cakes.html`. To go live it needs:

- **Form backend** — options: Formspree, Web3Forms, Netlify Forms, or wire directly to a business email via a serverless endpoint. Pick based on where the site is hosted.
- **Destination email** — **not shown on the live site.** Need Larry to confirm a business email address (e.g. `larry@lmmdetailingsvcs.com` or similar). Without one, the contact form has nowhere to go — fall back to `sms:` / `tel:` only.
- **Photo upload field** — the current form asks for notes but not photos. If desired, swap the notes field for a multi-file image input; most form backends support attachments for a small fee.
- **SMS notification** — optional: Twilio/ClickSend integration so quote requests trigger an SMS to Larry's cell in addition to email.

---

## Content gaps to confirm with client

### Pricing & packages
- **Ceramic tier prices** (`$1,575` / `$2,050` / `$2,500` for 3 / 5 / 10 year) — **verified from directory listings** referencing the live site. Confirm current pricing is still accurate.
- **The Show Package** — confirmed from live site at **from $95, ~4 hours**. The inclusions listed (two-bucket wash, wheels, tires, jambs, glass, spray wax) are **inferred from standard industry scope for an exterior-only detail at that price point**. Client to confirm what actually goes in The Show.
- **LMM's Best Package** — confirmed as a live package on the site. Starting price `$265` and the included items (correction, sealant, steam interior, leather) are **inferred tiering**. Client to confirm exact inclusions and price.
- **"The Reset" (Tier 03)** — **invented package name and scope.** Built from the extensive à la carte list the site mentions (paint correction, waterspot removal, mold/mildew, pet hair, engine bay, undercarriage, headlights). If Larry offers a "top tier" full-restoration package under a different name or pricing, swap it in.
- **À la carte service menu prices** — individual service prices (wash $65, clay+polish $185, single-stage correction $325, etc.) are **reasonable market rates for Athens, GA mobile detailing** but **were not explicitly listed on the live site**. Every price on `services.html` needs Larry's sign-off before this site goes live.
- **Student / military discounts** — referenced on the live site ("discounts and student discounts"). Military added by inference; confirm.

### Business details
- **Owner first name** — reviews reference "Larry". LinkedIn surfaces "Larry Magers, owner, LMM Enterprise". Confirm full name spelling and whether he wants it on the site (currently mentioned by first name only in one place).
- **Business address** — primary is **163 Westchester Cir, Athens, GA 30601** (Yelp, autoinclude, Roadtrippers). Alternate address **1290 Oconee St, Athens, GA 30605** surfaces in other directories. Which is the current base of operations?
- **Hours** — currently listed as Mon–Fri 8a–9:30p, Sat 6a–9:30p, Sun 9a–7:30p. These are late-night hours; confirm they're actually when Larry takes appointments vs. when he answers the phone.
- **Service area radius** — described as "Athens and surrounding counties." Confirm specific counties or a mileage radius (Clarke, Oconee, Madison, Jackson, Barrow, Oglethorpe?) so we can list them explicitly on the Visit page.
- **Social media** — no Instagram or Facebook surfaced in search. If Larry has active accounts, add them to the footer Follow column (they're currently only linking back to the official site and a phone link).
- **Email address** — not public. See quote form wiring note above.

### Testimonials
- The Google review quoted on the home page (`"My 15-year-old vehicle looked brand new when Larry was done..."`) is **paraphrased** from multiple similar 5-star reviews that mention the same themes (15-year-old vehicle, Larry by name, attention to detail). If Larry has specific permission-cleared quotes from named customers, swap them in verbatim.

---

## Copy to double-check

Before going live, confirm with the client:
- All service prices on `services.html`
- All three package inclusions on `packages.html`
- Ceramic coating tier prices
- Hours of operation
- Address (primary)
- Owner name spelling
- Whether the "Reset" name stays or gets replaced
