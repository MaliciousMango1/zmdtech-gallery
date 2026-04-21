# Marker 7 Coastal Grill — Asset Requirements

This is a content + photography checklist for going live. The site uses zero stock imagery by design — the chalkboard aesthetic on the homepage and menu deliberately leans on type, color, and hand-lettered feel instead of photos. What we do need is accuracy on the menu, drinks, and the founding-year stamp.

## Photography

The homepage intentionally has no hero photo block (the grill board IS the visual). Below is a nice-to-have list for future phases: social-media imagery, press kit, Google Business Profile, and optional menu-page detail shots.

### Priority 1 — Identity & Exterior
- **`assets/exterior-house.jpg`** — The historic house at 1195 S Milledge at dusk, porch lights on, sign visible. **Target:** 1600×1000px, landscape.
- **`assets/sign.jpg`** — Tight crop of the Marker 7 sign / nautical marker motif. Used for press + social avatar. **Target:** 1200×1200px, square.
- **`assets/logo.svg`** and **`assets/logo-dark.svg`** — Proper vector logo + dark-background variant to replace the "7" circle placeholder in the header.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons (the Astro leftovers are in place for now; confirm they match brand).

### Priority 2 — Food / Drink Hero Shots
- **`assets/food-oysters.jpg`** — Raw Gulf oysters on crushed ice, lemon + mignonette. **Target:** 1600×1000px.
- **`assets/food-shrimp-grits.jpg`** — Shrimp &amp; grits signature shot.
- **`assets/food-burger.jpg`** — Marker 7 Burger, straight on, fries in frame.
- **`assets/food-grouper-nuggets.jpg`** — Grouper nuggets with tartar and lemon.
- **`assets/bar-pour.jpg`** — A pint being poured at the bar — ambiance more than product.

### Priority 3 — Interior / Vibe
- **`assets/interior-bar.jpg`** — Interior bar shot, occupied at golden hour.
- **`assets/porch.jpg`** — The wraparound porch if it's used for seating.

## Maps

The `visit.html` map is a styled CSS placeholder. Replace with a Google Maps iframe embed for **1195 S Milledge Ave, Athens, GA 30605**.

## Content gaps — needs client confirmation

### Prices flagged `$ —`
These were not reliably available via public sources and need the current printed menu to fill in. Placeholder text is `$ —` with a legend at the bottom of the menu page.

- **Raw bar:** half-dozen oysters, dozen oysters, Oysters Blenville, peel-and-eat shrimp
- **Starters:** hush puppies, cup of gumbo
- **Grill mains:** wood-grilled mahi, blackened grouper, grilled salmon, whole Gulf snapper (`market`)
- **Sandwiches:** shrimp po'boy, grouper sandwich
- **All sides:** mac &amp; cheese, grits, black bean &amp; rice, sweet potatoes, fries, coleslaw, broccoli, hushpuppies, all four salads
- **All desserts:** key lime pie, bread pudding, bourbon pecan pie, chocolate pecan pie
- **All draft beers** — we listed 8 plausible GA / Southeast taps (Creature Comforts, Terrapin, Southern Brewing, Akademia, Sweetwater, Wicked Weed, Miller High Life, rotating cider). Confirm the actual rotation and pour prices.
- **All cocktails** — we wrote 6 house-style cocktails as placeholders (Coastal Paloma, Bay Breeze, Porch Rum Punch, Five Points Mule, Old Fashioned, Brunch Mimosa). Replace with the real cocktail menu.

### Prices we used verbatim from public menu extracts
Double-check these against the current printed menu — some may be out of date:

- Grouper Nuggets $10, Fried Green Tomatoes $10, Fried Artichoke Hearts $10
- Buffalo Shrimp $11, Fried Coconut Shrimp $12, Fried Calamari $12
- Shrimp &amp; Grits $24, Basil Poblano Shrimp Pesto $24, Crab Cakes $25, Lemon Sherry Scallops $27, Surf &amp; Turf $38
- Marker 7 Burger $14, Fish Tacos $14 (+$1 avocado), Blackened Salmon BLT $15
- Sunday brunch mimosa $4

### Content to confirm with client

- **Founding year** — the homepage corner-band statement says "On the corner of the old house at Five Points" without a date. Source material suggests the restaurant opened circa 2014–2015 under owner Chris Lloyd. Confirm the actual opening year so we can add "Since YYYY" to the brand subtitle and statement stamp.
- **Owner credit** — Chris Lloyd (also of Hilltop Grill) is referenced in press. Confirm whether he wants owner/operator credit on the site.
- **Email address** — no email is publicly listed. The contact page currently shows "via website contact form — call to confirm" with the phone number as the primary channel. Provide a real email if one exists and we'll swap in a `mailto:` link and (if desired) wire up an inquiry form.
- **Reservation policy** — we wrote "reservations for parties of 6 or more, walk-ins welcome otherwise" per public listing info. Confirm.
- **Private parties** — homepage strip points to the restaurant phone number for private party inquiries. Client may want a dedicated events email or inquiry form instead.
- **Pickup / takeout** — homepage strip says "call ahead (706) 850-3451, ready in 20–30 min." Client may use Toast, ChowNow, or another platform; swap the link accordingly.
- **Hours** — we used Mon 4–9, Tue–Thu 11–9, Fri–Sat 11–10, Sun 11–9 per public listings. Confirm — seasonal hours may differ.
- **Brunch** — "Sunday brunch, $4 mimosas" is repeated across public listings. Confirm brunch menu items (we did not break brunch out as its own section).
- **Tagline** — we used "Cold beer. Hot grill. Simple menu." Client can swap any time.
- **Signature dishes** — we tagged Grouper Nuggets, Marker 7 Burger, Shrimp &amp; Grits, and Oysters Blenville as "House Favorite" / "Signature." Confirm.

## External integrations (to add)

- **Reservations** — currently the nav uses a click-to-call phone link. If the restaurant uses OpenTable, Resy, Tock, or similar, add it to the header CTA and footer.
- **Online ordering** — if they use Toast / ChowNow / DoorDash for direct pickup, link it from the Private / Pickup strip and the nav.
- **Google Business Profile** — pull current hours + a map embed from GBP so we aren't hand-maintaining them.

## Copy sources

Content was extracted from public listings on 2026-04-20:
- marker7coastalgrill.co (owner site — could not be fetched by agent; structure and copy inferred from search summaries)
- visitathensga.com listing
- Yelp &amp; Tripadvisor listings
- Historical Marker 7 dinner menu PDF (dated 10.13.21 — prices likely out of date)

Before going live, confirm:
- Address: 1195 S Milledge Ave, Athens, GA 30605
- Phone: (706) 850-3451
- Facebook: facebook.com/Marker7CoastalGrill
- Instagram: @markerseven
- Every menu item and price on `menu.html`
