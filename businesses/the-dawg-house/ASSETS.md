# The Dawg House — Asset Requirements

Content was researched from the live site (https://www.petboarddaycaregroomathens.com) and associated listings on 2026-04-20. Placeholder blocks are in place throughout. Here's what we need from the client to ship the final site.

## Photography

All placeholders are styled `<div>` blocks with descriptive labels. Replace each with a real image in a new `assets/` subfolder.

### Priority 1 — Home (`index.html`)
The homepage was restructured around the **day-in-the-life schedule timeline** and a **pricing-by-size table**, so it is now largely photo-free. The only hero mark is an inline SVG paw. If the client wants imagery later, these would still be the high-value shots to commission:

- **`assets/open-floor-plan.jpg`** — Interior wide shot showing the open-floor-plan concept (sofa, big windows, dogs hanging out). The signature differentiator — still valuable if added as a breakout block between timeline and pricing. **Target:** 1100×1400px.
- **`assets/hero-play-yard.jpg`** — A warm, wide shot of dogs playing in the outdoor yard. Could replace/augment the SVG paw mark in the compressed hero. **Target:** 1200×1500px.
- Per-timeline-row photos (9 small images, e.g. 400×300px) would be a stretch goal to make the schedule visual — NOT required, schedule reads well as typography-only.

### Priority 2 — Service pages
- **`assets/boarding-kennel.jpg`** — Inside a comfy private kennel with plush bedding. Shows the "upscale" boarding claim. (`boarding.html`)
- **`assets/daycare-play.jpg`** — Multiple dogs in the yard, clearly supervised. (`daycare.html`)
- **`assets/grooming-in-action.jpg`** — A groomer (Lisa or another team member) at the table working on a dog. Candid, not staged. (`grooming.html`)
- **`assets/cat-playroom.jpg`** — Optional second photo for the daycare page to support the cat daycare block.

### Priority 3 — Nice to have
- **`assets/owner-lisa.jpg`** — Portrait of owner Lisa Vogt, ideally with a dog. Would elevate the "Why Athens trusts us" strip into a real human story.
- **`assets/staff-group.jpg`** — Team photo. Trust-builder.
- **`assets/exterior.jpg`** — Current exterior of 380 Macon Hwy so first-time clients recognize it. Could go on `visit.html` next to the map.
- **`assets/logo.svg`** — Proper vector logo to replace the `The Dawg House` text wordmark in the header.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons (current files were carried over from the placeholder build).

## Maps

Google Maps embed is stubbed as a placeholder block on `visit.html`. Replace with an `<iframe>` embed:

```html
<iframe
  src="https://www.google.com/maps/embed?pb=..."
  width="100%" height="100%" style="border:0;"
  allowfullscreen loading="lazy"
  referrerpolicy="no-referrer-when-downgrade"></iframe>
```

Get the embed code from **Google Maps → Share → Embed a map** for **380 Macon Hwy, Athens, GA 30606**.

## Form wiring

`visit.html` has a booking-inquiry form stubbed with an `alert()` on submit. Before launch, wire it to one of:

- **Formspree** or **Netlify Forms** (easiest — change the `<form>` `action` attribute, drop the `onsubmit` handler)
- A lightweight serverless endpoint that emails `office@thedawghousepetresort.com`
- A booking platform integration (see below)

## Content gaps to confirm with the client

### Pricing — high priority
**All prices on the site are placeholders (`$ —`).** The live source site does not publish prices publicly. Confirm current amounts and replace in `index.html` (home pricing-by-size table), `boarding.html`, `daycare.html`, and `grooming.html`:

- **Home pricing table** (`index.html`) — a 4-size-bracket grid (Toy/Small <25 lb, Medium 25–50 lb, Large 50–90 lb, Giant 90+ lb) across five services: Daycare day pass, Daycare 10-pack, Boarding per night, Full groom, Bath & brush. **Confirm the size brackets themselves** — we invented the lb cutoffs as reasonable defaults, the live site may use different boundaries.
- **Boarding** — nightly rate by size (small / medium / large), second-pet same-family rate, cat boarding rate, and the exact extended-stay discount threshold + percentage (live site mentions "longer than 14 days").
- **Daycare** — full-day rate, half-day rate, 5-day package, 10-day package, and any other tiers. The live site explicitly mentions `Groom Day Stay & Play` as "just $5 more if a pet is getting a trim" — that one we kept.
- **Grooming** — starting prices for full, mini, outline, bath+brush, de-shed, plus each spa add-on (blueberry facial, teeth brush, pawdicure, massage, nail trim).
- Cat grooming rates, and whether guinea pig / rabbit grooming is still offered (Yelp/search snippets mention it).

### Day-in-the-life schedule — confirm operational details
The home page now leads with a 9-row timeline (7:00 AM → 7:00 PM) describing a typical day at the facility. We invented the timestamps and activity descriptions based on common boarding/daycare operations. Before launch confirm each row with the client:

- 7:00 AM morning potty break, 8:00 AM breakfast in suites, 9:00 AM group play start, 11:30 AM quiet time, 12:30 PM lunch (by request), 1:00 PM afternoon play, 3:30 PM one-on-one enrichment, 5:00 PM dinner, 7:00 PM final potty / lights dim.
- Specifically: is there overnight staff on premises (we say yes), or is the building monitored remotely? Adjust the 7:00 PM row accordingly.
- Are meals really served in "individual suites," or in a common feeding area?
- Is there actually a structured quiet time at 11:30, or is it more organic?

### Holiday policy
The live site mentions holiday surcharges implicitly (popular weekends book up). Confirm:
- Are there holiday surcharge rates for Thanksgiving / Christmas / New Year?
- Any blackout or deposit policies for peak weekends?
- UGA home-game-weekend boarding policies (mentioned on site).

### Vaccination requirements — minor confirmations
We list **Rabies, Bordetella, DHPP** (from search results). Confirm:
- Do cats need specific vaccines (FVRCP, Rabies)? Not referenced in what we found.
- Minimum age requirement for daycare / boarding puppies?
- Is Canine Influenza (CIV) required or recommended?
- Spay/neuter — we listed "Recommended for dogs over 6 months in group play" as a safe default. Confirm the actual policy.

### Drop-off / pick-up windows
Sunday hours are split (8–10 am and 4–6 pm per the live site). Confirm:
- Is there a formal check-in window on other days, or is any time during open hours fine?
- Are Sunday windows drop-off-only, pickup-only, or either?
- Late-pickup fee structure?

### Team / staff bios
Owner **Lisa Vogt** is named in search results (UGA alumna, groomer since 2001, NuVet Certified Pet Groomer since 2006). We reference her once in a testimonial ("Lisa and the team"). Worth asking:
- Short bio for Lisa on an About page or homepage?
- Other groomers and boarding staff — names, years of experience?
- Would the shop want to add an `about.html` page for this? We intentionally kept to 5 pages for scope, but the founder story is strong.

### Email address
Two emails appeared in research:
- `office@thedawghousepetresort.com` (primary, Yelp/BBB/website)
- `dawghousegroom@gmail.com` (mentioned as a vaccination-record inbox in one search result)

We used the first everywhere. Confirm this is the right one, or whether vaccination records should route to the gmail.

### Testimonials
Current testimonials on the site are **paraphrased composites** from review snippets we saw (e.g. "16-year client," "royal treatment"). Before launch, get explicit permission to quote real clients with names, or lift verbatim 5-star reviews from Google / Yelp with attribution.

### Online booking
Currently walk-in / call-in only. Confirm whether the client wants a booking integration added later:
- **Gingr**, **Revelation Pets**, **ProPet** — industry-standard boarding / daycare software
- **Square Appointments** or similar for grooming only

### Social / review links
- Instagram: `@dawghousegroom` (confirmed)
- Facebook: `dawghouseboardingdaycaregrooming` (confirmed)
- Google Business Profile / review link — currently not linked in footer. Ask for the URL.

## Copy to double-check

Content was extracted from search-engine snippets of the live site on 2026-04-20 (direct WebFetch was unavailable during build). Before going live:

- Confirm the tagline "Your dog's second home." — that's our phrasing, not copy from the live site
- Confirm the "Since 2006" claim (consistent across all sources)
- Confirm the phone number (706) 355-9911 — this is consistent across Yelp, BBB, pethotels.com, and the live site
- Confirm the address 380 Macon Hwy, Athens, GA 30606
- Confirm the "20+ years in Athens" trust-strip stat (2006 founding → accurate as of 2026)
- Confirm that we correctly represent the "open floor plan, visible from sales floor" concept as a differentiator
- Confirm we can say "Athens' largest and oldest facility" (direct phrasing from live site meta copy)
- Confirm "we groom all sizes and breeds of dogs, cats, guinea pigs, and rabbits"

## Out of scope (ask if client wants)

- `about.html` with owner story, staff bios, facility history
- `cat-boarding.html` and `cat-grooming.html` dedicated subpages (the live site has them; we folded them into the main pages for simplicity)
- Boarding webcams / livestream ("the open floor plan" is similar in spirit — if cams exist, we'd want to feature them)
- Blog / news section for holiday hours, rate changes, tips
