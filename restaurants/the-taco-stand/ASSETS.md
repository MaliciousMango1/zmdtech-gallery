# The Taco Stand — Asset Requirements & Content Gaps

The design is intentionally type-forward — the homepage has no photography at all. Sub-pages are also photo-light by design. This is a fast-casual brand where the menu IS the pitch, and the typography carries the look. That said, there are still real gaps the client should fill in before go-live.

## Photography (optional, low priority)

The current build runs without any photography. If the client wants to add imagery in a future pass, good candidates would be:

- **`assets/exterior-milledge.jpg`** — Milledge Avenue storefront, ideally with the classic red awning. **Target:** 1600×1000px.
- **`assets/exterior-downtown.jpg`** — E Broad St location exterior. **Target:** 1600×1000px.
- **`assets/exterior-eastside.jpg`** — Barnett Shoals location exterior. **Target:** 1600×1000px.
- **`assets/counter-interior.jpg`** — The counter, red booths, paper menus. Evokes the '77 origin. **Target:** 1600×1000px.
- **`assets/hero-taco-lineup.jpg`** — Overhead of 4–6 tacos lined up on a tray. Could optionally replace the giant-type hero on home. **Target:** 2000×1250px.
- **`assets/sauce-lineup.jpg`** — Six salsa cups in a row, cilantro scattered. Could go into the sauces strip. **Target:** 1600×600px.
- **`assets/logo.svg`** — Proper vector logo to replace the Bricolage wordmark.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons (placeholders retained from initial folder).

## Content gaps — items flagged `$ —` on the site

The following items are on the board but we couldn't find current pricing from the live site, allmenus, or Tripadvisor/Yelp listings. Client should fill in:

### Tacos
- Pork taco — price missing
- Grilled shrimp taco — price missing

### Burritos
- Bean & Cheese burrito — price missing

### Salads / Bowls
- Taco Salad with steak, shrimp, fish, or tofu — prices missing
- "Burrito Bowl (no shell)" — we assumed this is offered (common at taqueria counters); confirm it exists and add price

### Drinks
- Fountain soda — price missing
- Bottled water — price missing
- Beer selection and pricing — entirely missing (if beer is even on the menu; confirm)

## Content to confirm with client

- **Founding year** — "Since 1977" is based on multiple published references (Red & Black guides, visitathensga.com). Confirm the actual founding year.
- **Number of locations** — we built the site around three locations (Milledge, Downtown E Broad, Eastside Barnett Shoals). Tripadvisor lists a 2270 Barnett Shoals address too; confirm which Barnett Shoals address is current and whether 2230 or 2270 is correct.
- **Eastside address** — published as "2230 S Barnett Shoals Rd" on some listings and "2270 Barnett Shoals Rd" on Yelp. Confirm correct address.
- **Hours, all three locations** — Milledge shows 11:00a–9:30p daily across most sources. Eastside shows "Mon–Sat 11:00a–9:00p, Sun closed" on Tripadvisor. Downtown hours were not published and are marked "Confirm at counter" on `visit.html`. Confirm all.
- **Phone numbers** — used:
  - Milledge: (706) 549-2894
  - Downtown: (706) 549-1446
  - Eastside: (706) 549-5481
  All three came from published business listings. Confirm.
- **Email** — we used `hello@thetacostandathens.com` on `order.html` as a plausible placeholder. No email was published on the live site. Client should supply a real contact email or remove the line.
- **Menu accuracy** — pulled verbatim item names and prices from allmenus.com, MenuGuide, Tripadvisor, and published listings. Prices at fast-casual spots move; confirm the current board at each location before going live.
- **Item descriptions** — for the flagship homepage tacos, we wrote short descriptions in The Taco Stand's voice (e.g., "A college-town original — copy at your peril"). The live site does not have these; if the client wants descriptions kept minimal or rewritten, they can rewrite.
- **Tags on tacos** — we tagged some items "Classic", "Hot", "Veg" for visual flavor. Confirm which items should carry which tags (e.g., Buffalo Chicken is tagged "Hot" but not confirmed as spicy on the live site).
- **Delivery partners** — Grubhub confirmed (direct listing URL:
  `https://www.grubhub.com/restaurant/the-taco-stand-670-n-milledge-ave-athens/1675228`).
  Uber Eats and DoorDash availability for The Taco Stand was NOT confirmed from research. Links on the site currently point to each platform's homepage — replace with direct merchant links or remove entirely if The Taco Stand isn't on those platforms.
- **Which location is on Grubhub** — the Grubhub listing is specifically the Milledge Ave location. If other locations have their own listings, add them; if not, note on `order.html` that delivery is Milledge-only.
- **Social media** — the Milledge and Eastside Facebook pages were found (`facebook.com/tacostandmilledge/`, `facebook.com/tacostandeastside/`). Instagram / TikTok were not surfaced. Confirm or add.

## External URLs used (verify before go-live)

- **Milledge Facebook:** https://www.facebook.com/tacostandmilledge/
- **Eastside Facebook:** https://www.facebook.com/tacostandeastside/
- **Grubhub (Milledge):** https://www.grubhub.com/restaurant/the-taco-stand-670-n-milledge-ave-athens/1675228
- **Google Maps directions links** — built with `destination=...` query on `visit.html`. Work as-is, no API key needed, but you may prefer embedded maps (iframe) per location.

## Maps

No embedded maps yet. If the client wants them on `visit.html`, add a Google Maps iframe per location under each `.location-card`.

## Copy decisions made without a client source

- Headline: "Real street tacos. Ordered at the counter." — original, fits the fast-casual brief. Confirm.
- Tagline: "Real street tacos. Since 1977." — original. Confirm.
- "Open late. Every day." headline on home location strip — we used this based on Milledge's 9:30p close. If the client doesn't consider 9:30p "late," swap the line.
- Order page copy ("Walk in. Scan the board. Say the thing." etc.) — punchy, original, matches the brand brief. Confirm voice is acceptable.

## Source pages referenced

Content pulled on 2026-04-20 from:
- https://www.thetacostandathens.com/ (official)
- https://menuguide.com/GA/Athens/The-Taco-Stand
- https://www.allmenus.com/ga/athens/743441-the-taco-stand/menu/
- https://www.tripadvisor.com/Restaurant_Review-g29209-d642327-Reviews-The_Taco_Stand-Athens_Georgia.html
- https://www.tripadvisor.com/Restaurant_Review-g29209-d1143465-Reviews-The_Taco_Stand-Athens_Georgia.html
- https://www.yelp.com/biz/taco-stand-athens
- https://www.yelp.com/biz/the-taco-stand-athens-2
- https://www.redandblack.com/guides/guides_athens_restaurants/taco-stand/article_81bac9a4-6ad5-11e6-8f07-6ff4899330d9.html
- https://www.visitathensga.com/listing/taco-stand/143/
- https://www.facebook.com/tacostandmilledge/
- https://www.facebook.com/tacostandeastside/
