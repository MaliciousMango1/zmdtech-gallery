# The Master's Table — Asset Requirements

Placeholder tiles, a map placeholder, and an inquiry form stub throughout. Here's what we need from the client.

## Photography

The homepage signature is a six-tile **event portfolio gallery** — those tiles are the highest-value photo slots on the site. Each placeholder has a `data-label` on the `.tile-photo` div indicating what should replace it. Replace each CSS-gradient placeholder with a real photo in a new `assets/` subfolder.

### Priority 1 — Homepage portfolio gallery (`index.html`)

The six tiles, in grid order:

- **`assets/portfolio/weddings.jpg`** — Reception head table. Ivory linens, gold chargers, floral centerpiece, candlelight. No guests in frame. **Target:** 1200×1200px, square.
- **`assets/portfolio/corporate.jpg`** — Corporate buffet line. White napery, chafing dishes, neutral crowd or empty setup. **Target:** 1200×1200px.
- **`assets/portfolio/rehearsal.jpg`** — Rehearsal dinner long table. Candles, family-style platters, Southern spread. **Target:** 1200×1200px.
- **`assets/portfolio/graduations.jpg`** — Backyard graduation party. Pulled pork buffet, banners, daylight. **Target:** 1200×1200px.
- **`assets/portfolio/holiday.jpg`** — Holiday buffet. Turkey and sides, garland runner, dim-warm lighting. **Target:** 1200×1200px.
- **`assets/portfolio/brunch.jpg`** — Brunch biscuit bar or grits station. Morning light, coffee service visible. **Target:** 1200×1200px.

Once real photos are in, remove the `.tile-pill` labels and the CSS `.tile-photo` gradients, and swap in `<img>` tags.

### Priority 2 — About page (`about.html`)

- **`assets/kitchen-1984.jpg`** — Archival or present-day shot of the Kelly Drive kitchen. Portrait orientation. **Target:** 1000×1250px. Currently a full-bleed olive/wine gradient placeholder.
- **`assets/team/owners.jpg`** — Headshot or working shot of the owners. Only needed if they're comfortable being shown.
- **`assets/team/chef.jpg`** — Executive chef on the line.
- **`assets/team/event-lead.jpg`** — Event coordinator.

### Priority 3 — Nice to have

- **`assets/food/`** — 6 to 10 plated food shots for a future menu-page gallery. Low country boil, fried chicken, peach cobbler, biscuit bar, tenderloin biscuits, etc.
- **`assets/logo.svg`** — Proper vector logo to replace the Forum wordmark in the header/footer.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons.

## Maps

Placeholder is in `visit.html`. Replace with a Google Maps iframe embed for **80 Kelly Drive, Winder, GA 30680**.

## Forms

The quote form on `index.html#quote` currently triggers `alert()` on submit. Wire to send to **Cateringbythemasterstable@yahoo.com** with subject prefix `[Quote Request]` via Cloudflare Pages Functions + an email backend (Resend, Postmark), Formspree, or a Google Form embed. Recommend consolidating the Yahoo address into a modern domain-hosted inbox as part of the handoff.

## Content to confirm with client

- **Founding year — 1984.** Pulled from chamber / directory listings. Current About timeline and all footers/headers say "Est. 1984." Confirm.
- **Owner names.** Not published anywhere we could find. The Team section has a generic "Ownership — Family operators" card with a placeholder note. Need real names (or confirmation they'd rather stay anonymous in copy).
- **Team photos and names for chef + event lead.** Both currently generic.
- **Timeline milestones.** All five dated milestones (1984, 1992, 2003, 2014, 2024) are plausible but invented. Ask the client to correct the dates and the narrative for each.
- **"42 years catering" + "214 events in 2014"** stats in the About page are estimates; confirm numbers or replace with real figures.
- **Pricing — every per-guest price on `menus.html` and `index.html` is estimated** based on the current live site's pricing pattern ($9–$10/person buffets from 2000s-era pricing, adjusted forward). The live site lists 1-meat + 4 sides at $9 and 2-meat + 4 sides at $10, which are clearly undervalued and likely out of date. All new prices ($14 boxed lunch up to $48 plated three-course) need client sign-off before publishing.
- **Menu contents.** Heritage Buffet, Plated Three-Course, Heavy Hors d'Oeuvres, Low Country Boil, Southern Supper, Holiday, Brunch, etc. — drawn from WeddingWire review mentions (beef tips, parmesan chicken, creamed corn, au gratin potatoes, broccoli casserole, mac & cheese, green beans, rolls, sweet potato casserole, corn casserole) and standard Southern catering patterns. Confirm every dish.
- **Guest range.** We wrote "10 – 500" and "75 minimum for plated." Confirm.
- **Region coverage.** We wrote "Barrow, Jackson, Clarke, greater Athens, metro Atlanta on request." Confirm delivery radius.
- **Office hours.** We used a reasonable Mon–Fri 9–5 pattern (Fri 9–3). Confirm.
- **Service capabilities.** We mentioned: full staff, rentals, bar service coordination, chafing dishes, smoker, dual convection ovens, ServSafe-certified management. Confirm what they actually offer vs. subcontract.
- **Faith-based framing.** Chamber listings describe the business as faith-based. We kept it light ("built on faith, family recipes") in the About page. Confirm tone is right.
- **"We do not accept credit or debit cards" note on the current site.** We removed this. Confirm whether they now accept cards; if not, we need to add a note to the quote form.
- **Past client list.** WeddingWire reviews mention 200-guest weddings and strong service reviews. No specific venues or clients cited. If the client is comfortable listing past venues (churches, country clubs, barns) that would strengthen the About page.

## Copy to double-check

Content was drafted on 2026-04-20 from chamber listings, WeddingWire reviews, The Knot profile, and the current live site (cateringbythemasterstable.com). Before going live:

- Confirm address: 80 Kelly Drive, Winder, GA 30680
- Confirm phone: (770) 867-8540
- Confirm email: Cateringbythemasterstable@yahoo.com (recommend migrating off Yahoo)
- Confirm every menu item and per-guest price on `menus.html`
- Confirm timeline dates and owner/team names on `about.html`
- Confirm all six portfolio tile labels on `index.html` match event types they actually cater
