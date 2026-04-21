# The National — Asset Requirements & Open Questions

The site is intentionally photography-light. The editorial treatment is carried by typography and hairline rules, not plated-food hero shots. Still, a small set of real assets and a few confirmations from the client would tighten everything up before launch.

## Content sources

Menu content, prices, and descriptions were pulled from **allmenus.com** on 2026-04-20 (the published printed menu). Restaurant background, ownership, and hours were confirmed via search against the live site at `http://www.thenationalrestaurant.com` (HTTP-only; `WebFetch` blocked by cert policy during the build), the Visit Athens listing, Yelp, and OpenTable.

## Content to confirm with client

- **Exact founding year.** We used **2007** per Peter Dale / Hugh Acheson interviews and Visit Athens copy. Confirm.
- **Current chef billing.** We credited **Chef Burns Sullivan** on the homepage essay; Peter Dale is credited as founder/owner and Erin Wilson as GM/partner on the private dining page. Confirm all three are currently active and correctly titled.
- **Menu accuracy.** Every dish name and description on `menu.html` is taken verbatim from the most recent printed menu we could find. Prices were included where listed. **All cellar prices and any seasonal-menu changes are flagged `$ —`** and must be filled in by the client.
- **Wine list.** The six by-the-glass pours on `index.html` and `menu.html#cellar` are representative of the restaurant's Mediterranean / Iberian lean but are **not verified from a current list**. Replace with the actual current BTG list and full cellar PDF if desired.
- **Hours.** We used: Mon–Tue dinner 5–9; Wed–Sat lunch 11–2 and dinner 5–9; Sunday closed. Confirm against current POS.
- **Email address.** `reservations@thenationalrestaurant.com` is a reasonable guess based on the domain; confirm the correct inbox (or provide `info@`, `events@`, etc.).
- **Private dining capacity.** We wrote "a dozen to several dozen" and "full-restaurant buyouts" without a specific count. Provide: private room max seated, full buyout capacity, and F&B minimums by night.
- **Lunch days.** Live-site copy says lunch runs Wed–Sat; search results include Thursday. We went with the Wed–Sat version. Confirm.
- **Pull quotes on `index.html` and `private-dining.html`.** Both are house-voice lines written for this redesign. If the client would prefer a press pull (Garden & Gun, Eater, Southern Living, etc.) in their place, swap in.
- **"Issue No. 01 · Spring"** in the top-left of the nav is an editorial flourish and can be rotated seasonally or removed.

## Photography (optional but nice to have)

This design deliberately avoids plated-food cards. The two places a real image would add something:

- **`assets/dining-room.jpg`** — Wide, low-light shot of the dining room at service. Could sit at the top of `private-dining.html` or anchor a future About page. **Target:** 1600×1000px, landscape, warm tones.
- **`assets/exterior.jpg`** — The West Hancock storefront at dusk. Could replace the map placeholder on `visit.html` or run above the masthead. **Target:** 1600×1000px.
- **`assets/logo.svg`** — If The National has an actual wordmark or logo, swap into the masthead on `index.html` in place of the current Syne-set type treatment.
- **`assets/favicon.svg`** / **`assets/favicon.ico`** — The inherited favicons ship with the folder; confirm they are current.

## Maps

`visit.html` has a styled placeholder in place of an embedded map. Replace with a Google Maps iframe embed for **232 W Hancock Ave, Athens, GA 30601**.

## Forms

The private dining inquiry form on `private-dining.html#inquire` currently fires `alert()` on submit and resets. Wire to deliver to **reservations@thenationalrestaurant.com** (or the confirmed inbox) with subject prefix `[Private Dining Inquiry]` via Cloudflare Pages Functions + Resend/Postmark, Formspree, or a direct SMTP relay.

## External integrations

- **OpenTable** reservations: `https://www.opentable.com/r/the-national-athens` — confirm this is the canonical URL (live site may use a different reservations vendor).
- **Facebook**: `https://www.facebook.com/thenationalathens/` — confirm active.
- **Instagram** is not currently linked; add if the client wants it in the footer.

## Copy to double-check

Content was extracted / written on 2026-04-20. Before going live:
- Confirm address: **232 W Hancock Ave, Athens, GA 30601**
- Confirm phone: **(706) 549-3450**
- Confirm every menu item and price on `menu.html`
- Confirm the essay copy on `index.html` reads true to the kitchen's voice — it is written in a restrained, first-person-plural style meant to feel like a weekly kitchen dispatch and can be rotated as often as the client wants. Consider a short CMS or a simple file-swap for the weekly update.
