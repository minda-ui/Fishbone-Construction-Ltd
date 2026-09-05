---
title: Standard KB skeleton adopted
category: Decisions
status: active
sensitive: false
created: 2026-09-05
updated: 2026-09-05
sources:
  - ../../Outputs/change-log-2026-09-05-kb-skeleton-and-raw-tidy.md
related:
  - ../index.md
---

# Standard KB skeleton adopted

On 2026-09-05 this knowledge base was brought up to the structure already in use by
`Fishbone Properties Ltd - Knowledge Base` and `Fishbone Commercial Properties Ltd - Knowledge
Base`. Until then it had only `Raw/` and a flat `Wiki/` of five Google Docs: no standing context
file, no `Archive/`, and an entirely empty `Outputs/`.

## Key facts

| Item | Value | Source |
|---|---|---|
| Model followed | `Fishbone Commercial Properties Ltd - Knowledge Base`, `CLAUDE.md` v2 | [^1] |
| Files created | `CLAUDE.md`, `README.md`, `Archive/`, `Outputs/kb-registers.md`, `Wiki/index.md`, `Wiki/_templates/article.md`, `Wiki/Decisions/` | [^2] |
| Change logging | Moved from one Google Doc to `Outputs/change-log-YYYY-MM-DD-<slug>.md` | [^2] |
| Raw files reorganised | 99 project documents grouped into 8 supplier folders | [^2] |

## What was copied unchanged

The rules with a recorded failure behind them, because re-deriving them would mean repeating the
failure:

- **Archive-then-recreate** for every standing file, with a suffix naming a *specific* reason.
  Drive has no in-place edit, so a replacement is a new file plus a renamed old one.
- **Dated change-log entries are written once and never edited.** A correction is a new entry
  that references the old one, so a reader can see what was believed at the time.
- **The outbound-reference check.** After replacing a file, open everything it points at and
  confirm the target still says what is claimed. A sister KB left three references pointing at
  sections that had been archived, and nothing was watching.
- **A number inherited from an earlier session is not evidence.** Count it, or do not state it.
- **Retract in place.** A claim that turns out to be wrong is struck through and corrected, not
  deleted.

## What was changed for this company

The sister KBs hold a property and a tenant each. This one trades. The differences that follow:

- **Categories.** `Projects`, `Customers` and `Suppliers` replace `Properties` and `Tenants`.
- **Section 0 states the KB's purpose**, which the sister files do not need to. The owner's
  instruction was that this KB collects real-time data, processes it, documents it and passes
  the result to the Fishbone Group KB. It is a pipeline node, and work here should be written to
  be handed upward.
- **Section 0 also carries a standing warning to check the sister KBs before concluding anything
  about a counterparty name.** On 2026-09-04 an entire analysis rested on "Fishbone Drylining"
  credits being income from a related company. They were this company drawing on its own
  facility under its former name, and the group Loans wiki had recorded that on 21 August. The
  Loans folder had not been searched.
- **Section 3c** covers the invoice-to-Classifier-and-Budget procedure, which has no analogue in
  the sister KBs.
- **Section 3d** carries reading limits specific to this company's documents, including that
  Screwfix order-history PDFs have no text layer at all.
- **Section 5** proposes routines aimed at what actually broke here: a bank statement processor,
  and a data-capture watchdog, because Dext has been failing since 24 August and the QuickBooks
  bank feed has been stale since at least 2 September, and in both cases nobody was alerted.

## What was deliberately left alone

- **The five legacy Google Docs at the root of `Wiki/`.** They are live and correct. Converting
  them to Markdown and moving them into category folders changes the URLs the owner uses and the
  reference block inside the Goathland instructions. Listed in `index.md` under "Unfiled" with
  the question put to the owner rather than answered.
- **The old `Change Log` Google Doc.** Closed and banner-marked, not deleted. It is still the
  record of 25 August to 5 September 2026.
- **The 99 Raw filenames.** The Dext transaction id is the link back to Dext and to the Budget
  and Classifier notes written on 2026-08-25. Grouping them into supplier folders and writing an
  `INDEX.md` gives the legibility without breaking that link.

## Open questions

- Should the five Google Docs be converted to Markdown and foldered?
- No access review has been run on this KB. Both sister KBs ran one and both found something.
- The wiki holds almost no substance yet. Everything discovered about the company's trading
  position lives in change-log entries, which are never revised - the wrong home for facts that
  change.
  **Closed 2026-09-05 later the same day:** twelve articles were built across five new
  categories. See `Outputs/change-log-2026-09-05-wiki-from-bank-data.md`.

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-05 | Created | `Outputs/change-log-2026-09-05-kb-skeleton-and-raw-tidy.md` |

## Sources

[^1]: `Fishbone Commercial Properties Ltd - Knowledge Base/CLAUDE.md`, version 2 of 2026-09-03, corrected 2026-09-04 and 2026-09-05.
[^2]: [Change-log entry](../../Outputs/change-log-2026-09-05-kb-skeleton-and-raw-tidy.md), 2026-09-05.
