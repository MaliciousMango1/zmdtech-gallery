# Moma Punkin's Place — Asset Requirements

This business does not currently have a real website. The domain `momapunkinsplace.com` resolves to a food-delivery aggregator landing page for catering orders, not a site the owner actually controls. Every lead they get today is mediated by that aggregator. **This is the pitch: a first real website they own, with a direct customer relationship and no middleman.**

Placeholders throughout use `$ —` for unknown prices/contact details per gallery convention. Below is what we need from the client before launch.

## Location discrepancy — please confirm

The build spec called for **Greensboro, Georgia**. Public listings (Yelp, the aggregator site) associate Moma Punkin's Place with **Greensboro, North Carolina** and a Statesville, NC commissary at 224 Turnersburg Hwy. We built the site as **Greensboro, GA 30642** as specified. Before launch, **confirm which Greensboro** the client operates in and update:

- All four pages' brand subtitle ("Greensboro, Georgia")
- `index.html` masthead eyebrow
- `index.html` info strip address ("Greensboro, GA 30642")
- Footer address on all pages
- `visit.html` contact card address
- `catering.html` service-area counties (we used Greene/Putnam/Morgan/Hancock/Oconee — these are the GA counties around Greensboro, GA)
- Page meta descriptions and `<title>` tags
- `catering.html` service-area counties (swap for NC counties if it's actually Greensboro, NC — likely Guilford / Forsyth / Alamance / Rockingham)

## Content to confirm

### Contact details (all currently `$ —` placeholders)

- **Street address** — used `$ — street address` in every footer, info strip, and the Visit card
- **Phone number** — `tel:+10000000000` placeholder on every page. Replace with real number
- **Email** — used `hello@momapunkinsplace.com` as a reasonable placeholder. Confirm the real address (might need to be a Gmail until they set up email on the domain)

### Owner / family story

- We did not include an "about" / owner story. The brand leans on warmth implicitly but the "family-run" tagline is thin without a name. Ask the owner:
  - Who is "Moma Punkin"? (Nickname? Real person? Grandmother?)
  - Who's running the kitchen day-to-day?
  - Would they want a short "from the family" paragraph on the homepage or Visit page?

### Menu

- Menu items on `menu.html` and the homepage "daily table" are a reasonable Southern-soul-food baseline. **Every item and price needs to be confirmed with the client.** Add seasonal items, remove anything they don't actually serve.
- All prices currently show `$ —`. Replace with real prices.
- Confirm whether plates come with cornbread and a drink, or whether those are à la carte.
- Confirm pint / quart pricing for sides and vegetables.

### Hours

- Placeholder hours: Tue–Sat 11 am–8 pm, Sun 11:30 am–6 pm, closed Monday. This is typical for a Southern kitchen but **must be confirmed** — delivery aggregator listings showed different hours (Mon–Sun 10 am–8 pm pickup, Sun 11:30 am–7 pm delivery) which look like aggregator operating windows rather than restaurant hours.

### Catering packages

- Three tiered packages ("Sunday plate" / "Family table" / "The big spread") plus "By the pan" are invented structures. Confirm whether the client actually offers tiered packages or prefers fully custom quoting.
- All per-person prices are `$ —`. Replace.
- Minimums (15 / 25 / 50) are assumptions based on typical soul-food caterer norms.
- **Lead time** — we said 48 hours for most orders, a week for 75+ person events. Aggregator listing mentions "48-hour turnaround for custom orders" which we incorporated. Confirm.
- **Deposit** — 25% on booking is an assumption. Confirm their actual terms.
- **Service area** — see location discrepancy above.

### Dine-in vs. take-out only

- We wrote the Visit page as "dine in if we have the room, take-out otherwise." This is a safe framing if they run a small kitchen / commissary without formal dining. **Confirm whether they actually have any dine-in seating** — if it's catering + take-out only, we should remove "dine in" language from masthead lede, info strip, and Visit copy.

## Photography

Replace placeholder blocks with real images in a new `assets/` subfolder. We intentionally kept this design light on photos — the "daily table" text columns and green catering band do not need hero imagery. But a handful of good shots would lift the site:

### Priority 1

- **`assets/plate.jpg`** — One good plate (fried chicken, greens, mac, cornbread) on a simple surface. Would go above or below the masthead. **Target:** 1600×1000px, landscape.
- **`assets/pans.jpg`** — Chafing dishes or full-pan spread at an actual event. The money shot for the Catering page. **Target:** 1600×1000px, landscape.

### Priority 2

- **`assets/kitchen.jpg`** — Someone cooking. Hands in the pan, stovetop, real work. Adds the "family-run" feel without being posed. **Target:** 1200×1500px, portrait.
- **`assets/banana-pudding.jpg`** — Signature dessert close-up. **Target:** 1000×1000px, square.
- **`assets/storefront.jpg`** — Exterior with signage (if they have a storefront). **Target:** 1600×900px, landscape.

### Priority 3

- **`assets/logo.svg`** — A proper vector logo to replace the Libre Baskerville italic wordmark in the header/footer.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons.

## Map

Placeholder is in `visit.html`. Replace with a Google Maps iframe embed for the confirmed street address once we have it.

## Forms

Two catering inquiry forms:
- Homepage `index.html` (section 3, collard-green band — 4 fields: name, event date, guest count, message)
- Catering page `catering.html#inquire` (expanded — name, phone, date, guests, email, message)

Both currently trigger `alert()` on submit. Before launch, wire to send to the confirmed email address with subject prefix `[Catering Inquiry]` via Cloudflare Pages Functions + an email backend (Resend, Postmark), Formspree, or a simple Google Form embed. The point of this site is lead capture — these forms need to work reliably before we go live.

## External integrations

The live aggregator listing (`momapunkinsplace.com`) is currently where all their orders flow. Decisions to make with the client:

- **Do we redirect that domain** once the new site launches, or is the current listing on a sub-path they don't control?
- **Online ordering** — if they want take-out ordering on the real site, we'll need to wire up Toast / Square / ChowNow / a simple Stripe order form. Not built into this version; the site is catering-inquiry-first by design.
- **Delivery aggregators** (DoorDash, Uber Eats, Grubhub) — if they're listed on these, we could link them from the Visit page. None are linked currently.

## Social

- TikTok: `@momapunkinsplace` exists. Instagram / Facebook unconfirmed. Add social links to the footer once confirmed.

## Copy to double-check

Content was written on 2026-04-20 based on public listings. Everything voice-and-tone was kept plainspoken and warm per brief ("We cook what our grandmother cooked", no "artisan", no marketing hype). Before going live, read through with the owner to make sure the voice feels like theirs and nothing overpromises.
