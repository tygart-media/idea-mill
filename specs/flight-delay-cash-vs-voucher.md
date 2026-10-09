# Voucher vs Cash — Airline Refund Checker

> Paste a confirmation email or delay text; get back whether the delay already triggered a cash refund under federal rules — before you tap the voucher.

## The document

The confirmation email, the delay SMS, or a photo of the gate screen. Fields extracted: PNR, flight number, date, origin/destination, scheduled vs. actual times, what the airline offered (voucher/credit vs. cash). No account for the first answer. Month 2: add the second document — bag-fee receipt, seat-fee receipt, hotel booked because the inbound died.

## The public file

1. **14 CFR Part 260** (DOT Refunds and Other Consumer Protections final rule, April 2024) — full refund of fare + taxes + ancillary fees owed on cancellation or significant delay/change when the passenger doesn't take the new itinerary and doesn't accept a voucher/credit/substitute. Refund supposed to be automatic: 7 business days (credit card), 20 calendar days (other methods). Carriers must disclose the cash option before pitching miles.
2. **July 8, 2026 DOT enforcement-discretion notice** (extending Dec 5, 2025 pause) — a mere flight-number change is NOT a cancellation if the passenger is rebooked with no significant change/delay. Still counts: 3+ hours domestic departure/arrival delay, different airport, class downgrade.
3. **BTS TranStats** (marketing-carrier view, Jan–Jun 2026): 85,998 cancellations (2.23% of 3.86M flights) vs. 59,609 (1.56%) same window 2025; 823,345 arrival delays (21.35%); on-time 76.14%.
4. **DOT Air Travel Consumer Report** (April 2026): 7,278 complaints; refunds #1 at 2,296. ACERS (Aviation Complaint, Enforcement, and Reporting System) opened Aug 1, 2025. OIG 2025 audit: >139,000 refund complaints 2020–2022 vs. 1,568 in all of 2019; >$155M in civil penalties across 14 airlines.

## The join

Itinerary (delay hours, cancellation status, what was offered/accepted) → Part 260 thresholds (3h domestic / 6h international, rebooking refused, voucher refused) → is cash owed? Ancillary layer: bag fees for bags that never rode, seat fees on cancelled segments, Wi-Fi not provided — Part 260 names these; almost nobody files because the receipt is three emails deep.

## The verdict

- **Cash owed** — the delay/cancellation crossed the Part 260 line with no accepted substitute; draft the carrier request or ACERS filing, human sends.
- **Voucher trap** — cash was owed but the passenger already tapped the voucher/credit; flag what was lost.
- **Not significant** — under the thresholds (including the July 2026 renumbering carve-out); still a labeled itinerary captured.

## Guardrails

- The model drafts the carrier request or ACERS filing; a human owns the send. ACERS and carrier portals are irreversible enough.
- Never pretend the model is a DOT lawyer — Part 260 has definitions; "significant change" is not a vibe; the July 2026 discretion carve-out is real and must be applied correctly.
- Get paid when the cash posts, or a cut of recovered ancillaries — never a seat fee to see the first answer.

## Limitations

- The July 8, 2026 enforcement-discretion notice narrows what counts as a cancellation — renumbered-but-on-time flights are carved out; misapplying this trains customers to ignore the product (stated in essay).
- Codeshare legs can drop the refund obligation onto a foreign operator the passenger never contracted with — jurisdictional edge cases (stated in essay).
- Airline PDFs, codeshare itineraries, and split-board screenshots are messy inputs; the model does the first pass, not the final legal call (stated in essay).
- Don't build a trip organizer or "consumer-protection copilot" — the wedge is the single verdict at the gate, not a travel profile (stated in essay).
- The B2B scoreboard (which carriers convert 3-hour delays into credits, which ancillary SKUs never auto-refund) needs thousands of labeled itineraries first (stated in essay).

## Original essay

https://tygartmedia.com/the-best-delay-product-tells-you-cash-is-owed-before-you-take-the-vouc/
