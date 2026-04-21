# Simpson Chiropractic Wellness & Weight Loss — Asset Requirements

Placeholder photo block for the clinician, a map placeholder, and a stubbed intake form. Here's what we'd need from the client to ship.

## Photography

Replace placeholder blocks with real images in a new `assets/` subfolder.

### Priority 1 — Home (`index.html`)
- **`assets/dr-simpson.jpg`** — Portrait of Dr. Tony Simpson. Warm, natural light, professional but approachable (clinic setting preferred over studio). **Target:** 1000x1250px, portrait (4:5).

### Priority 2 — Nice to have (no placeholder yet; add later if we want more visuals)
- **`assets/clinic-exterior.jpg`** — The 700 Hawthorne Ave storefront/entrance.
- **`assets/clinic-reception.jpg`** — Reception or waiting area, calm lighting, no identifiable patients.
- **`assets/treatment-room.jpg`** — Treatment or exam room, uncluttered, no identifiable patients.
- **`assets/team.jpg`** — Full team photo if the client wants to highlight staff beyond Dr. Simpson.
- **`assets/logo.svg`** — Proper vector logo to replace the Source Serif 4 wordmark.
- **`assets/favicon.svg`** and **`assets/favicon.ico`** — Real favicons.

## Maps

Placeholder is in `contact.html`. Replace with a Google Maps iframe embed for **700 Hawthorne Avenue, Athens, GA 30606**.

## Forms

The intake form on `new-patients.html#intake` currently triggers `alert()` on submit. Wire to send to the clinic's preferred inbox with subject prefix `[New Patient Request]` via Cloudflare Pages Functions + an email backend (Resend, Postmark), Formspree, or a HIPAA-aware form provider (JotForm HIPAA, Formstack HIPAA).

**Important:** Do not route PHI through a non-HIPAA-aware pipeline. The current form is limited to contact info + a free-text reason, which is intended to stay light — but confirm with the clinic what they're comfortable collecting before go-live.

## Content to confirm with client

- **Clinician name and preferred form** — Used "Dr. Tony Simpson" throughout (matches Google/Facebook/directories). Healthgrades and Vitals list him as **Dr. Anthony Simpson, DC**. Confirm which form he prefers publicly and whether to add "DC" after the name.
- **Years in practice** — Used "over 30 years" and "since the early 1990s" based on directory copy. Confirm exact year he opened the Athens practice.
- **Clinic email** — Not listed on the live site or any directory we found. Confirm whether to publish one on the contact page. The footer and contact page currently have no email address.
- **Additional clinicians** — Site currently assumes Dr. Simpson is the sole treating clinician. Confirm whether associates, acupuncturists, coaches, or massage therapists should be featured.
- **Services menu** — Research surfaced four service lines (chiropractic, neuropathy, weight loss, wellness with gut-health coaching). Confirm that's the complete list and that "gut-health coaching" is how they want to describe it.
- **Insurance list** — We listed BCBS of GA, United Healthcare, Aetna, Medicaid, and VA based on directory mentions. Confirm the full in-network list the clinic wants featured, and whether they want to call out specific exclusions.
- **CareCredit** — Mentioned on `contact.html#insurance` because Simpson Chiropractic Center has a CareCredit doctor-locator listing. Confirm they still accept it.
- **Hours** — Used live-site hours (Mon/Wed/Thu 8:45-5:30, Tue 10:30-5:30, Fri-Sun closed). Confirm.
- **Phone and fax** — (706) 543-1900 and (706) 543-1904 — confirm both still current.
- **Address** — 700 Hawthorne Avenue, Athens, GA 30606 — confirm current.

## Medical-claim language flagged for physician review

All service copy was written deliberately to avoid outcome guarantees, specific clinical claims, and "cure" language. Flag these spots for Dr. Simpson to read through before launch:

- **`services.html#chiropractic`** — Refers to "adjustments," "a treatment plan tailored to what the exam shows," and education. No outcome claims. Confirm the clinician is comfortable with this framing.
- **`services.html#neuropathy`** — This is the highest-risk section. We wrote "addresses the contributing factors we can influence" and avoided any claim that neuropathy is "reversed," "cured," or "healed." We also added an off-ramp: "If we're a fit for your case, we'll walk you through exactly what the program looks like." **Recommend Dr. Simpson personally approve this section** — neuropathy marketing is an area regulators and state boards watch closely.
- **`services.html#weight-loss`** — Says "structured program," "clear plan," "regular check-ins." No specific pounds/week claims, no before/after language, no medication mentions. Confirm whether the clinic prescribes or administers any weight-loss medication (semaglutide, etc.) — if yes, that needs its own dedicated copy and compliance review. Currently the copy treats it as coaching + structured support only.
- **`services.html#wellness`** — Lifestyle-level claims only (sleep, movement, keeping progress). No disease-state language. Low risk.
- **`index.html` "Our approach"** — "find the root cause, explain it plainly, and build a plan the patient can actually follow." "Root cause" can be a loaded phrase in chiropractic marketing; confirm Dr. Simpson is comfortable keeping it. Alternative phrasing: "understand what's contributing, not just what hurts."
- **`index.html` lede** — "Care for the root cause, not just the symptom." Same note as above.
- **Disclaimer blocks** — Both `services.html` and `new-patients.html` end with standard "not a substitute for clinical evaluation / outcomes vary" disclaimers. Confirm with clinic counsel whether these are sufficient or whether additional language is required per Georgia board guidance.

## Content extraction notes

Content drafted on 2026-04-20 from the following sources:
- chiropracticinathens.com (live site)
- Facebook page (`SimpsonChiroCenter`)
- Instagram (`simpsonchirowl`)
- Healthgrades, Vitals, Yelp, Chamber of Commerce, BestProsInTown directory listings
- CareCredit doctor locator

No patient testimonials, outcome stories, or before/after content was carried over from the live site. If the client wants testimonials added, collect fresh patient consent for any quotes used.
