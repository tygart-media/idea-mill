# Notice vs Roll — Property Tax Assessment Checker

> Photograph a property tax notice; get back whether the assessed value sits high, in band, or can't be judged against nearby sales on the public roll.

## The document

The notice of appraised value, the assessment card, or the protest packet. Fields extracted: parcel ID, proposed market value, exemption lines. No account for the first answer. Start: one county.

## The public file

The county's public parcel roll — parcel attributes, last sale, neighborhood sales, exemptions, protest calendar. In most large metros, a comparable-sales extract or open GIS layer. The checker joins the notice to the roll and to sales that closed near the valuation date.

Context from the essay: NBER Working Paper 35632 (Aug 2026, "Taxpayer Behavior in the Age of AI") — a Dallas County field experiment (45,200 postcards, 645 households) found that giving owners an evidence pack plus a chatbot lifted direct-appeal filing from 41.4% to 50.5% (+9.1 points). Forbes (June 2026, Cook County): commercial appeal rates 64% vs. homeowner 27%; some lawyered pockets hit 92%, poorer neighborhoods sank near 5%. Park City agent Wayne Levinson used AI parcel screening to secure $13.9M in 2025 assessed-value cuts — with a human filing and sitting the hearing.

## The join

Notice (parcel ID + proposed value) → county roll (parcel attributes, comps, exemptions) → is the number high relative to recent sales of like parcels, wrong on square footage/condition, or fine? Month 2: add the prior-year notice for the same parcel.

## The verdict

- **High** — assessed value above what nearby sales support; draft the protest the owner signs.
- **In band** — the number sits with the comps; still a labeled pair captured.
- **Roll too thin** — the county's public file can't support a join; say so honestly.

## Guardrails

- Never hallucinate case law or precedent — cite the roll and the sale, never a dreamed case (essay cites a BC appeal board that had to write an AI-disclosure rule after fake citations).
- Never invent a federal program — point at the county's real protest page (essay: Douglas County, CO warned residents about a viral video inventing a federal "Senior Homeowner Tax Review Request" — no such form exists).
- The model drafts the protest; a named human signs and files. Never submit the protest, accept contingency, or speak at the appraisal review board — those are seats, not features.
- Charge only after the join shows a mismatch.

## Limitations

- County file formats vary wildly; homestead rules and freeze provisions differ by state — one county to start, no national platform in month one (stated in essay).
- The NBER lift was smaller among less-educated owners, lower-valued homes, and minority households — a chat-only product recreates the lawyer gap in cheaper clothes (stated in essay).
- Appeals shift the tax base — commercial appeals already shift 3–4% onto houses yearly in Cook County; the product should be honest that winning has system effects (stated in essay).
- Mass-appraisal models overshoot after sale years; condition codes drift — the join needs the valuation-date sales, not today's (inferred).

## Original essay

https://tygartmedia.com/the-best-tax-product-reads-the-notice-against-the-roll/
