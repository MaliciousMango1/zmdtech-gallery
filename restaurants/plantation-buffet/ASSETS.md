# Plantation Buffet — Asset Requirements & Content Gaps

Content was extracted from public listings (live site was not directly reachable via WebFetch/curl from this environment — research came from the Google business listing, Tripadvisor, Yelp, Facebook page, Flagpole article, Visit Athens GA listing, and the plantationbuffet.com URL). Before going live, walk through the items below with the owner.

## Source URL researched

- **Live site (canonical):** https://plantationbuffet.com/
- **Menu page (linked from live site):** https://plantationbuffet.com/menu/menus.php
- **Facebook:** https://www.facebook.com/plantationbuffet/ (also lists as "J&L Buffet")
- **Flagpole article (2025 rename):** https://flagpole.com/featured/2025/06/17/plantation-buffet-makes-a-change-and-more-food-news/
- **Visit Athens listing:** https://www.visitathensga.com/listing/j-&-l-buffet/5344/

## Content gaps — MUST confirm with owner before launch

### Pricing (home page `index.html`, pricing band)
Currently shown as `$ —` placeholders. Reviews on Yelp/Tripadvisor reference values between $10 and $15 for the all-you-can-eat buffet over the last few years — we did not find a confirmed current adult/senior/child price on the live site. **Confirm:**
- Adult lunch buffet price
- Senior (60+) discount / price — confirm whether one exists
- Child under 10 price
- Whether drink (sweet tea) is actually included or charged separately

### Menu rotation by day of week (menu.html)
The live site advertises "a different food bar every day" but we could not retrieve the actual by-day rotation. The day-by-day menu in `menu.html` (Mon pork chop, Tue country-style, Wed pot roast, Thu meat-and-three, Fri fish fry) is based on reviewer comments (fried fish is real and is reviewed as "especially Fridays"; fried pork chop is referenced as "available on Mondays") — the rest of the day-by-day specifics are plausible Southern-buffet standards but **not verified**. Get the actual weekly rotation sheet from the kitchen and replace wholesale.

### Always-on staples (menu.html, index.html buffet columns)
The list of daily staples is drawn from cumulative reviews. Items confirmed across multiple reviews: fried chicken, baked chicken, meatloaf, hamburger steak, fried fish, butter beans, turnip greens, collards, field peas, green beans, northern beans, mashed potatoes & gravy, mac & cheese, potato salad, coleslaw, cabbage, cornbread, peach cobbler, banana pudding, sweet tea. Items added by plausible inference (not directly confirmed in our sources): yeast rolls, hushpuppies, sweet potato pie, pound cake, garden salad, three-bean salad, sliced tomatoes, candied yams, pickled beets, blackberry cobbler, soft-serve ice cream, lemonade. **Walk the line with the kitchen and prune anything that isn't actually there.**

### Founding year / name on the masthead
Using "Since 1982" — the year Ed DeAngelo rebranded the 1977 Hanley's Hickory Pit as Plantation Buffet. If the owner wants to count from 1977 (the building's restaurant history), update the masthead meta, heritage year, footer `brand-sub`, and the About timeline accordingly.

### Rebrand to "J & L Buffet"
The business was renamed J & L Buffet in 2025 per the Flagpole article, but the site domain, Google listing, and Facebook handle all still read "Plantation Buffet." **Confirm with the owner which name is forward-facing for the new website** — options:
1. Keep "Plantation Buffet" as primary (current build).
2. Rebrand all pages to "J & L Buffet (formerly Plantation Buffet)."
3. Dual-brand, e.g. "Plantation Buffet · J & L."

If we switch to option 2 or 3, we'll need to update every page's header `brand-name`, the masthead, the About story, and the footer.

### Email addresses
We used `info@plantationbuffet.com` (visit page) and `catering@plantationbuffet.com` (catering page) as placeholders. **The live site does not publish an email.** Confirm real addresses or remove the email rows.

### Catering details
The live site / listings mention catering but no menu or pricing. Everything in `catering.html` (pan sizes, 10–25 servings per pan, 48-hour notice, delivery within Athens-Clarke County) is placeholder language. **Confirm:**
- Actual pan sizes and serving counts
- Minimum order / notice window
- Whether delivery is offered and the radius
- Whether there's a catering menu PDF to link to

### "Outdoor seating" claim (visit page)
Referenced on the live Facebook page in an older post. **Confirm the front patio still exists / is in use** before claiming it on the Visit page.

### "Plaque in the back hallway" anecdote (about page)
The eleven-year-regular / UGA groundskeeper anecdote in `about.html` is **invented for voice**. Either replace with a real regular's story (with permission) or delete that paragraph.

### Social media
Facebook page exists at https://www.facebook.com/plantationbuffet/ — currently not linked anywhere on the site. Ask if the owner wants it in the footer. No Instagram / X / TikTok found.

## Photography — placeholder blocks to replace

The design is deliberately text-forward, so photo placeholders are minimal. Only one placeholder block on the whole site:

- **`visit.html` map placeholder** — Replace with a real Google Maps iframe embed for `1119 Martin Luther King Jr. Pkwy, Athens, GA 30601`.

If the owner wants photography added later, good candidate spots (and the shots we'd need):
- **Exterior / signage** — The building is distinctive (cinder block, hand-painted sign). A single exterior hero shot on the About page would add a lot. Target: 1400×900.
- **Steam line / hot bar** — The steam line in action at peak lunch, from behind. Target: 1200×900.
- **Cornbread in cast iron** — A single well-lit shot of a cast-iron pan of cornbread. Would be a great homepage hero replacement if we ever swap out the text masthead. Target: 1200×1500 portrait.
- **Dessert station** — Cobbler and banana pudding together. Target: 1000×750.
- **Plates in hand** — A loaded plate on a tray, top-down. Target: 1000×1000 square.

## External integrations

None currently. If the owner eventually wants online ordering or reservations, we'll need to discuss the platform (catering inquiry form via Formspree / Cloudflare Pages Functions → email is the lightest option).

## Final confirmations before launch

- Address: 1119 Martin Luther King Jr. Pkwy, Athens, GA 30601 ✓ (confirmed across all listings)
- Phone: (706) 353-3663 ✓ (confirmed across all listings)
- Hours: Mon–Fri 10:30 AM – 2:00 PM, Sat–Sun closed ✓ (confirmed across all listings)
- Owner: Keith Gray (since 1998) ✓ (confirmed via Flagpole)
- History: Hanley's Hickory Pit (1977) → Plantation Buffet (1982) → Keith Gray (1998) → J&L Buffet addition (2025) ✓ (confirmed via Flagpole + Facebook post)
- Every price on every page — **NOT confirmed; flagged as `$ —` placeholders**
- Every menu item — **partially confirmed; see above**

## Favicons

`favicon.ico` and `favicon.svg` were left in place from the prior scaffold. Replace with Plantation Buffet-specific marks (a cornbread wedge, a cast-iron pan, a cursive "PB" — owner's call) when we have the brand assets.
