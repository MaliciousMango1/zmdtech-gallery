# The Place — Asset Requirements

The site is intentionally photo-light. The short-list menu-as-homepage design leans on typography over imagery, so there are no photo placeholders to swap. The asset gaps are primarily content confirmations (prices, hours, a map embed) and, if the client wants them, a small set of optional atmosphere photos for a future gallery section.

## Content to confirm with client

**Every price on the menu is rendered as `$ —` (em-dash flag).** We did not invent prices. Before going live, replace each flagged item across `index.html` and `menu.html` with the current menu price.

- **Founding year — "Since 2015"** — reported as February 2015 from press interviews with Alan Pope. Confirm exact month/year to display on brand subtitle (every header + footer) and on the homepage eyebrow.
- **Address — 229 E Broad Street, Athens, GA 30601** — taken from Yelp, Visit Athens, and the restaurant's live site. The creative brief described it as "Clayton Street"; the actual address is East Broad. Confirm before print.
- **Phone — (706) 850-2988** — confirm.
- **Email — info@theplaceathens.com** — confirm this is the correct public-facing inbox.
- **Hours** — Mon–Thu 11 am–9 pm, Fri–Sat 11 am–10 pm, Sun brunch 10 am–2 pm, Sun dinner 4 pm–9 pm. Sourced from Yelp + Visit Athens listings. Confirm, especially the Sunday brunch-break-dinner split — live sources disagreed on whether there's an afternoon break.
- **Reservations channel** — we say "by phone, walk-ins welcome." If they use OpenTable, Resy, or Toast reservations, add the link to the reservation rail on home and the contact block on `visit.html`.
- **Menu accuracy** — entrees on the short list (Buttermilk Chicken, Shrimp & Grits, Bone-in Pork Chop, Braised Pork Shoulder, Red Snapper, Hand-Pressed Burger, Meat & Three) pulled from the live site, Yelp, and Visit Athens. Biscuit Benedict is brunch-only per their brunch menu. On `menu.html` we added plausible but unconfirmed items: Cornbread & Honey Butter, Deviled Eggs, House Wedge, Collards, Mac & Cheese, Mashed Potatoes, Bourbon Pecan Pie, Banana Pudding, Peach Cobbler. Confirm or replace with the actual sides/desserts list.
- **Wine / bar list** — we wrote four placeholder drink entries (House Red, House White, Bourbon Neat, Sweet Tea). They have an upstairs bar that stays open late per press. If they want a real bar list featured, we need the list.
- **Owners — Alan & Ryan Pope** — named in the provenance paragraph on `index.html`. Confirm spelling and that they're comfortable being named.
- **The grandfather's car dealership story** — used in the provenance copy ("we named it after our grandfather's car dealership"). Confirmed from press; verify the family is okay with us leaning on it.

## Photography (optional — not required by current layout)

The home page is typographic by design. If the client later wants imagery:

- **`assets/exterior.jpg`** — Evening exterior of the brick storefront at 229 E Broad, ideally with The Arch visible across the street. **Target:** 1600×1000px.
- **`assets/dining-room.jpg`** — Downstairs dining room, warm light, occupied tables or empty. **Target:** 1200×900px.
- **`assets/upstairs-bar.jpg`** — The upstairs bar at night. **Target:** 1200×900px.
- **`assets/plate-chicken.jpg`** — The Buttermilk Chicken on the waffle (their signature). **Target:** 1200×900px.
- **`assets/plate-shrimp-grits.jpg`** — Shrimp & grits, the other signature. **Target:** 1200×900px.
- **`assets/logo.svg`** — Proper vector wordmark to replace the Libre Caslon Text italic brand text.
- **`assets/favicon.svg`** / **`assets/favicon.ico`** — Real favicons. Current favicons were carried over from the placeholder scaffold and should be replaced.

## Maps

`visit.html` has a typographic grid placeholder that reads "MAP — 229 E Broad St · Across From The Arch". Replace with a Google Maps iframe embed for **229 E Broad Street, Athens, GA 30601** before launch.

## External integrations

- **Reservations** — currently "by phone." If the client signs up with Resy/OpenTable/Toast, add the URL in three places: the reservation rail on `index.html`, the contact block on `visit.html`, and the footer across all three pages.
- **Online ordering** — Toast ordering is live at `order.toasttab.com/online/the-place-athens`. Not currently linked in our site. Decide whether to surface it (probably in the footer and/or on `visit.html`) or keep the site purely brand-editorial.
- **Social** — Facebook and Instagram (@theplaceathens) exist. Not currently linked. Add to footer if desired.

## Copy voice

Provenance paragraph on `index.html` is written in first-person plural, literary, italic Libre Caslon body. Tone is confident-quiet: "We took over a quiet brick-walled room across from The Arch and gave it back to Southern cooking." Read it out loud before approving — the owners should recognize themselves in it.

## Sources

Extracted 2026-04-20 from:
- `theplaceathens.com` (home, about, contact, dinner, sunday-brunch, menus, catering, trays)
- Yelp listing — 229 E Broad St, Athens
- Visit Athens GA listing
- Tripadvisor, MenuGuide, allmenus.com
- Emily Selby Q&A with Alan Pope (opening-year reference)
