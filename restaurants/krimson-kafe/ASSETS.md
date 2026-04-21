# Krimson Kafe — Asset Requirements

Placeholder flavor pills, price stubs, a map placeholder, and an inquiry form stub throughout. Here's what we need from the client.

## Photography

Replace each placeholder with a real image in a new `assets/` subfolder.

### Priority 1 — Home (`index.html`)
- **`assets/split-dine.jpg`** — Overhead of a pimento cheese sandwich on sourdough with pickle and chips, on a cream plate, warm natural light. Used as optional background fade on the left "Dine in" panel. **Target:** 1400x1050px.
- **`assets/split-cake.jpg`** — A cream cheese pound cake loaf, sliced, on a wooden board. Used behind (or next to) the right "Take one home" panel. **Target:** 1400x1050px.
- **`assets/exterior.jpg`** — Storefront on Greensboro Hwy with the red awning and Krimson Kafe sign. **Target:** 1600x900px.

### Priority 2 — Cakes (`cakes.html`)
- **`assets/cake-cream-cheese.jpg`**, **`cake-lemon.jpg`**, **`cake-chocolate.jpg`**, **`cake-vanilla.jpg`**, **`cake-pecan.jpg`**, **`cake-seasonal.jpg`** — Overhead shots of each flavor, sliced, consistent styling. **Target:** 900x900px square each.
- **`assets/mini-loaves.jpg`** — A box of mini loaves arranged. **Target:** 900x900px.
- **`assets/office-box.jpg`** — A mixed dozen box opened. **Target:** 900x900px.

### Priority 3 — Menu & Visit
- **`assets/menu-sandwich.jpg`** — Hero sandwich shot for top of menu page.
- **`assets/menu-soup.jpg`** — Bowl of tomato bisque on a wood counter.
- **`assets/interior.jpg`** — Dining room shot showing tables and counter. For Visit page.
- **`assets/counter-cakes.jpg`** — The pound cake display at the counter.

### Priority 4 — Nice to have
- **`assets/logo.svg`** — Vector logo to replace the Young Serif wordmark.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons (currently linked but not present).

## Maps

Placeholder is in `visit.html`. Replace with a Google Maps iframe embed for **40 Greensboro Hwy, Watkinsville, GA 30677**.

## Forms

The catering inquiry form on `catering.html#inquire` currently triggers `alert()` on submit. Wire to send to the cafe's preferred inbox with subject prefix `[Catering Inquiry]` via Cloudflare Pages Functions + an email backend (Resend, Postmark), Formspree, or a Google Form embed.

## External integrations

- **Online ordering** — currently linking to `https://www.krimsonkafe.com/` (their existing OpenCart storefront). If the client wants a proper ecommerce migration (Shopify, Square, Squarespace), the nav CTA and Cakes page "Order online" buttons need to point to the new URL. Confirm which platform they want to use for pound cake retail going forward.
- **Facebook** — linked to `https://www.facebook.com/p/The-Krimson-Kafe-100063474672987/`. Confirm current and active.

## Content to confirm with client

### Pound cake flavors & prices (HIGH)
We stubbed these flavors based on common small-batch cafe patterns: **Classic Cream Cheese, Lemon, Chocolate, Vanilla Bean, Brown Butter Pecan, Seasonal, Mini Loaves, Office Box, Whole Cake pre-order**. The live OpenCart storefront could not be fetched during build (tool permission denied). All cake prices are marked `$ —`. Client must provide:
- Actual current flavors (and seasonal rotation)
- Whole loaf price
- Mini loaf 6-pack price
- Office box 12-pack price
- Whole cake pre-order price & lead time
- Any size options beyond 9-inch loaf (e.g. bundt, mini-bundt, tube)

### Menu prices (MEDIUM)
Confirmed from Yelp / Tripadvisor / press:
- **Daily Soup Call — Cup — $4.25**
- **Wyllie Salad — $7.75**
- **Green Salad — $4.75**
- **Spring Salad — $9.25**
- **Deli Salads & Spreads — $7.75**
- **Pimento Cheese Sandwich — $9.75**
- **Chicken Salad Sandwich — $9.75**

Marked `$ —` (client to fill):
- Ruben, Turkey & Provolone, Tuna Salad, Grilled Cheese
- Bowl of soup, Chili, Tomato Basil Bisque specific prices
- Add-grilled-chicken surcharge
- Chicken Salad Plate price
- Pimento & Chicken Salad by the pint
- Fresh Fruit Cup
- All drinks (sweet tea, unsweet tea, lemonade, coffee, bottled drinks)

### Operating details
- **Hours** — live site shows Mon–Thu 11a–2p, Fri/Sat/Sun closed. Confirm this is still current (small cafes often shift hours seasonally).
- **Address & phone** — 40 Greensboro Hwy, Watkinsville GA 30677 · (706) 310-0888. Confirm.
- **Email** — not on the live site in any public-facing form. Ask for a catering/inquiry email.
- **Owner / founder name** — not referenced anywhere on the current site. Ask if they want a "meet the owner" or about page (can be added as `about.html`).
- **Founding year** — unknown. Ask for year founded for footer brand subtitle (optional).

### Catering
Catering is not explicitly documented on the live site, but reviews mention bagged-lunch orders. We wrote catering copy assuming: bagged lunches, sandwich trays, salad bowls, soup by the gallon, pound cake boxes, family tables. Client must confirm:
- Which of these they actually offer
- Minimum order sizes
- Delivery radius + delivery fee structure (or pickup-only)
- Lead time (we wrote "48 hours ideal")

### Voice / copy
- We used "lunch in, cake to go" / "Lunch in the cafe. Pound cakes by the box." as the tagline. Confirm client is happy with it.
- Masthead lede: "Lunch in the cafe. Pound cakes by the box. Catering on request." Confirm.

## Copy to double-check

Content was extracted from Yelp, Tripadvisor, Visit Oconee, Explore Georgia, and AllMenus on 2026-04-20. The live OpenCart storefront at krimsonkafe.com could not be fetched during build due to tool permissions; several flavor and price fields remain stubbed. Before going live:
- Confirm every menu item and price
- Confirm every pound cake flavor and price
- Confirm hours, address, phone, catering details
- Get high-quality food photography to replace placeholders
