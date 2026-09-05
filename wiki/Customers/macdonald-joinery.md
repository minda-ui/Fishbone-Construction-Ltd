---
title: Macdonald Joinery
category: Customers
status: active
sensitive: true
created: 2026-09-05
updated: 2026-09-05
sources:
  - ../../Raw/2026-09-05_owner-note_macdonald-joinery-has-no-projects.md
  - ../../Raw/Finance/20260321_04212819.csv
  - ../../Raw/Finance/20260421_04212819.csv
  - ../../Raw/Finance/20260521_04212819.csv
  - ../../Raw/Finance/20260621_04212819.csv
  - ../../Raw/Finance/20260721_04212819.csv
  - ../../Raw/Finance/20260821_04212819.csv
related:
  - ../Finance/trading-receipts.md
  - ../Finance/related-party-funding.md
  - ../Suppliers/subcontractors.md
---

# Macdonald Joinery

The company's only substantial third-party customer, and the source of 80% of all customer
receipts in the six months to 21 August 2026. Its payments fell 86% in a single month in May
2026. **The owner confirmed on 2026-09-05 that the reason is that Macdonald Joinery has no
projects** - no work to place, rather than a dispute, a lost contract or a withheld payment.

## Key facts

| Item | Value | Source |
|---|---|---|
| Received, six months to 21 Aug 2026 | £162,986 | [^1] |
| Share of all third-party customer receipts | 80% | [^1] |
| Peak month (22 Feb - 21 Mar) | £63,832 | [^1] |
| Latest month (22 Jul - 21 Aug) | £8,660 | [^1] |
| Fall, peak to latest | 86% | derived |
| Month the fall happened | 22 Apr - 21 May 2026 | [^1] |
| **Reason** | **The customer has no projects** | [^2] |
| Whether temporary or permanent | **Not known** | [^2] |

## Details

### The payment record

| Statement month | Received |
|---|---:|
| 22 Feb - 21 Mar | £63,832 |
| 22 Mar - 21 Apr | £56,687 |
| 22 Apr - 21 May | £17,712 |
| 22 May - 21 Jun | £7,722 |
| 22 Jun - 21 Jul | £8,372 |
| 22 Jul - 21 Aug | £8,660 |

Two months at around £60,000, then a single step down, then a flat line at roughly £8,000.
Payments arrive both as plain "MACDONALD JOINERY" credits and against specific references
(FC0207, FC0208, FC0210, FC0214, MAC0215), so the relationship was job-based rather than a
single contract.

### What the owner said

Asked why the payments fell, the owner's answer on 2026-09-05 was that Macdonald Joinery **does
not have projects**. The full statement and what it does and does not settle are in
[the owner note](../../Raw/2026-09-05_owner-note_macdonald-joinery-has-no-projects.md).

This closes a question that five months of bank data could not: the fall was demand at the
customer, not a failure of the relationship. Nothing is in dispute, nothing was lost to a
competitor, and there is no debtor to pursue.

**It is also the explanation with the fewest routes back.** A dispute can be resolved, a
withheld payment can be chased, a completed contract can be followed by the next one. A
customer with no work offers none of those. The revenue returns only when Macdonald's own
demand returns, and Fishbone does not control that or, on the evidence here, have visibility of
it.

### What remains open

- **Whether it is temporary.** The statement describes a state now. It says nothing about
  whether Macdonald expects work to return, or when. Until that is known, no forecast should
  assume recovery from this customer.
- **What the residual ~£8,000 a month is.** It has been steady for three months, which is not
  what a stopped relationship looks like. It may be a small continuing job, a payment plan
  against an older balance, or a retention release. Unexamined.
- **Whether anything is still owed.** No receivable position has been checked. The QuickBooks
  A/R detail would answer it, and the sales ledger is not affected by the stale bank feed.

### Why it mattered so much

The company's cost base responded correctly to the fall. Subcontractor and material spend went
from £62,721 in the February-March period to £18,647 in June-July, tracking revenue down - see
[Subcontractors](../Suppliers/subcontractors.md). Payroll held flat at about £9,100.

What did not respond was debt service, at roughly £42,000 to £45,000 a month regardless. The gap
has been filled entirely by [related-party funding](../Finance/related-party-funding.md), around
£53,000 a month from Fishbone Properties Ltd and the directors.

With the reason now known, the consequence sharpens: **80% of receipts depended on one customer,
that customer has no work, and no other customer or pipeline is recorded anywhere in this
knowledge base.** The concentration risk did not just exist - it has already materialised.

## Open questions

- **What replaces this revenue?** This is now the first-order question. No sales pipeline, no
  contracted work and no other substantial customer appears anywhere in this knowledge base.
- Is Macdonald's lack of work expected to be temporary, and has anyone asked them?
- What is the residual ~£8,000 a month, and is it expected to continue?
- Is there an outstanding receivable? Check the QuickBooks A/R detail.
- What is the customer's full legal name and company number? The statements show only
  "MACDONALD JOINERY", and no contract, order or invoice from them is held in `Raw/`.

~~Why did payments fall 86% in May 2026? Contract completed, lost, disputed, or withheld.~~
**Answered 2026-09-05: the customer has no projects.** Retained here per `CLAUDE.md` §6d rule 2
so the record shows what was not known and for how long.

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-05 | Created from the six statement CSVs | `Outputs/change-log-2026-09-05-wiki-from-bank-data.md` |
| 2026-09-05 | Reason for the collapse recorded from the owner's statement; the five-way open question closed and the pipeline question raised in its place | `Outputs/change-log-2026-09-05-macdonald-answered.md` |

## Sources

[^1]: All six statement CSVs in [`Raw/Finance/`](../../Raw/Finance/), categorised and reconciled 2026-09-05.
[^2]: [Owner note, 2026-09-05](../../Raw/2026-09-05_owner-note_macdonald-joinery-has-no-projects.md) - verbal statement by the Managing Director, written up the same day.
