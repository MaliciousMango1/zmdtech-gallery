# Trumps Catering — Asset Requirements

Demo site has no photography. All visual blocks are placeholder patterns with `data-label` tags. Values flagged `<span class="flag">verify</span>` in the HTML are unconfirmed. Here's what we need from the client before launch.

## Photography

Create an `assets/` subfolder and replace placeholders.

### Priority 1 — Home (`index.html`)
The homepage is intentionally photo-free in this demo (masthead is typographic, taxonomy cells are solid-color panels). If the client wants imagery, we recommend:
- **`assets/taxonomy-weddings.jpg`** through **`assets/taxonomy-cocktail.jpg`** — six tight crops, one per taxonomy cell. 800×600px minimum. Shown behind a darkening overlay on hover.
- **`assets/masthead-table.jpg`** — optional full-bleed shot of a set table, banquet or wedding. Currently the masthead is clean typography only.

### Priority 2 — About (`about.html`)
- **`assets/about-portrait.jpg`** — Kitchen or team portrait to replace the striped placeholder. Horizontal crop or 4×5 portrait. Andrée and Ron together would be ideal.
- **`assets/team-andree.jpg`**, **`assets/team-ron.jpg`**, **`assets/team-chef.jpg`** — headshots (or kitchen action shots) for the three team cards. 600×600px minimum.

### Priority 3 — Menus (`menus.html`)
- Optional header shots for each menu format (buffet spread, plated course, canapé tray, box lunch). Improves scanability but not required.

### Priority 4 — Nice to have
- **`assets/ballroom-milledge.jpg`** — the on-Milledge ballroom at setup. Shows the domed fiber-optic ceiling.
- **`assets/ballroom-georgian.jpg`** — the Historic Georgian ballroom.
- **`assets/logo.svg`** — proper vector logo. Currently using a typographic wordmark (`Trumps.`) in IBM Plex Serif.

## Maps

`contact.html` uses a placeholder map block. Replace with a Google Maps iframe embed for **2026 S Milledge Ave, Suite B, Athens, GA 30605**.

## Forms

The inquiry form on `index.html#inquire` currently triggers `alert()` on submit. Wire to:
- Destination: **info@trumpscatering.com** (confirm this is the right inbox — live site's contact page should be cross-checked)
- Subject prefix: `[Inquiry – {event_type}]`
- Backend options: Cloudflare Pages Functions + Resend/Postmark, Formspree, or a direct SMTP relay
- Honeypot + rate-limiting recommended given the public `tel:` link

## Content to confirm with client

Everything flagged `verify` in the HTML needs client sign-off. Summary:

### Business facts
- **Founded 1986** — confirmed by multiple sources (Explore Georgia, visitathensga.com, Wheree). "40 years" is accurate as of 2026.
- **Founders** — Ron Schwartz and Andrée Kosak. Pulled from LinkedIn. Confirm spelling of "Andrée" (with acute accent).
- **Executive Chef** — not listed publicly. Need name and a line of bio for the About page team card.
- **Phone** — (706) 546-1320. Confirmed via Yelp and visitathensga.com.
- **Email** — `info@trumpscatering.com` is a placeholder. The live Squarespace contact page uses a form, not a visible email. Confirm the correct address.
- **Address** — 2026 S Milledge Ave, Suite B, Athens, GA 30605. Confirmed via Yelp.
- **Hours** — Mon–Fri 9–5 (office) confirmed. Saturday "by appointment" and Sunday closed are assumed — confirm.

### Capacity and venue claims
- **Ballroom on Milledge capacity: 225** — per Eventective listing.
- **Historic Georgian ballroom capacity** — unlisted. Need a number.
- **"30+ event staff on call"** in About `By the numbers` — placeholder. Confirm actual bench size.
- **"1,500+ weddings"** in About — reasonable for 40 years at ~40/year but not a real figure. Replace with a real tally or remove the specific number.

### Menu items and pricing
- Every menu item on `menus.html` is a reasonable guess informed by client reviews ("mashed potato bar," "sweet corn soufflé," "carved beef tenderloin," "fried chicken with white cheddar and green onion grits," "cupcakes with caramel filling and buttercream") — but the full menu lists need client approval.
- **No prices are real.** Every price shows `$—` with a `verify` flag. Fill with actual per-guest starting prices or keep as "inquire for pricing" if the client prefers that posture.
- Confirm minimums listed in the Contact page FAQ (15 box lunches, 40 buffet/plated, 50 cocktail).

### Press and testimonials
- All four quotes on the About page are **placeholders** marked `verify`. Pull real testimonials from:
  - WeddingWire (existing profile): https://www.weddingwire.com/biz/trumps-catering-athens/0ee47aea583c6de6.html
  - The Knot: https://www.theknot.com/marketplace/trumps-catering-athens-ga-339060
  - Google reviews
  - Flagpole, Online Athens, or UGA alumni publications for press coverage

### Copy tone
- Voice is B2B confident ("We've done 1,500 weddings and counting. You'll be in good hands."). Confirm the client is comfortable with this posture — it's more direct than the current Squarespace brochure copy.

## External links to confirm

- Current Squarespace site: https://www.trumpscatering.com/ — confirm all content has been superseded before launch.
- Facebook: https://www.facebook.com/TrumpsCatering/
- Instagram: https://www.instagram.com/trumpscatering/
- LinkedIn: https://www.linkedin.com/company/trumps-caterings

Social links are not currently in the footer. Add if the client wants them.

## Content extracted from

- trumpscatering.com (primary) — via search snippets; WebFetch was disabled during build, so extraction is from search summaries
- visitathensga.com, exploregeorgia.org, Yelp, WeddingWire, The Knot, Eventective, PartySlate, LinkedIn — cross-referenced 2026-04-20
