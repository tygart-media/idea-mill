# Nameplate vs Program — Home Energy Rebate Checker

> Photograph an HVAC nameplate or water-heater sticker; get back whether your ZIP still has an open rebate file for that equipment.

## The document

A photo of the outdoor unit's nameplate, the water-heater sticker, or the first page of last month's utility bill — plus the ZIP code. Fields extracted: equipment model number, fuel type, and location. No account for the first answer.

## The public file

State **Home Efficiency Rebates (HOMES) and High-Efficiency Electric Home Rebates (HEEHR/HEAR)** program files under the Inflation Reduction Act's $8.8B — tracked via the Building Performance Association's June 2026 fact sheet: 55 states/territories applied by Jan 2025; only 12 states + DC actually launched as of June 2026. DOE updated program guidance June 1, 2026 (active programs had until Aug 31 to conform); the guidance limited non-electric appliance replacement under HEEHR — several states now electric-to-electric only for reservations on/after Sept 1, 2026. Also matched against ENERGY STAR listings and each state's current eligible-measure list.

Context: the residential 25C energy-efficiency tax credit ended for property placed in service after Dec 31, 2025 — the simple path is closed; the messy rebate path is what's left. Georgia (GEFA) is the proof case: 2,600+ households paid via 150+ contractors (~$1,482/yr savings) — then paused new HEAR applications Aug 14, 2026. "Open last month is not open this week."

## The join

Nameplate (model number + fuel type) + ZIP → the state's current program status (open / reserved / paused / closed) + eligible-measure list → is this equipment, in this ZIP, under a live program, and does the fuel path qualify (electric-to-electric rule)? Month 2: add the second object in the same house (water heater, utility bill page).

## The verdict

- **Open** — the program is live for this equipment/ZIP/fuel path; draft the state packet, human submits.
- **Reserved / paused / closed** — program not currently taking this; still a labeled unit captured.
- **Fuel-switch blocked** — fails the post-Sept-2026 electric-to-electric rule.
- **File too thin** — the state's measure list can't be resolved; say so (inferred).

## Guardrails

- The model reads and drafts; a homeowner or licensed contractor signs and submits. Income verification, AMI bands, measured-vs-modeled paths are a profession — the portal doesn't care about your demo.
- Never auto-submit rebate applications or reservations.
- Never pretend the model is a state energy office.
- Get paid on a cut of funded rebates, a contractor lead with a live reservation, or the B2B scoreboard — never a seat fee to see the first answer.

## Limitations

- State portals change eligible SKU lists without press releases; launch dates slip; pauses happen (Georgia paused HEAR Aug 2026) — the file is a moving target and the checker is only as fresh as its last scrape (stated in essay).
- Nameplates are stamped metal in bad light — OCR misfires on model numbers are the core accuracy risk (stated in essay).
- 43 states were still in launch lag as of June 2026 — most ZIPs will return "not open yet" early on (stated in essay).
- Don't build a national rebate marketplace or contractor CRM in week one; don't mix the application with income attestation automation (stated in essay).
- Don't brand it "AI for electrification" — wrong customers (stated in essay).

## Original essay

https://tygartmedia.com/the-best-rebate-product-reads-the-nameplate-before-you-call-the-contra/
