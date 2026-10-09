# Fee vs Filing — 401(k) Plan Fee Checker

> Photograph a 401(k) fee disclosure; get back whether the plan's fees sit inside or above the peer band for its size, cut from public filings.

## The document

The annual 404a-5 fee disclosure notice, the recordkeeper invoice, or the administrative-expense line on the sponsor's copy of Form 5500. Fields extracted: plan name, participant count (if printed), dollar fee or basis points (if printed). No login for the first answer.

## The public file

**Form 5500, Schedule H, administrative expenses** — filed by plan administrators, published by the Department of Labor from EFAST2; the 2009-and-later datasets update around the first of each month. Joined to the size band from the September 2026 Admin316 cut (Russell McNorton): every 2024 plan-year Form 5500 with Schedule H, pension feature code 2K, ≥25 active participants, positive admin expenses and positive year-end assets — 48,944 plans.

Published bands (per-participant $ / basis points, median and 90th percentile):
- 25–99 participants: median $364 / 32.5 bps, 90th $977
- 100–249: median $228 / 31.8 bps, 90th $548
- 250–500: median $166 / 28.7 bps, 90th $382
- 500+: median $104 / 18.6 bps, 90th $250
- National median: $162 / 27.0 bps. 30.6% of plans under 500 participants paid more than twice the national median (>$324/person).

The 404a-5 disclosure regime itself: required under 29 CFR 2550.404a-5 (DOL), collected under OMB 1210-0090.

## The join

Disclosure page (dollar fee + headcount, or assets) → peer band for that participant-count bracket → dollars-per-participant vs. band median and 90th percentile; basis points vs. 27.0 national median. Month 2 extension: join the sponsor's page to the public Form 5500 row by EIN/plan number — filed admin expense next to the invoice. Month 3: add the 404a-5 investment-expense table as a second label (captures revenue sharing invisible on the invoice).

## The verdict

- **Inside the band** — the fee line sits within the peer band for that participant count.
- **Above the band** — the fee line sits above the band; show $/participant vs. median and 90th percentile.
- **Page too thin** — the page lacks the fee or headcount needed to place it.

## Guardrails

- Never accuse a fiduciary of a breach — excessive-fee pleading is a lawyer's work; the checker's work is the label. (Essay: paying $977/participant isn't itself a breach; paying it without a comparison is harder to defend.)
- Never file with the Department of Labor / EBSA as a first action. Never move plan assets.
- Models draft; the sponsor signs. Irreversible steps stay human. A draft question to the recordkeeper or committee note is fine after a human signer; a demand letter is not the model's job.
- Charge only after the page proves a mismatch.

## Limitations

- The bands are from 2024 plan-year filings (September 2026 cut) — they age as new filings publish (stated in essay; build order says to label which band set is in use).
- Peer-band comparison is not a fiduciary-breach determination; high fees can be legitimate (stated in essay).
- Recordkeeper invoices and filed admin expenses can legitimately differ in what's included (inferred — the essay's month-2 join shows both numbers rather than declaring one wrong).
- Revenue-sharing arrangements never appear on the invoice, so invoice-only checks understate total cost — the essay's month-3 extension addresses this, but early versions miss it (stated in essay).
- Plan documents are a swamp; the checker deliberately reads only the admin-expense line, so document-level nuance is out of scope by design (stated in essay).

## Original essay

https://tygartmedia.com/the-best-401k-product-reads-the-fee-against-the-filing/
