# The System

## The machine

Every product in this repo is an instance of one machine with four stages:

```
1. INTAKE      Document the customer already holds (photo, PDF, screenshot)
2. JOIN        Match it against the public file on the shared fields
3. VERDICT     Match / Mismatch / File too thin
4. GATE        Human signs anything that leaves the building
```

Nothing in the machine gives advice. It compares two records and reports the
difference. That constraint is load-bearing: it keeps every instance out of
regulated-advice territory (medical, legal, financial) and inside
document-comparison territory, which is unregulated math.

## Why now

Two things changed at once:

1. **The files got public.** Agencies were required to publish machine-readable
   price, tariff, roll, and schedule files. Most of them are boring CSVs on
   .gov domains. They were always public; they only recently became *usable*
   without a data team.

2. **The reader got cheap.** A phone photo of a receipt, bill, or label can now
   be converted to structured fields in seconds by any frontier vision model.
   The intake primitive — the thing that used to require a scanner, an app,
   and a signup — is now a camera and a prompt.

The wedge is the join happening *before* money moves: before the card is
charged, before the voucher is accepted, before the job closes. After is
customer service. Before is a product.

## The economics

- **Free checker, paid gap.** The first verdict is free. Revenue comes from the
  confirmed mismatch: contingency on the recovered amount, or a flat fee for
  the inquiry pack. Never a subscription to a dashboard.
- **The map is the moat.** The first hundred documents are a demo. The ten
  thousandth is a labeled dataset of charged-vs-filed pairs by vendor, chain,
  and ZIP. Nobody else keeps the pair. That dataset — not the checker — is the
  durable asset. A plan sponsor, a regulator, or a reporter will pay for the
  pair once it is boring and repeatable.
- **Start narrow.** One document type, one public file, one geography, no
  account. Expand only after strangers use the checker unprompted.

## What the machine refuses

- It does not tell anyone to stop a medication, split a tablet, or change a
  clinical decision.
- It does not file appeals, complaints, or legal claims.
- It does not move money.
- It does not sell subscriptions to dashboards of things the user could look
  up themselves.
- A mismatch can be a plan design, a spread, a coupon that already fired, or
  a bad read of the document. The machine reports the gap; a person decides
  what it means.

## Building from a spec

Each spec in `/specs` is self-contained. The fastest path:

1. Paste the spec into your AI of choice.
2. Ask for a prototype: intake UI, file ingestion, join logic, verdict screen.
3. Test it against five real documents before writing any more code.
4. If strangers won't photograph one document, stop. You have an essay, not
   a company.
