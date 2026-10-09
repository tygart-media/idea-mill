# Receipt vs File — Pharmacy Price Checker

> Photograph a pharmacy receipt; get back whether what you paid sits next to the public acquisition file and the Medicare negotiated price.

## The document

A pharmacy register receipt, the sticker on the bag, or a Part D explanation of benefits. Fields extracted: NDC (if printed), drug name and strength (if NDC is not printed), quantity, amount paid, fill date, pharmacy name, and payment type (cash, coupon, or plan).

## The public file

Two files, both from the Centers for Medicare and Medicaid Services (CMS):

1. **NADAC** (National Average Drug Acquisition Cost) — a survey of what retail pharmacies pay wholesalers, net of prompt-pay discounts. Published weekly on data.medicaid.gov. Matched by NDC for the week of the fill.
2. **Maximum fair price file** — the negotiated prices for the first 10 Part D drugs, published August 15, 2024, effective January 1, 2026. Relevant only when the drug is one of the first ten and the payer is Part D. Matched by NDC and supply.

Context from the essay: the FTC's January 14, 2025 interim staff report found the Big Three PBMs (Caremark, Express Scripts, OptumRx) marked up specialty generics by hundreds to thousands of percent — $7.3B in excess of NADAC-estimated acquisition cost, 2017–2022. CMS estimated the negotiated prices would have cut 2023 spending on those drugs by ~$6B (22%).

## The join

Receipt line (NDC or drug name + strength + quantity) → NADAC row for that NDC in the fill week → compare amount paid vs. acquisition cost, showing the gap in dollars. If Part D and one of the first ten drugs → also compare against the maximum fair price for that NDC/supply. Start narrow per the essay: cash generics with a stable NADAC row, one state, no account.

## The verdict

- **Match** — the paid amount sits next to the file.
- **Mismatch** — the paid amount is above the file by a stated dollar gap.
- **File too thin** — a real answer: NADAC doesn't cover every branded specialty; a maximum fair price is not a cash price for someone outside Part D. Saying so is the product working.

## Guardrails

- No clinical advice: never tell anyone to stop a drug, split a tablet, or switch pharmacies on a clinical claim.
- Never file an appeal. Never move money.
- The model drafts the comparison; a person owns the send. Anything outbound (note to pharmacy, Part D inquiry, state board complaint) requires a human signer who has seen the receipt, the file row, and the exact sentence to be sent.
- Contingency fees only after that signature and only after a confirmed mismatch. No subscription dashboards.

## Limitations

- Receipt OCR across non-standard pharmacy formats is the hard engineering problem (inferred).
- NDC often isn't printed; drug name + strength → NDC resolution via the FDA NDC directory can misfire, and a bad NDC read produces a false mismatch (essay notes a mismatch can be "a bad read of the NDC").
- A mismatch can also be plan design, spread pricing, or a coupon that already fired — not necessarily overcharging (stated in essay).
- NADAC is acquisition cost, not a fair retail price — pharmacies have rent, pharmacists, dispensing fees; markup over NADAC is not automatically a rip-off (stated in essay).
- Essay advises: don't start with oncology markups and PBM letters — high-stakes first customers become legal exhibits (stated in essay).

## Original essay

https://tygartmedia.com/the-best-pharmacy-product-reads-the-receipt-against-the-file/
