# Itinerary vs Code — Flight Delay Rights Checker

> Paste an itinerary or photograph a boarding pass; get back the refund clock, the care clock, and whether the airline's stated cause matches the code it later reports.

## The document

The thing already on the phone: boarding pass, itinerary email, delay notification text, hotel folio (if one exists). Fields extracted: flight number, date, origin, destination, scheduled time, what the airline said (the stated cause), delay length, whether the passenger accepted rebooking/voucher.

## The public file

1. **14 CFR Part 260** (refund rule) — automatic refund owed on cancellation, or delay ≥3 hours domestic / ≥6 hours international, when the passenger doesn't accept rebooking or voucher. Cause doesn't matter.
2. **DOT Airline Customer Service Dashboard** — each reporting carrier's posted commitments for controllable cancellations/delays (meals, hotels, rebooking). Commitments attach to disruptions the carrier codes as within its control.
3. **14 CFR Part 234, as amended Sept 3, 2026** (91 FR 56588), effective **October 19, 2026** — new reporting category Section 511(b) for ten FAA Reauthorization Act events carriers may no longer place in the Air Carrier (controllable) bucket: death-cleanup, extreme-weather/debris/sabotage damage, uncontrolled baggage-system outage, cyberattack, government-system shutdown, overheated brakes after emergency stop, unscheduled maintenance (incl. airworthiness-directive work), onboard medical emergency, unruly-passenger removal, volcanic ash/wind/wind-shear airport closure.
4. **BTS cause file** — the carrier's reported cause code, published late, by carrier and airport.

## The join

Itinerary (stated cause + delay hours) → Part 260 refund clock (3h/6h thresholds, rebooking refused?) → dashboard commitments for that carrier (does the stated cause look like Air Carrier or one of the ten 511(b) events?) → later, the BTS-posted code vs. what the airline said at the gate. Start: one carrier, one metro, paste only, no accounts. Month 2: add hotel folio. Month 3: internal scoreboard of stated vs. coded cause.

## The verdict

- **Refund clock** — did the delay cross the Part 260 threshold with rebooking refused? (Code-independent.)
- **Care clock** — what the carrier posted on the dashboard, and whether the delay text looks like Air Carrier or a 511(b) event.
- **Mismatch** — the text said crew, the later code said maintenance; or the text said mechanical and the posted code said 511(b).
- **File too thin** — not enough on the itinerary/text to place the clocks (inferred; essay's honest-uncertainty rule).

## Guardrails

- The model drafts; a person files. A refund request can be a draft; a DOT aviation-consumer complaint, a chargeback asserting a broken commitment, or any letter asserting a legal right goes out only with a human signer.
- Never auto-send complaints — otherwise it's "an unlicensed claims shop with a timer" (essay).
- Uncertainty is a feature: label the text as "consistent with a 511(b) event" or not; never swear to unscheduled maintenance without the maintenance log. False certainty hands the airline's lawyer a free exhibit.
- Changing the cause code changes the hotel, not the refund — never collapse the two rights into one slogan.

## Limitations

- The BTS cause file posts late — the mismatch verdict arrives weeks after the trip (stated in essay).
- "Mechanical" is genuinely ambiguous: deferred item the carrier owns vs. unscheduled maintenance the new category holds; the passenger can't see the code (stated in essay).
- Federal law doesn't generally require hotels/meals — care rights rest on the carrier's posted dashboard commitments, which carriers can change (stated in essay).
- The October 19, 2026 rule gives carriers a sharper "not our fault" bucket — the join still works but the carrier's wrong answers get more precise (stated in essay).
- One carrier + one metro to start; the mismatch map (the sellable asset for travel desks, card issuers, plaintiff shops) needs volume (stated in essay).

## Original essay

https://tygartmedia.com/the-best-delay-product-reads-the-itinerary-against-the-code/
