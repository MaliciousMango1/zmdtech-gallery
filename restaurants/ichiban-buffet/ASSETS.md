# Ichiban Buffet — Asset Requirements

The home page is text and table-forward on purpose — there are no photo placeholders on `index.html`. The only visual placeholder in the build is the map block on `visit.html`. Almost every ask below is **content confirmation** rather than design production.

## Pricing — the #1 gap

The homepage pricing matrix is the signature section. We only have two verified prices. Everything else is `$ —` and needs to be filled in from the current printed menu or the register sign.

| Row | Adult | Senior (60+) | Child (under 10) | Under 3 |
|---|---|---|---|---|
| Lunch Buffet (Mon–Fri until 3:30) | **$7.50** (confirmed) | $ — | $ — | Free |
| Dinner Buffet (after 3:30, weekdays) | **$10.50** (confirmed) | $ — | $ — | Free |
| Weekend & Holiday (all day Sat & Sun) | $ — | $ — | $ — | Free |
| Drink add-on | $ — | $ — | $ — | $ — |

Also confirm:
- Is "Senior" really 60+ or is it a different age (55? 65?)?
- Is "Child" really under 10 or a different age (under 12 is more common)?
- Is "Under 3" actually free? Plausible but not verified.
- Does lunch pricing cut off at 3:30 or a different time?
- Is weekend pricing flat all day or does it also have a lunch/dinner split?

## Menu confirmation

Menu items were pulled from DoorDash, Yelp, Tripadvisor, and customer reviews. Every item on `menu.html` needs to be checked against the current printed menu:

**Verified prices (from DoorDash listing):**
- Cheese Wonton — $6.50
- Dumplings — $7.49
- Sesame Chicken Combo — $11.99
- General Tso's Chicken Combo — $11.99
- Orange Chicken Combo (price not captured; listed as available)

**Plausible-but-unconfirmed items we included:** Mongolian beef, pepper steak, sweet & sour pork, coconut shrimp, kung pao chicken, California roll, spicy tuna roll, salmon nigiri, shrimp tempura roll, avocado roll, chef's special roll, tuna nigiri, lo mein, chow mein, Singapore noodles, udon, hibachi vegetables, egg roll, spring roll, egg drop soup, hot & sour soup, miso soup, fried shrimp, sugar donuts, soft-serve, ice cream bars, jello, pudding, fortune cookies.

Have the client cross off anything they don't serve, add anything missing, and fill in every `$ —`.

## Business facts to confirm

- **Address:** 78 E May St, Suite A, Winder, GA 30680
- **Phone:** (678) 975-7673
- **Hours:** Mon–Thu 11:00 AM – 9:30 PM · Fri & Sat 11:00 AM – 10:30 PM · Sun 11:00 AM – 9:30 PM
- **Online ordering:** https://ichibanbuffetga.kwickmenu.com/ (linked as "Order online" in every header and footer)

## Photography — if they want it later

The current design intentionally uses no photos on the home page. If the client wants a small photo dressing, we would add **one** of these — and only one, to avoid cluttering the paper-white layout:

- **`assets/sushi-bar.jpg`** — Overhead shot of the sushi bar in service, fresh rolls being plated. 1400×900 landscape.
- **`assets/wok-line.jpg`** — Steam over the hot wok steam table with serving tongs. 1400×900.
- **`assets/interior.jpg`** — Wide dining room shot during a mid-service lunch. 1400×900.

A proper **`assets/logo.svg`** and **`assets/favicon.svg`** would replace the Tenor Sans wordmark in the header and the missing favicon. Low priority — the wordmark reads fine as-is.

## Map

Placeholder is in `visit.html`. Replace with a Google Maps iframe embed for **78 E May St, Winder, GA 30680**.

## Catering form

The inquiry form on `catering.html` triggers `alert()` on submit. Wire to send to the restaurant's business email (not yet known — confirm with client) with subject prefix `[Catering Inquiry]` via Cloudflare Pages Functions + Resend, Formspree, or a Google Form embed.

## External integration to confirm

- **KwickMenu** online ordering — https://ichibanbuffetga.kwickmenu.com/ — confirm the URL is still live and that the restaurant wants it as the primary "Order online" destination (alternative: DoorDash at https://www.doordash.com/store/ichiban-buffet-24858437/).

## Content research sources

Data collected on 2026-04-20 from:
- winderichiban.com (live site — referenced for business facts)
- DoorDash listing (menu items + the four verified prices)
- Yelp, Tripadvisor (address, phone, hours, customer-reported prices)
- Facebook (winderichiban)
- KwickMenu page header ("OVER $50: 10% OFF" promo noted — confirm if still active)
