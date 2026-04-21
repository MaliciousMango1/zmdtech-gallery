# The Traveling Hobo Cafe — Asset Requirements

The home page was intentionally designed to work without photography — it leans heavily on typography and at-a-glance information density (the "Google Business card" pattern). Most of what's missing is content confirmation, not imagery.

## Photography

The cafe does not currently host high-resolution imagery on its Facebook page. Most photos on aggregator sites (Yelp, Tripadvisor) are user-uploaded, unlicensed, and low-resolution. To replace the map placeholder and upgrade the menu page, we'd want:

### Priority 1 — Nice-to-have, not blocking
- **`assets/exterior.jpg`** — Front of the building on Greensboro Hwy, porch visible, ideally in afternoon light. **Target:** 1600×1000px, landscape. For use on the Visit page above the map and (optionally) in a future About section.
- **`assets/hero-burger.jpg`** — The Classic Hobo Thick Burger, plated with Box Car fries. **Target:** 1200×900px. Could optionally be added to the home at-a-glance card or the menu preview.
- **`assets/hero-shrimp-basket.jpg`** — The fried shrimp basket with slaw and a lemon wedge. **Target:** 1200×900px.

### Priority 2 — If the client wants a menu gallery
- **`assets/menu-detail/`** — 4–6 plated food shots (burger, po' boy, shrimp basket, fried green tomatoes, Cobb salad, lemonade). 1000×750px each.
- **`assets/interior.jpg`** — Dining room or porch, occupied tables fine if lit well, or empty for a quiet-hours shot.
- **`assets/owner.jpg`** — If the client wants an About page, a candid of the owner/chef in the kitchen.

### Priority 3 — Branding
- **`assets/logo.svg`** — Vector logo to replace the Marcellus wordmark in the header. The Facebook page uses a railroad/boxcar-style mark; request the original artwork or a clean redraw.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons. Currently not linked (no favicon files in this folder).

## Maps

Placeholder is on `visit.html`. Replace with a Google Maps iframe embed for **20 Greensboro Hwy, Ste B, Watkinsville, GA 30677**.

## Content to confirm with client

**Business basics — from aggregator sites, needs verification:**
- **Address** — 20 Greensboro Hwy, Ste B, Watkinsville, GA 30677 (Yelp, Tripadvisor, Sirved). Confirm "Ste B" is correct; some listings show no suite number.
- **Phone** — (706) 310-4323. Confirm this is the correct, current number (allmenus.com lists (877) 585-1085 which is a generic aggregator number, not theirs).
- **Hours** — Currently listed as Tue–Sat 11a–8p with a mid-day break on some days. **Please confirm exact hours.** We simplified to "11a–8p" for clarity; several sources show a 2:30p–4p kitchen break. Which is current?
- **Closed days** — Listed as Mon and Sun closed. Confirm.

**Brand identity — prescribed brief says "Bold / Fast-Casual" and "cafe":**
- The actual menu leans heavily on burgers, fried baskets, and sandwiches — more of a lunch/dinner diner than a breakfast cafe. We kept the tagline "Coffee's on. Breakfast's ready." from the brief but **the menu shows no breakfast items and no coffee listing**. Confirm with client whether they serve breakfast/coffee (the name suggests yes, but public menus do not list it). If not, we should revise the tagline and the home masthead's right-column line.
- **Popular dishes** on the home were pulled from Yelp/Tripadvisor review mentions. Replace with the owner's actual top 3.

**Menu accuracy — pulled from Sirved on 2026-04-20:**
- All 60+ menu items and prices came from Sirved. These may be out of date. Confirm against the current printed menu. Expect to add: daily specials, seasonal items, breakfast menu (if applicable), and a coffee/espresso list (if applicable).
- **Item descriptions** under each name were written by us for flavor — confirm they match what's actually on the plate (e.g., "Railroad Reuben Burger" is described as "Swiss, sauerkraut, Thousand Island on a house burger" but we don't have the actual recipe).
- **Build Your Burger** section from Sirved was folded into the main burgers section for clarity. Confirm the client is OK with this.

**Voice & tagline:**
- Home masthead italic line — "Coffee's on. Breakfast's ready." Confirm or replace.
- Find us strip — "the little place with the porch and the lemonade out front." Written from aggregator photos showing a porch; confirm accuracy.
- Visit page note about "short break between lunch and dinner" — remove if not applicable.

**Parking details (`visit.html`):**
- We wrote "free lot on-site in front of the building... additional street parking." This is a reasonable guess for a small highway-side cafe in Watkinsville but was not verified. Confirm.

**Dog-friendly claim:**
- Yelp and Tripadvisor both list the cafe as dog-friendly. We wrote "Welcome on the porch with a water bowl." Confirm.

**Founding year / history:**
- No founding date is published on Facebook or aggregator sites. The oldest Tripadvisor reviews go back several years. If the client wants a founding year on the brand subtitle or a future About page, we need it.

## Linking

The site currently has no online ordering, no reservations, and no email. If the client wants any of those:
- **Online ordering** — set up with Toast, ChowNow, Square, or similar; add "Order online" CTA in header.
- **Email inquiries** — currently no email anywhere on the site. If they want a contact form or email link, provide the address.
- **Reservations** — not typical for a fast-casual cafe of this size. Probably skip.

## External links verified (please re-check before launch)

- Facebook: https://www.facebook.com/TravelingHoboCafe/
- Yelp: https://www.yelp.com/biz/the-traveling-hobo-cafe-watkinsville
- Tripadvisor: https://www.tripadvisor.com/Restaurant_Review-g35353-d9586859-Reviews-The_Traveling_Hobo_Cafe-Watkinsville_Georgia.html
- Google Maps directions: https://www.google.com/maps/search/?api=1&query=20+Greensboro+Hwy+Watkinsville+GA+30677

## Copy source

Content was extracted from the cafe's Facebook page, Yelp, Tripadvisor, Sirved, and Explore Georgia on 2026-04-20. Before going live, confirm:
- Address: 20 Greensboro Hwy, Ste B, Watkinsville, GA 30677
- Phone: (706) 310-4323
- Hours (see above)
- Every menu item and price on `menu.html`
- Whether the "cafe / coffee / breakfast" positioning matches their actual menu or should be revised to "fast-casual diner" language
