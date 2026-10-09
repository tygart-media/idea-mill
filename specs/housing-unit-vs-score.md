# Unit vs Score — HUD Housing Inspection Checker

> Photograph a defect in your unit; get back whether it's an item HUD now scores, joined to the property's last published inspection score.

## The document

A phone photo of the inspectable item plus the address on the lease or the property name on the building. Item types: outlet (especially near water), fire-labeled door, guardrail, HVAC/thermostat, interior lighting. No account for the first answer. One metro, public housing and multifamily only, to start.

## The public file

1. **HUD USER physical inspection scores** — downloadable comma-delimited files for public housing and multifamily assisted properties, posted through April 8, 2026. Property-level scores with identifiers.
2. **NSPIRE standards + Notice PIH 2025-27 / H 2025-06** (issued Sept 30, 2025) — the scoring clock: six affirmative requirements start taking points **October 1, 2026**: fire-labeled doors; unprotected outlet within six feet of a water source; guardrails; HVAC; interior lighting; minimum electrical and lighting. (HUD delayed once already, to Oct 1, 2025; the extra year is over.)
3. Reference: HUD OIG evaluation 2026-OE-0802 (July 24, 2026) — of 469 public housing properties scoring ≤70 (Mar 2025–Feb 2026), 79.5% scored below 60; 20,360 life-threatening/severe deficiencies across 5,491 buildings and 8,658 units. NAHRO analysis: scores rose ~13 points (public housing) / ~6 (multifamily) after the UPCS switch, partly on unscored affirmative requirements — "the cushion ends" Oct 1.

## The join

Photo (defect family classification) + address → HUD USER file lookup (is this an assisted property? last published score?) → does the defect belong to a family that takes points under the Oct 1, 2026 notice? Output the three-line verdict with citations: HUD USER file date, notice citation, defect family.

## The verdict

- **Scored item** — the photo shows a defect family the notice scores.
- **Not scored** — the item isn't in a scored family.
- **Property not in the HUD file** — not assisted housing; say so and stop.
- **Photo too thin to judge** — honest failure mode.

## Guardrails

- Never hallucinate inspection IDs, scores, or defect citations — cite the HUD USER file date, the notice, and the defect family, or say the join failed.
- Never invent a federal "housing refund request" — point at the real PHA complaint process or HUD hotline, or say nothing.
- The model drafts work orders/complaints; a named human signs. A formal complaint, tenancy-termination request, or uninhabitability claim creates a court-treatable record.
- Never act as counsel of record; never file the complaint, accept contingency, or speak at hearings — those are seats, not features.
- Charge only after the join shows a scored defect the file didn't absorb.

## Limitations

- HCV units run on a later NSPIRE clock; city code isn't NSPIRE; market-rate buildings have no HUD file — the checker must fail honestly on all three (stated in essay).
- Photo classification of defects (e.g., "unprotected outlet within six feet of water") is the hard vision problem; blurry photos must return "too thin," not a guess (inferred from essay's honesty rule).
- HUD USER files lag reality — a cited score may predate recent repairs or new deficiencies (inferred).
- Scores are expected to decline once habitability items are scored (OIG), so early verdicts sit on a moving baseline (stated in essay).
- Don't brand it an "agentic housing copilot" — attracts the wrong users and the wrong lawyers (stated in essay).

## Original essay

https://tygartmedia.com/the-best-housing-product-reads-the-unit-against-the-score/
