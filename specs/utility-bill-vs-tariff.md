# Bill vs Tariff — Utility Rate Checker

> Photograph a utility bill; get back whether each line matches the filed tariff schedule in force on the read date.

## The document

The monthly utility statement, photo or PDF. Fields extracted: utility name, rate schedule code, kWh (and demand if commercial), each rider as its own line, basic charge, effective/read dates. No account for the first answer. Start: one utility, one residential schedule.

## The public file

The **filed tariff** — every investor-owned utility in a rate-regulated state files rate schedules with its public utilities commission; munis and co-ops publish rate books. The checker joins the bill to the sheet in force on the read date: service class, basic charge, energy charge, riders, effective dates, docket number.

Context from the essay: CAP/NRDC's August 2026 Rate Hikes Tracker counted ≥275 electric/gas utilities with increases starting 2025+, touching 116.4M electric and 59.7M gas customers — $78.9B electric / $22.5B gas through 2028. EIA Sept 2026: national average residential 17.51¢/kWh (2025), 18.25¢ (2026); July 2026 residential revenue 18.31¢/kWh, up 4.9% YoY; 44 states + DC higher year over year.

## The join

Bill lines (schedule code, basic charge, energy charge, each rider) → the filed tariff sheet effective on the read date → line-by-line comparison: does the basic charge match Schedule A? Did any rider survive past its sunset date? Is the customer on the right class (e.g., after a solar install)? Does the math check? Month 2: add the prior bill as a second document for the same account.

## The verdict

- **Match** — the bill lines sit next to the filed sheet.
- **Mismatch** — a line doesn't match: wrong basic charge, zombie rider past sunset, wrong class, math error, late fee over the filed cap.
- **Tariff file too thin** — the commission's book isn't machine-readable or the schedule can't be located; say so honestly.

## Guardrails

- Never hallucinate docket numbers, riders, or effective dates — cite the tariff sheet, the effective date, and the bill line, or say the join failed.
- Never invent a federal "energy refund request" — point at the commission's real complaint page or say nothing.
- The model drafts the informal complaint and the mismatch paragraph; a named human signs. A commission filing is a claim the utility will treat as one.
- Never act as counsel of record, submit the complaint, accept contingency, or speak at a rate hearing — seats, not features.
- Charge only after the join shows a mismatch.

## Limitations

- Tariff books vary wildly: some commissions publish machine-readable schedules, others publish "scanned theater" — the join fails honestly on the latter (stated in essay).
- Municipal/co-op rate books and retail-choice supply contracts aren't delivery tariffs; a national build drowns in them — start one utility, one schedule (stated in essay).
- Riders have sunset dates and fuel clauses lag posted indexes; timing mismatches need the exact effective-date sheet, not the current one (inferred).
- Don't brand it an "agentic energy copilot" — wrong users, wrong lawyers (stated in essay).
- The sellable map (which utilities keep collecting sunset riders, which class codes drift after meter swaps) needs thousands of labeled bills first (stated in essay).

## Original essay

https://tygartmedia.com/the-best-utility-product-reads-the-bill-against-the-tariff/
