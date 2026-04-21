# White Tiger — Asset Requirements

This redesign unifies three existing brand domains (whitetigergourmet.com, whitetigerathens.com, whitetigerdeluxe.com) into a single site. Placeholders are used throughout for photography, maps, and pricing. Here's what we need from the client to ship live.

## Brand consolidation (most important)

The live business has three public-facing domains with overlapping but inconsistent content:

- **whitetigergourmet.com** — original site for the Athens Hiawassee location
- **whitetigerathens.com** — newer marketing site for Athens
- **whitetigerdeluxe.com** — standalone site for the Watkinsville location

This redesign assumes consolidation onto a single site with two location pages. **Confirm with client:**
1. Which domain becomes canonical (recommend **whitetiger.com** or **whitetigerathens.com** as the umbrella)?
2. Are the other two domains 301-redirected?
3. Do "Gourmet" and "Deluxe" remain as location sub-names only, or should either be retired?
4. Confirm the Instagram handle — live at `@whitetigerathens`. Keep?

## Photography

Replace each placeholder visual with a real image in a new `assets/` subfolder. This site leans on typography and uses very little photography, but a few shots will help.

### Priority 1 — Home (`index.html`)
No photo placeholders on the homepage by design. Optional additions:
- **`assets/counter-normaltown.jpg`** — The service counter or exterior at Hiawassee Ave. Consider adding to the Normaltown location card. **Target:** 1000×1250px.
- **`assets/counter-deluxe.jpg`** — The service counter, bar, or drive-through at Watkinsville. **Target:** 1000×1250px.

### Priority 2 — Menu / Featured
- **`assets/tiger-plate.jpg`** — Hero shot of the Tiger Plate (pulled pork, mac 'n cheese, slaw, slider roll). Would go into the Featured Band if the client wants imagery there. **Target:** 1400×900px.
- **`assets/pimento-burger.jpg`**, **`assets/barbarella.jpg`**, **`assets/slaw-dog.jpg`** — Menu category imagery. **Target:** 800×800px each.

### Priority 3 — Nice to have
- **`assets/exterior-hiawassee.jpg`** and **`assets/exterior-watkinsville.jpg`** — Storefronts.
- **`assets/logo.svg`** — Proper vector logo to replace the Unbounded wordmark.
- **`assets/favicon.svg`** / **`.ico`** — Real favicons (current files are placeholders from the Astro scaffold).

## Maps

Placeholder blocks in `locations.html` for both counters. Replace with Google Maps iframe embeds for:
- **217 Hiawassee Ave, Athens, GA 30601** (Normaltown)
- **64 N Main St, Watkinsville, GA 30677** (Deluxe)

## Forms

The catering inquiry form on `catering.html#inquire` currently triggers `alert()` on submit. Wire to send to the client's preferred address (likely `catering@whitetigerathens.com` or `hello@whitetigerdeluxe.com`) with subject prefix `[Catering Inquiry]` via Cloudflare Pages Functions + Resend/Postmark, Formspree, or a Google Form embed.

Confirm the routing:
- Do all catering inquiries go to one inbox regardless of counter preference?
- Or split by the "Counter preference" select field in the form?

## External integrations (already linked, just confirm)

- **Toast online ordering (Athens):** https://order.toasttab.com/online/white-tiger-gourmet
- **Toast online ordering (Watkinsville):** https://www.toasttab.com/local/order/white-tiger-gourmet-watkinsville-64-n-main-st/r-9914ba3e-5dae-4d22-bd3e-87292b3fe62c
- **ezCater catering:** https://www.ezcater.com/catering/white-tiger-gourmet-1
- **Instagram:** https://www.instagram.com/whitetigerathens/

Confirm all URLs are current and primary. The redesign currently points the header "Order" CTA at the Athens Toast link.

## Content gaps to confirm with client

### Menu
- **Every price is a placeholder** (`$ —`). We pulled item names and descriptions from third-party listings (Yelp, Uber Eats, MenuGuide) and the live marketing sites. Confirm the full menu against the current printed menu. Add or remove items as needed.
- **Tiger Dog** — invented as a signature cross-sell of hot dog + pimento cheese + White Tiger sauce. Remove if not a real item.
- **Half & Half Plate** — plausible pit-style option, confirm it exists.
- **Cookie / Brownie / Seasonal Pie** — banana puddin' is confirmed; the other desserts are reasonable but need confirmation.
- **Deluxe-specific menu items** — the Watkinsville location has expanded burgers, brunch, and bar menu that are not reflected in detail here. If the client wants a per-location menu split, we need the Deluxe menu as a document.
- **Brunch menu** — Deluxe runs weekend brunch Sat 10a / Sun 10a. Menu not captured. Recommend adding a `brunch` anchor on `menu.html` or a Deluxe-specific section on `locations.html`.

### Hours
- **Normaltown:** Tue–Sun 11a–8p, closed Monday (confirmed via live search).
- **Deluxe:** Tue–Thu 11a–9p, Fri 11a–10p, Sat 10a–10p, Sun 10a–9p, closed Monday (confirmed via live search).
- Confirm both.

### Phone numbers
- **Normaltown:** (706) 353-6847 (confirmed).
- **Deluxe:** (706) 705-6115 (confirmed).

### Addresses
- **Normaltown:** 217 Hiawassee Ave, Athens, GA 30601 (confirmed).
- **Deluxe:** 64 N Main St, Watkinsville, GA 30677 (confirmed).

### Brand story
- **Owner/chef:** Ken Manring, Gainesville GA native, CIA-trained, opened White Tiger in March 2007. Currently only mentioned implicitly. Ask if he wants an "About" or "Our Story" page or a short founder line on the homepage.
- **Cart origin:** The business started as a BBQ cart outside the Athens courthouse before the 2007 brick-and-mortar. Used in passing in the locations page intro. Confirm the story is OK to tell publicly.
- **Building history:** 217 Hiawassee was built 1905, previously Davis House grocery and Thrasher's Grocery (known for biscuits in the '70s). Not in copy yet. Add if client wants that flavor.

### Catering
- **Package pricing and minimums** — all `$ —` placeholders. Need real numbers and minimum headcount.
- **Sample catering menu** — we extrapolated reasonable items. Confirm against the client's actual catering packet.
- **Bar packages from Deluxe** — mentioned on catering page. Confirm this is offered and how pricing works.
- **ezCater minimum** — currently linked without detail.

### Tagline / voice
- **"Gourmet. Grocery. BBQ counter. One brand, multiple counters."** — invented for the masthead to signal consolidation. Client may want this softened or replaced.
- **"One White Tiger. Three counters."** — the source brief referenced three counters. Research surfaced only two confirmed public locations (Hiawassee and Watkinsville). The site currently reads "Two spots, one White Tiger." If a third counter exists (e.g. a grocery pickup, a stadium cart, a seasonal pop-up), we need details before adding it back.

## Copy to double-check

Content was extracted from whitetigergourmet.com, whitetigerathens.com, whitetigerdeluxe.com, Yelp, Tripadvisor, Uber Eats, Toast, and local press on 2026-04-20. Before going live:
- Confirm the two-location claim. If there are more counters (stadium, farmers' market, pop-up), we need them.
- Confirm the founding year (2007) and the Watkinsville opening year (2022).
- Confirm both phone numbers, addresses, and hours.
- Confirm every menu item name, description, and price on `menu.html`.
- Confirm catering email address for form routing.
