# Thyme to Cater Bistro — Asset Requirements

A photo-light design by choice — the homepage leans on typography and the award pill rather than a hero photo. A few placeholder regions and unconfirmed copy still need a client pass.

## Photography

No hero photo is required. The design is intentionally type-led. If the client wants imagery, consider adding an optional photo strip between the lunch preview and the slab list.

### Nice to have (for a future revision)
- **`assets/bistro-exterior.jpg`** — Storefront at 960 Lee Street, ideally late-morning light. **Target:** 1600×900px.
- **`assets/chef-keith.jpg`** — Portrait of Chef Keith Mosser in the kitchen. For a potential About block on the catering page. **Target:** 1000×1250px.
- **`assets/event-wide.jpg`** — Wide shot of a recent plated wedding or dinner event (guests blurred or absent). For a potential catering-page header. **Target:** 1600×900px.
- **`assets/pastry-case.jpg`** — Close-up of the pastry case, morning light. **Target:** 1000×750px.
- **`assets/logo.svg`** and **`assets/favicon.svg`** — Vector logo and favicons. Brand currently renders as Zilla Slab italic wordmark.

## Maps

Placeholder in `visit.html`. Replace with a Google Maps iframe embed for **960 Lee Street, Suite 200, Jefferson, GA 30549**.

## Forms

The catering inquiry form on `index.html#inquire` and `catering.html#inquire` currently triggers `alert()` on submit. Wire to send to **catering@thymetocater.com** with subject prefix `[Catering Inquiry]` via Cloudflare Pages Functions + an email backend (Resend, Postmark), Formspree, or a Google Form embed.

## Content to confirm with client

### Verified from public sources (2026-04-20)
- Address: 960 Lee St, Suite 200, Jefferson, GA 30549 (Yelp, Google, GA Business Journal)
- Catering phone: (706) 338-1163 (Thyme to Cater website)
- Cafe phone: (762) 763-2004 (Bistro To Go / Clover listing)
- Email: catering@thymetocater.com (Thyme to Cater website)
- Owner / chef: Keith Mosser (with wife Mindy Mosser, co-founder); trained in Florence, Italy, apprenticed under Johann Lafer in Stromberg, Germany
- Catering established: 2009 (per Thyme to Cater website)
- Award: "Best Catering" in Jackson County 2023, 2024, 2025 & 2026 — used as "3 Years Running" on the hero pill (the live site note said three years; public sources say four). **Confirm with client which framing to use.**

### Unverified / placeholder (FLAG)
- **Hero pill copy** — "Voted Best Catering · 3 Years Running" follows the brief. Public sources suggest four consecutive years (2023–2026). Update to "4 Years Running" if client confirms.
- **Testimonial on homepage** — "From the tasting to the last plate cleared…" attributed to "Hannah & Drew M. · Wedding, 180 guests" is **fabricated as a plausible placeholder**. Replace with a real testimonial from the client's files before launch.
- **Today's lunch menu items** — The 5 items on the homepage (Chicken Salad Croissant, Tomato Basil Bisque, Turkey & Brie Panini, Harvest Cobb, Chef's Take-Home Dinner) are composed from publicly described categories (paninis, salads, take-home dinners, from-scratch pastries). Prices are plausible but **not verified**. The intent is that the client will update this daily.
- **"Tomorrow" teaser** — Plausible placeholder. Update daily via CMS or hard-edit.
- **Menu page items & prices** — All items on `menu.html` are composed to match publicly described categories. Confirm against the real Clover online-ordering menu at clover.com/online-ordering/bistrotogo. Items marked `$ —` need pricing (Lasagna Bolognese, Chicken Pot Pie, Bistro Cookie Box).
- **Catering package pricing** — All four packages show `$ — / guest`. Public sources do not publish per-guest pricing; client to supply.
- **Sample catering menus** — Three sample menus on `catering.html` (Signature Wedding Dinner, Corporate Lunch Buffet, Rehearsal Dinner Southern) are composed as representative examples. Confirm each menu item is something the kitchen actually prepares.
- **Hours** — Used Bistro To Go / Clover hours (Mon–Fri 6a–7p, Sat 8a–2p, Sun closed). Note that Yelp lists different hours (Mon–Thu 6a–10p, Fri 5a–10p, Sat–Sun 6a–10p) which appear outdated. Confirm current hours with client.
- **"Events catered 7 days"** footer note — assumed. Confirm.
- **Chef Keith's experience: "17 years"** — derived from catering-established-2009 through 2026. Public sources also say "27 years in food service" generally. Copy currently says "For 17 years he's been cooking weddings" (referring to Thyme to Cater's age, not Keith's overall career). Confirm framing.
- **$250 wedding administrative fee** — verified from Thyme to Cater website; confirm still current.

## Copy to double-check

Content was drafted 2026-04-20 from public sources: thymetocaterbistro.com, thymetocater.com, Yelp, Google Business Journal, Facebook (Bistro to go — Thyme to Cater), and the Jackson County Chamber listing. Before going live, have the client review:
- The full `menu.html` items, prices, and descriptions
- The three sample menus on `catering.html`
- The homepage testimonial (currently a placeholder)
- The "3 Years Running" vs "4 Years Running" award framing

## External integrations (confirm or link)

- **Clover online ordering** — https://www.clover.com/online-ordering/bistrotogo — not currently linked from this site. Consider adding an "Order online" button on `menu.html` and in the header CTA region.
- **Instagram** — @thymetocaterga, @bistro_togo_ga — consider a footer social link row.
- **Facebook** — facebook.com/ThymetoCater and facebook.com/bistrotogottc — same.
