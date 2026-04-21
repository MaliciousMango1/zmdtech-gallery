# Big City Bread Cafe — Asset & Content Requirements

Redesign goal was editorial/upscale: a modern artisan cafe site structured around "dayparts" (when you'd visit) instead of a generic pitch. Content was researched on 2026-04-20 from the live site at **bigcitybreadcafe.com** plus Yelp, Tripadvisor, visitathensga.com, and Athens CEO. Network access to the live domain was blocked during the build, so we leaned heavily on cached search-snippet data — full menu detail needs confirmation.

## Photography

The homepage is intentionally text-only (the dayparts lists and the mission band carry the design). Photos are most valuable on the bakery page and the visit page. Create an `assets/` subfolder and replace the few placeholders.

### Priority 1 — Bakery (`bakery.html`)
- **`assets/bakery-loaves.jpg`** — Row of whole loaves on a wooden rack, cooling. Natural light. Shows craft without being staged. Target: 1600×900.
- **`assets/bakery-pastries.jpg`** — Pastry case or tray — croissants, scones, bars — shot from slightly above. Target: 1600×900.
- **`assets/catering-tray.jpg`** — A catering pastry or sandwich tray staged for drop-off. Target: 1200×900.

### Priority 2 — Visit (`visit.html`)
- **`assets/patio.jpg`** — The shaded patio, ideally with a couple of people in soft focus. Important because the patio is a key part of the visit. Target: 1600×900.
- **`assets/exterior.jpg`** — Corner-shop exterior, 393 N. Finley St, preferably morning light. Target: 1600×900.

### Priority 3 — Nice to have
- **`assets/hero-bread.jpg`** — A quiet hero still (a single loaf being sliced, or dough on a floured bench) that could replace the text-only masthead if the client prefers imagery on the homepage.
- **`assets/team.jpg`** — Matthew and Deenan Scott in the kitchen, or a team shot. Currently no owner/chef feature on the site; we could add an About page later.
- **`assets/logo.svg`** — Proper vector wordmark to replace the Bodoni Moda text treatment.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons. Currently using the placeholders that were already in the folder.

## Maps

Placeholder is on `visit.html`. Replace with a Google Maps iframe embed centered on **393 N. Finley St, Athens, GA 30601**. The text "Open in Google Maps" link is already wired to `google.com/maps/dir/?api=1&destination=...`.

## External integrations (already linked, confirm)

- **Toast online ordering:** https://order.toasttab.com/online/bigcitybreadcafe — confirm this is current.
- **Instagram:** https://www.instagram.com/bigcitybreadcafe/
- **Facebook:** https://www.facebook.com/BigCityBreadCafe/

## Forms

There is no catering inquiry form — the site uses `mailto:info@bcbcafe.com` and `tel:` links. If the client wants a form (the live site has one at `/catering-form`), wire it up on `bakery.html#catering` with Cloudflare Pages Functions + Resend / Postmark / Formspree, routed to `info@bcbcafe.com` with subject prefix `[Catering Inquiry]`.

## Content gaps — needs client confirmation

These items are flagged in-place with `$ —` (price) or live in the menu as placeholder descriptions. Every one needs client sign-off before launch.

### Prices not confirmed
Every menu item flagged with `$ —` needs a real price. Specifically:
- **Breakfast:** Breakfast Sandwich, Two Eggs Any Way, Granola & Yogurt Parfait, Biscuits & Jam.
- **Lunch:** BLT, French Ham & Cheese, Fresh Mozzarella sandwich, Soup of the Day, House Salad, Tahini Salad.
- **Brunch:** Eggs Benedict, Shrimp & Grits, Breakfast Hash, Avocado Toast. (These are inferred weekend items — we could not verify which are actually on the live brunch menu.)
- **Drinks:** All coffee/tea/wine prices. We confirmed they use 1000 Faces and Jittery Joe's roasters but did not get pulled-shot prices.
- **Bakery:** Individual loaf prices, cake slice prices, cookie and bar prices. We have a price range ($4 – $6.25) for pastries but not per-item breakdowns.

### Prices that ARE confirmed (from search snippets — still double-check against current printed menu)
- Big City Quiche — $13.50
- French Toast — $9.00
- Choose Two Plate — $11.50
- Smoked Turkey sandwich — $14.00
- Chicken Salad sandwich — $15.00
- Tuna Salad sandwich — $14.00
- BBQ Tofu sandwich — $14.00
- Hummus Sandwich — $13.50
- Pastries / bars range — $4.00 – $6.25

### Menu items that may not exist on the live site
We inferred several items from general cafe conventions to flesh out the "dayparts" lists. These should be removed if they aren't really on the menu:
- **Brunch page:** Eggs Benedict, Shrimp & Grits, Breakfast Hash, Avocado Toast — we could not verify these specifically, though brunch-all-day is real on weekends.
- **Drinks:** Pour-Over, Mimosa/Bellini, loose-leaf tea — inferred.
- **Bakery specialty loaves:** Olive, rosemary, walnut-raisin — we know they do specialty loaves by order, but the specific flavors are placeholders.
- **Pastries:** Chocolate Peanut Butter Bars, Lemon & Raspberry Bars, Pecan Pie Bars — mentioned in search snippets, confirm currency.

### Copy that needs confirmation
- **Founding year — 1998.** Confirmed in multiple sources (About page mentions 20+ years in 2021, Athens CEO article from 2021 confirms).
- **Owners — Matthew and Deenan Scott.** Confirmed via Athens CEO feature and wedding-wire listing. Matthew Scott is chef/owner, graduate of Johnson & Wales culinary program. We did NOT include a dedicated "about the owners" page or block — the brief called for a minimal 4-page site. If the client wants an About page, we can add one.
- **Phone — (706) 353-0029.** Confirmed. Secondary catering line **(706) 353-0043** also confirmed.
- **Email — info@bcbcafe.com.** From search snippets. Double-check.
- **Address — 393 N. Finley Street, Athens, GA 30601.** Confirmed.
- **"Studio C" suffix.** Yelp/Bipper Media list the address as "393 N Finley St **Studio C**" — we omitted "Studio C" for cleaner typography. Confirm whether the mail address needs it.
- **Hours** — Mon–Fri 8a–3p, Sat & Sun 8a–2p. Confirmed by multiple sources. We list Saturday + Sunday as "Brunch" since the live site calls them brunch service, even though breakfast items run all day.
- **Party capacity — "60 or less".** Taken verbatim from the WeddingWire listing for the cafe's event rentals. Confirm.
- **Lead time — "24 hr" / "48 hr".** Inferred. The live catering page has specifics we could not fetch — replace with real lead times.
- **Mission-band quote.** "We knead dough at 5am. Coffee's on by 6. Doors open at 7." is **our copy**, not a client quote. Swap it for a real line from Matthew or Deenan Scott if the client wants attribution.
- **Daypart window "7 to 11am" in brief** was corrected to the real open: **8a for breakfast, 11a for lunch**.

## Copy / SEO checklist

Before launch:
- Confirm address format (393 N. Finley St vs. 393 N. Finley St Studio C).
- Confirm hours — the live site may vary seasonally (search results mention slightly different Saturday closes in some third-party listings).
- Review every `$ —` flag and replace with real pricing.
- Proof every sandwich description against the live menu — the five confirmed ones map to the live lunch page, but the other three (BLT, French Ham & Cheese, Fresh Mozzarella) are plausible additions we inferred from the Choose Two Plate options list.
- Decide on an About page. Chef Matthew Scott's Johnson & Wales background and Matthew + Deenan's ownership is a good short story the current site doesn't emphasize.
- Confirm the Toast online-ordering URL is still active.

## Research sources

- https://www.bigcitybreadcafe.com/ (home)
- https://www.bigcitybreadcafe.com/lunch (lunch menu)
- https://www.bigcitybreadcafe.com/brunch (brunch menu)
- https://www.bigcitybreadcafe.com/about (history)
- https://www.bigcitybreadcafe.com/catering
- https://www.bigcitybreadcafe.com/contact
- https://athensceo.com/features/2021/07/big-city-bread-cafe-celebrates-20-years-regulars... (founding year, owners)
- https://www.yelp.com/biz/big-city-bread-cafe-athens-2
- https://www.tripadvisor.com/Restaurant_Review-g29209-d968529-Reviews-Big_City_Bread_Cafe-Athens_Georgia.html
- https://www.visitathensga.com/listing/big-city-bread-cafe/82/
- https://www.weddingwire.com/biz/big-city-bread-cafe-catering-athens/5e0b9d90c6654e96.html

Direct WebFetch and curl to bigcitybreadcafe.com were blocked during this build; every fact above was pulled from search-engine snippets of those pages. A second pass with direct fetching would sharpen the menu and catering detail considerably.
