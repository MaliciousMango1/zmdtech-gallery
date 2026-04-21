# Mr. Haircut — Asset Requirements

Placeholder blocks are in place throughout the site. Here's what we need from the client to swap them in.

## Photography

All placeholders are styled blocks with labels describing what goes there. Replace each with a real image in a new `assets/` subfolder.

### Priority 1 — Hero / Home (`index.html`)
- **`assets/hero-interior.jpg`** — A warm, wide shot of the shop interior. The chairs, the mirrors, the barber's station. Midday natural light if possible. **Target:** 1200×1500px, portrait orientation.
- **`assets/about-archive.jpg`** — Either a vintage exterior photo of the original Flat Top Barber Shop OR a current exterior shot of the corner of Broad & Jackson. Helps the "since 1968" story land. **Target:** 1000×1250px.

### Priority 2 — About page (`about.html`)
- **`assets/history-exterior.jpg`** — Vintage or current exterior of 295 E Broad St. Storefront signage visible ideally.
- **`assets/chair-interior.jpg`** — A barber at work, or a close-up of a chair + tools. Candid, unposed is better than staged.

### Priority 3 — Nice to have
- **`assets/barbers-group.jpg`** — Team photo of the barbers (with permission). Adds trust and humanizes the "all-women barbers" angle.
- **`assets/logo.svg`** — A proper vector logo to replace the `MR. HAIRCUT` text wordmark in the header. Current favicon is placeholder.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons (current files were carried over from the placeholder build).

## Maps

Google Maps embeds are stubbed as placeholder blocks on `index.html` and `visit.html`. Replace each with an `<iframe>` embed:

```html
<iframe
  src="https://www.google.com/maps/embed?pb=..."
  width="100%" height="100%" style="border:0;"
  allowfullscreen loading="lazy"
  referrerpolicy="no-referrer-when-downgrade"></iframe>
```

Get the embed code from [Google Maps → Share → Embed a map] for **295 E Broad St, Athens, GA 30601**.

## Other gaps to confirm with client

- **Email address** — not shown on the live site. Ask if there's a shop email for inquiries (e.g., product availability, press, private events).
- **Online booking** — live site is walk-in only. Confirm this is staying that way, or whether they'd want a booking integration (Booksy, Fresha, Square Appointments).
- **Google Reviews link** — currently stubbed to `#` in the footer. Get the real review URL or Google Business profile link.
- **UGA home-game closure dates** — mentioned as a rule but no specific dates. A seasonal banner could be worth adding in football months.
- **Product brands beyond Suavecito** — the live site mentions "variety of products" but only specifies Suavecito. Ask for the current product lineup to refine the services page.
- **Barber bios** — optional, but a short "meet the team" section on the About page with names + years of experience would add trust if the shop is comfortable sharing.

## Copy to double-check

Content was extracted from the live Wix site on 2026-04-20. Before going live:
- Confirm prices (we used the live site's list verbatim)
- Confirm hours
- Confirm the founding story (Duncan brothers → Pam Mullins 1994)
