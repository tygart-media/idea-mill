# The Idea Mill — Build Specs

Every spec in this repo is the same machine, pointed at a different industry:

**A document the customer already holds, joined against a file the government was required to publish, with a verdict on the other side.**

That's it. That's the whole system. Twelve times, twelve industries.

## How to use this

Each file in `/specs` is a standalone build spec. Paste one into your AI — any of them — and ask it to scaffold the prototype. The spec gives it the concept, the document, the public file, the join logic, the verdict shape, the guardrails, and the honest limitations. Everything we think about the idea is in the file. There is no hidden second document.

## The pattern

```
DOCUMENT (customer holds)  +  FILE (agency published)  →  VERDICT
```

The verdict is always one of three words:

- **Match** — the numbers sit next to each other. Nothing to do.
- **Mismatch** — the gap is real and the file proves it. This is where the product earns its keep.
- **File too thin** — the public file doesn't cover this case, or the document doesn't have enough to say. Saying so is the product working, not failing.

## The rules every spec follows

1. **No account for the first answer.** The first verdict is free and takes seconds. If you can't get a stranger to try it once, you don't have a company.
2. **The model drafts; a person owns the send.** Anything that leaves the building — a letter, an inquiry, a complaint — needs a human signer who has seen the document, the file row, and the exact sentence being sent.
3. **Charge on the proven gap, or don't charge.** Contingency after a confirmed mismatch is fine. Subscriptions to dashboards are not the business here.
4. **Say what it can't do.** Every spec lists its limitations honestly. A product that can't say "file too thin" will eventually say something wrong with confidence.

## The specs

| # | Spec | Document | Public file |
|---|------|----------|-------------|
| 01 | [Pharmacy receipt vs acquisition cost](specs/pharmacy-receipt-vs-nadac.md) | Pharmacy receipt / bag label | NADAC weekly file + Medicare maximum fair price |
| 02 | [401(k) fee vs filing](specs/401k-fee-vs-filing.md) | 401(k) statement | Plan filing |
| 03 | [HOA assessment vs reserve study](specs/hoa-assessment-vs-study.md) | HOA assessment notice | Reserve study |
| 04 | [Flight delay: itinerary vs cause code](specs/flight-delay-itinerary-vs-code.md) | Itinerary / boarding pass | Delay cause codes |
| 05 | [Housing: unit vs score](specs/housing-unit-vs-score.md) | Listing / unit details | Housing score |
| 06 | [Utility bill vs filed tariff](specs/utility-bill-vs-tariff.md) | Utility statement | Filed tariff |
| 07 | [Tax notice vs assessment roll](specs/tax-notice-vs-roll.md) | Tax notice | Assessment roll |
| 08 | [Medical EOB vs hospital chargemaster](specs/medical-bill-eob-vs-chargemaster.md) | Explanation of benefits | Hospital price file |
| 09 | [Rebate: nameplate check](specs/rebate-nameplate.md) | Product nameplate | Rebate file |
| 10 | [Recall: label check](specs/recall-label.md) | Product label | Recall list |
| 11 | [Flight delay: cash vs voucher](specs/flight-delay-cash-vs-voucher.md) | Itinerary | Compensation rules |
| 12 | [Contractor short-pay flag](specs/short-pay-contractor-packet.md) | Job packet / invoice | Contract / scope file |

## Go make it

These are open. Take one, build it, keep the map it produces — the labeled pairs of *what was charged vs what was filed* are the moat, not the checker. If you build something real from a spec, we'd love to hear about it.

— Tygart Media
