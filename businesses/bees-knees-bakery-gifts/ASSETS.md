# Bee's Knees Bakery & Gifts — Asset Requirements

Placeholder photo blocks and a map placeholder are in place throughout the site. Here's what we need from the client to swap them in.

## Photography

Replace each placeholder block with a real image in a new `assets/` subfolder.

### Priority 1 — Home (`index.html`)
- **`assets/hero-cake.jpg`** — A signature cake on a clean, warm-lit surface. Should feel inviting and polished — hero shot of the bakery's craft. **Target:** 1200×1500px, portrait orientation.
- **`assets/cat-sweets.jpg`** — Wide shot of the cupcake display case. Shows variety, colors, daily abundance. **Target:** 1000×750px.
- **`assets/cat-custom.jpg`** — A standout custom birthday or celebration cake. Should show design/decoration work. **Target:** 1000×750px.
- **`assets/cat-wedding.jpg`** — A tiered wedding cake, ideally from a recent event. **Target:** 1000×750px.
- **`assets/case-full.jpg`** — The cupcake case with fresh cupcakes visible in multiple flavors. **Target:** 1000×1250px.
- **`assets/cookies.jpg`** — Decorated iced butter cookies, close-up. **Target:** 1000×1250px.

### Priority 2 — Custom Cakes (`cakes.html`)
- **`assets/cookies-detail.jpg`** — Close-up of decorated cookies showing detail work and colors.

### Priority 3 — Weddings (`weddings.html`)
- **`assets/wedding-tier.jpg`** — Tiered wedding cake, ideally on a reception table with florals or in a bakery portfolio shot. **Target:** 1000×1250px.
- **`assets/wedding-gallery/`** *(optional)* — 6–12 additional wedding cake photos to populate a future gallery section.

### Priority 4 — Nice to have
- **`assets/logo.svg`** — A proper vector logo to replace the "Bee's Knees" italic wordmark in the header.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons (current files are placeholders).
- **`assets/bakery-exterior.jpg`** — Storefront / Epps Bridge Parkway exterior for the Visit page.
- **`assets/owner-baking.jpg`** — Candid behind-the-counter or decorating shot to humanize the "family-run" story on a future About page.

## Maps

A Google Maps embed is stubbed as a placeholder block on `visit.html`. Replace with an `<iframe>`:

```html
<iframe
  src="https://www.google.com/maps/embed?pb=..."
  width="100%" height="100%" style="border:0;"
  allowfullscreen loading="lazy"
  referrerpolicy="no-referrer-when-downgrade"></iframe>
```

Embed for **1850 Epps Bridge Pkwy, Ste 113, Athens, GA 30606**.

## Forms

Two forms are stubbed on `cakes.html` and `weddings.html`. Currently they display an alert on submit — in production, wire them to:

- **Cloudflare Pages Functions** with an email backend (Resend, Postmark, SendGrid), OR
- **Formspree / Netlify Forms** equivalent if we want no-code, OR
- **A Google Form embed** as a quick shortcut if the client prefers

Both forms should send to **beeskneesbakeryandgifts@gmail.com** with subject prefixes:
- Cakes form → `[Custom Cake Inquiry]`
- Weddings form → `[Wedding Consultation Request]`

## Other gaps to confirm with client

- **"Gifts" offering** — The business name includes "& Gifts" but the current live site lists no giftware products. Ask the owner: is this an in-store-only product line? Retired? Planned? If active, we should add a `gifts.html` page with categories (candles, gift baskets, seasonal, etc.).
- **About / Our Story** — The live site's "Our Story" page surprisingly shows the lunch menu, not a story. Ask the owner for 2–3 paragraphs on the bakery's origin, the baker(s), and what makes them tick. Would add a 6th page or a section on `index.html`.
- **Online ordering** — Live site references "Order Online" but links lead to broken pages. Confirm whether online ordering (via Square?) should be integrated. `bees-knees-bakery.square.site` exists but is empty.
- **Cupcake gallery / cake gallery** — A visual gallery would be strong for custom cake conversions. Ask for 20+ custom-cake photos to build a gallery section.
- **Holiday specials** — Pumpkin, hummingbird, and Italian cream flavors suggest Thanksgiving/Christmas/spring programs. Ask about seasonal releases we can feature.
- **Testimonials** — No testimonial copy is on the live site. Ask for 2–3 quotes from repeat customers or wedding clients.
- **Social media assets** — Instagram handle (@beeskneesbakeryathens) is linked. Confirm any additional platforms (TikTok, Pinterest for cakes).

## Copy to double-check

Content was extracted from the live GoDaddy site on 2026-04-20. Before going live:
- Confirm all prices (we used the live site's list verbatim)
- Confirm hours (currently Mon–Sat 10am–6pm)
- Confirm sandwich list and lunch pricing are still current
- Confirm cake flavor / filling / icing lists are complete (we listed every flavor on the live site)
- Confirm the "gifts" question above
