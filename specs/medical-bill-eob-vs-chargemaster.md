# EOB vs Hospital File — Medical Bill Checker

> Photograph a hospital bill or EOB; get back whether the billed line matches the price the facility was required to post.

## The document

An Explanation of Benefits (insurer portal PDF) or an itemized hospital statement (photo of the last page). Fields extracted: CPT/HCPCS codes, dollar amounts per line, facility name. No account for the first answer.

## The public file

The hospital's **machine-readable standard-charges file** required under 45 CFR 180 — CMS treats it as a compliance object. Enforcement context from the essay: 10 civil monetary penalties in 2025 (vs. 3 in 2024), 28 hospitals fined by Feb 2026 ($32,301–$309,738); 519 hospitals got warning/corrective-action notices since April 2026; CMS publishes enforcement outcomes as a public dataset. But compliance ≠ usable: PatientRightsAdvocate.org's 8th scorecard (Sept 2026) put full-rule compliance at 49.4% of 2,000 hospitals, and only 18% posted real dollar prices for at least half of items. "Missing, not comparable" is a labeled outcome.

Related flags the checker marks (not files): out-of-network clinician at an in-network facility, ER professional-fee balance billing, balances the No Surprises Act should have removed.

## The join

Statement line (CPT/HCPCS + dollars + facility) → that facility's posted standard-charges file → is the billed number the listed number, a negotiated rate, a cash price, or a number with no cousin in the file? Month 2: add the insurer EOB as a second document for the same facility.

## The verdict

- **Match** — the billed line sits next to the posted price.
- **Mismatch** — the billed line doesn't match; draft the question the patient or office manager sends next.
- **File too thin** — the facility's file is theater (posted but not joinable); that's a labeled outcome, not a failure.

## Guardrails

- Never submit a CMS complaint, state insurance complaint, or payment from the patient's card. Never call itself a patient advocate.
- The model drafts (itemized-bill request, charity-care packet, No Surprises Help Desk narrative); a person owns the send. Billing disputes move money and create claim records.
- No Surprises flags are informational — the checker marks the pattern; it doesn't file the federal complaint.
- The CFPB's Jan 2025 medical-debt credit-reporting rule was vacated July 11, 2025 — don't build on credit-report relief (essay).
- Charge only after the file proves a mismatch.

## Limitations

- Only 18% of hospitals post real dollar prices for half their items — most joins will hit "file too thin" until compliance improves (stated in essay).
- Hospital files use inconsistent schemas; CPT families drift from cash-price columns; insurer EOBs systematically omit codes the hospital file uses (stated in essay).
- The No Surprises IDR machine (1.37M disputes in H2 2025, providers winning ~85%) is a provider–payer fight, not a patient tool — the checker stays on the patient-facing flag (stated in essay).
- KFF (Apr 2026): ~half of US adults couldn't cover a $500 surprise bill without borrowing — the audience is real but financially fragile; contingency pricing needs care (inferred).
- Don't build a full revenue-cycle platform (eligibility, prior auth, clearinghouses) in month one (stated in essay).

## Original essay

https://tygartmedia.com/the-best-bill-product-reads-the-eob-against-the-hospital-file/
