# Label vs File — Product Recall Checker

> Photograph a product label, lot code, or VIN plate; get back whether that exact object is in a live recall file.

## The document

A photo of the back of the package (UPC + lot code), the VIN plate, or the receipt still showing the UPC. One identifier to start — grocery (UPC + lot) or VIN, not both. No account for the first answer. Pick one door first: grocery is the fastest photo, VIN the cleanest identifier, toys/infant gear the highest-fear door.

## The public file

The agency recall feeds, mirrored nightly (RecallBench does this publicly as of Sept 16, 2026):

1. **CPSC** — 305 recalls (2024), 420 (2025), 434 YTD by mid-Sept 2026.
2. **FDA + USDA-FSIS food events** — 516 (2024) → 642 (2025), +24%.
3. **NHTSA campaigns** — 996 (2025), 645 through mid-Sept 2026; e.g., the Feb 20, 2026 Ford/Lincoln tail-light file named 4,381,878 vehicles.

Match keys: UPC/lot/establishment number (food/consumer products), VIN prefix (vehicles).

## The join

Photo (GTIN/UPC + lot line, or VIN) → nightly-mirrored agency feeds → exact match on lot/UPC/VIN range? If match: show the agency page, date, class (when the agency uses one), and draft the next step (return, repair, claim) — the customer sends it.

## The verdict

- **Match** — the object is in a live file; show agency page + class + drafted next step.
- **No match** — not in the file; still a labeled object captured.
- **Need a clearer lot line** — the photo can't resolve the identifier; honest failure, not a guess.

## Guardrails

- Never build a medical diagnostic — a lot-code match is not a diagnosis; on foodborne illness, point at the agency notice and a clinician.
- Never auto-file claims, attorney retainers, dealer work orders, or customs/medical filings. Models draft; people own the send.
- Never build a class-action mill that auto-files.
- Don't mix food, toys, and vehicles in the first 90 days of go-to-market — one door.

## Limitations

- Lot codes are tiny, UPCs sit under glare, VINs live on dirty plates — the vision read is the accuracy bottleneck; "need a clearer lot line" must be a first-class answer (stated in essay).
- Event counts are rising (CPSC +38% 2024→2025) — the feed volume grows, but household matching behavior doesn't; the product fights apathy, not data scarcity (inferred).
- A match is not a diagnosis or a legal claim — food-safety matches especially need the agency-notice-plus-clinician framing (stated in essay).
- The B2B scoreboard (which SKUs/plants/VIN prefixes repeat) needs thousands of labeled matches before it's sellable (stated in essay).
- Don't brand it "AI for pantry safety" — wrong customers (stated in essay).

## Original essay

https://tygartmedia.com/the-best-recall-product-reads-the-label-before-you-throw-the-box-away/
