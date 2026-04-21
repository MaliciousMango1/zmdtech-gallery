# George's Lowcountry Table — Asset Requirements

The rebuild is intentionally photo-light. The homepage uses typography and hairlines instead of hero photography — the "What came in today" kitchen board is the visual hero. That said, a few placeholders and blanks remain for the client to fill.

## Site basics — confirm with client

- **Founding year** — we set "Est. 2016" based on a Red & Black profile noting Reggie DiSante had opened the restaurant "nine years ago" as of 2019. Confirm actual founding year.
- **Address** — 420 Macon Hwy, Athens, GA 30606 (from Yelp / Visit Athens). The prompt mentioned a Watkinsville / Windsor framing; the restaurant is actually on Macon Hwy near Five Points in Athens. Copy uses Athens GA + "Five points edge" language; adjust if the client prefers the Watkinsville identity.
- **Phone** — (706) 548-3359. Confirm.
- **Email** — we used `info@georgeslowcountrytable.com` and `events@georgeslowcountrytable.com` as plausible patterns. The live site's domain is georgeslowcountrytable.com, so these are reasonable guesses. Confirm real inboxes.
- **Reservation URL** — wired to `https://resy.com/cities/athens-ga/venues/georges-lowcountry-table` from a search result. Confirm this is the current Resy venue URL. The live site also mentions OpenTable-style 24-hour-ahead booking — confirm whether Resy or a different platform is the canonical link.
- **Named-for-George-Davis copy** — we credit George Davis (Gus Garcia's, Harry Bissett's) in the footer tag and in the copyright line. Sourced from the Red & Black profile; confirm the wording is acceptable to Reggie.

## Menu — items and prices

All prices in `menu.html` and on the homepage `catch` grid are drawn from public menu listings. Flag anything out of date.

### Prices pulled from public listings (confirm current)
- Shrimp and Grits entree — **$21**
- Shrimp and Grits starter — **$9**
- Seared Scallops — **$30**
- Pan Seared Redfish — **$25**
- Seafood Jambalaya — **$20**
- Shrimp Tortellini Carbonara — **$22**
- Stuffed Eggplant — **$18**
- Fried Green Tomatoes — **$8**
- Sherry Crab Bisque — **$7**
- Gumbo Ya Ya — **$7**
- French Onion — **$6**
- Shrimp Remoulade — **$8**
- Popcorn Crawfish — **$9**
- Pimento Cheese & Fried Okra — **$8**
- Oysters — **$5–$10** (raw or chargrilled)
- Oyster Tuesday — **one dozen for $12.95**

### Marked `$ —` (needs confirmation)
- Oyster by-the-piece and dozen pricing (Raw Bar section, homepage)
- Lowcountry Boil entree
- All sides (Stone-ground grits, Hoppin' Johns, Braised Collards, Fried Okra, Red Beans & Rice)
- All desserts (Bread Pudding, Crème Brûlée, Key Lime Pie, Chocolate Eruption, Caramel Cheesecake)

### Items we inferred / added
- **Desserts list** — Bread Pudding, Crème Brûlée, Key Lime Pie, Chocolate Eruption, Caramel Cheesecake. The first four are from public menu listings; caramel cheesecake is from a review mention. Confirm the current dessert card.
- **Sides** — assembled from customary Lowcountry / Cajun sides (collards, hoppin' johns, stone-ground grits, red beans, fried okra). Confirm which are actually on the plate at George's.
- **Lowcountry Boil** — referenced on the live site as a special. Flagged price pending.

## Oyster list — INVENTED

The five oyster varieties on the homepage "We shuck by the dozen" strip are **plausible but invented**. The live site does not publish a rotating oyster-variety list. The names chosen (Beausoleil, Apalachicola, Blue Point, Sewansecott, Kumamoto) cover typical East Coast / Gulf / Pacific spreads a coastal restaurant might carry, but **every one should be replaced with what the kitchen actually orders** before going live. Prices all marked `$ —`.

## Events — INVENTED SPECIFICS, CONFIRMED CAPACITY

- **Capacity of 40 — confirmed** via multiple public listings.
- **Three-course rehearsal format, two weeks' notice for catering, Tuesday–Thursday buyout window, room-fee-waived-at-minimum** — these are all plausible restaurant-industry defaults we wrote to flesh out the page. Reggie should read and edit or replace with the actual offering.
- **Tailgate / off-premise catering** — the live site and reviews mention catering; we extended it to tailgates (gameday is a reasonable Athens angle). Confirm the client actually does this.

## Forms

The events inquiry form on `events.html#inquire` fires `alert()` on submit. Before launch, wire to:
- Post to `events@georgeslowcountrytable.com` via Formspree / Resend / Cloudflare Pages Functions.
- Subject prefix `[Event Inquiry]`.

## Maps

`visit.html` has a hairline-grid map placeholder. Replace with a Google Maps iframe embed for **420 Macon Hwy, Athens, GA 30606**.

## Photography

Homepage is intentionally photo-free — this is by design. The rebuild leans on typography and the kitchen board layout. Optional future adds:
- `assets/interior.jpg` — dining room at service, low light.
- `assets/oysters.jpg` — oyster plate, overhead, natural light.
- `assets/grits.jpg` — shrimp and grits hero.
- `assets/exterior.jpg` — the Macon Hwy storefront at dusk.
- `assets/logo.svg` — vector logo to replace the Spectral wordmark.
- `assets/favicon.svg`, `assets/favicon.ico` — favicons are currently the placeholder Astro-export files; replace with brand favicons.

## Social & integrations

- Instagram: `https://www.instagram.com/georgeslowcountry/` (confirmed).
- Facebook: `https://www.facebook.com/georgeslowcountry/` (confirmed).
- SpotOn online ordering: `https://order.spoton.com/so-georges-lowcountry-table-15705/...` — not currently linked. Ask if they want a "Order online" link on Visit or in the footer.

## Copy to confirm

All research done on 2026-04-20 via public search result summaries (live site fetch was blocked in this environment). Before going live, please confirm:
- Address, phone, email
- Hours
- Every menu item and price (including the homepage catch grid)
- The George Davis attribution wording
- Founding year
- Reservation URL
