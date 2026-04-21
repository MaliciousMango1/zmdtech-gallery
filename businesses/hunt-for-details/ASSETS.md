# Hunt for Details — Asset Requirements

Placeholder photo blocks live throughout — home masthead is type-only (no photo by choice), portfolio is an all-placeholder grid, and the visit map is a grid-lines placeholder. Everything below is what the client needs to supply to finish the site.

## Photography

Create an `assets/` subfolder and drop the real images in.

### Priority 1 — Portfolio (`portfolio.html`)
The portfolio page is the single biggest visual lift. 12 placeholder tiles need real replacements.
- **`assets/portfolio/ceramic-porsche-911.jpg`** — Hero-width ceramic install on a 911, studio-lit. **Target:** 1600×1200px.
- **`assets/portfolio/correction-mustang.jpg`** — Two-stage correction on a black Mustang GT. Show reflection depth. **Target:** 1200×900px.
- **`assets/portfolio/interior-tahoe.jpg`** — Interior reset on a family SUV. **Target:** 1200×900px.
- **`assets/portfolio/ceramic-audi-rs5.jpg`** — Coated Nardo gray RS5. **Target:** 1200×900px.
- **`assets/portfolio/restoration-chevelle.jpg`** — '68 Chevelle show-prep detail. **Target:** 1200×900px.
- **`assets/portfolio/correction-bmw-m4.jpg`** — Swirl removal, wide shot. **Target:** 1400×900px.
- **`assets/portfolio/interior-f250.jpg`** — Work-truck carpet extraction, before/after fine. **Target:** 1400×900px.
- **`assets/portfolio/ceramic-model-y.jpg`** — Coated Model Y. **Target:** 1200×900px.
- **`assets/portfolio/restoration-jeep.jpg`** — Headlight/trim restoration on a Wrangler. **Target:** 1200×900px.
- **`assets/portfolio/interior-outback.jpg`** — Pet-hair interior reset. **Target:** 1200×900px.
- **`assets/portfolio/correction-c8.jpg`** — Corvette C8 correction + coating, hero width. **Target:** 1600×1200px.
- **`assets/portfolio/interior-highlander.jpg`** — Resale-prep interior. **Target:** 1200×900px.

### Priority 2 — Brand
- **`assets/logo.svg`** — Vector logo to replace the "Hunt. for Details" wordmark used in every header/footer. The dot accent is currently colored with CSS.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons.
- **`assets/owner-justin.jpg`** — A photo of Justin Hunt for a future About/owner section (not currently built but reserved).

### Priority 3 — Nice to have
- **`assets/studio-interior.jpg`** — Studio bay at 184 Collins Industrial Blvd, clean install environment.
- **`assets/process-coating.jpg`** — Ceramic application in progress. Useful for future process section.
- **`assets/process-polish.jpg`** — Machine polisher on a panel. Same.

## Maps

Placeholder is in `visit.html` (grid-lines block). Replace with a Google Maps iframe embed for **184 Collins Industrial Blvd, Suite H, Athens, GA 30601** with a service-radius overlay if possible.

## Forms

The quote request form on `index.html#quote` (and anchored from every nav) currently calls `alert()` on submit. Wire this to:
- Send to **hello@huntfordetails.com** (or confirmed owner email) with subject prefix `[Quote Request]`
- Include the uploaded photos as attachments — this is the whole point of the funnel
- Suggested backends: Cloudflare Pages Functions + Resend, Formspree (supports file upload on paid tier), or a Netlify form with file handling enabled

## Portfolio filters

The filter pills on `portfolio.html` (All / Ceramic / Correction / Interior / Restoration) are UI only — no filter JS is wired up. Either:
- Add a small JS filter on data-attributes, or
- Collapse to a single grid and drop the filters before launch

## Content to confirm with client

- **Founding year** — "Est. 2021" is what search results reported for the business starting under Justin Hunt. Used on brand subtitle in every header and footer. Confirm.
- **Phone** — `(770) 833-8102`. Confirmed from Yelp/BBB/Nextdoor listings.
- **Address** — `184 Collins Industrial Blvd, Suite H, Athens, GA 30601`. Confirmed from multiple directories.
- **Hours** — `Mon–Fri 9a–6p, closed Sat/Sun`. From Yahoo/BBB listings. Confirm.
- **Email** — we used `hello@huntfordetails.com` as a placeholder. The live site only exposes a contact form — no email address surfaces publicly. Get the correct one.
- **Owner** — Justin Hunt. Confirmed.
- **Mobile vs. studio split** — this site is framed as mobile-forward per the brief tagline ("Mobile Detailing · Est. 2021 · 100% Mobile" voice), but the live business actually operates by-appointment at a fixed studio per public listings. We split the difference: full details and washes come to you; ceramic and multi-stage correction are studio-based. **Confirm with Justin whether he actually wants to push a mobile offering or if the site should drop the mobile framing entirely.**
- **Starting prices** — the cascading services block shows:
  - Ceramic Coating from $900
  - Paint Correction from $600
  - Full Detail from $250
  - Interior Deep Clean from $200
  - Restoration / Add-ons from `$ —` (quoted)
  These are reasonable starting points for Athens-area pricing and match the "$150–$250 typical job" signal from reviews, but **none are on the live huntfordetails.com site**. Confirm every number before publishing.
- **Ceramic coating duration** — we said "3 to 5 year protection." Confirm which coating line Justin uses and the actual warranty period.
- **Certified installer** — trust band claims "Certified Coating Installer." Confirm which brand certification (Gtechniq, CQuartz, System X, etc.) and whether it can be displayed.
- **Insurance** — we claim "Fully Licensed & Insured." Confirm.
- **"1,200+ Vehicles Detailed"** — round-number trust stat. Get the actual figure.
- **Service area list** — Athens, Five Points, Watkinsville, Oconee County, Bogart, Bishop, Winterville, Statham, Winder, Commerce. Plausible for a Collins Industrial Blvd shop; confirm the real coverage radius.
- **Deposit policy** — we wrote "$100 deposit holds ceramic and multi-stage correction dates." Plausible industry-standard; confirm.

## Copy to double-check

Content was compiled from Google/Yelp/BBB/Nextdoor/Facebook search results referencing huntfordetails.com on 2026-04-20. The live site's contact form wall meant we could not pull exact service descriptions or current pricing — **every service description and price needs a pass from Justin before launch.**

## External links already wired

- **Official site** footer link → https://www.huntfordetails.com
- **Facebook** footer link → https://www.facebook.com/HuntforDetails/

Confirm both URLs are current.
