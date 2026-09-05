---
title: Macdonald Joinery
category: Customers
status: active
sensitive: true
created: 2026-09-05
updated: 2026-09-05
sources:
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
receipts in the six months to 21 August 2026. **Its payments fell 86% in a single month in May
2026 and have not recovered.** Why is the most important unanswered question about this
business.

## Key facts

| Item | Value | Source |
|---|---|---|
| Received, six months to 21 Aug 2026 | £162,986 | [^1] |
| Share of all third-party customer receipts | 80% | [^1] |
| Peak month (22 Feb - 21 Mar) | £63,832 | [^1] |
| Latest month (22 Jul - 21 Aug) | £8,660 | [^1] |
| Fall, peak to latest | 86% | derived |
| Month the fall happened | 22 Apr - 21 May 2026 | [^1] |
| Reason | **Unknown** | - |

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

Two months at around £60,000, then a single step down, then a flat line at roughly £8,000. The
three months since are remarkably consistent, which suggests something regular and small
continued rather than the relationship ending outright.

Payments arrive both as plain "MACDONALD JOINERY" credits and against specific references
(FC0207, FC0208, FC0210, FC0214, MAC0215), so the relationship is job-based rather than a
single contract.

### Why this matters

The company's cost base responded correctly. Subcontractor and material spend fell from £62,721
in the February-March period to £18,647 in June-July, tracking revenue down - see
[Subcontractors](../Suppliers/subcontractors.md). Payroll held flat at about £9,100.

What did not respond was debt service, at roughly £42,000 to £45,000 a month regardless. The
gap between the two has been filled entirely by
[related-party funding](../Finance/related-party-funding.md), around £53,000 a month.

So the collapse of this one customer relationship is the proximate cause of the company's
current position. Everything downstream - the £497,071 six-month shortfall, the director loans,
the pressure on Fishbone Properties Ltd - follows from it.

### What is not known

Nothing in this knowledge base explains the fall. The candidate explanations are materially
different from each other:

| If | Then |
|---|---|
| A contract completed on schedule | Normal. The question becomes what replaces it, and the answer is that nothing has |
| A contract was lost or cancelled | The relationship is damaged and the pipeline question is urgent |
| Work is in dispute | There may be a receivable to pursue, and a liability to assess |
| Payment is being withheld or delayed | This is a debtor problem, potentially recoverable |
| Macdonald Joinery itself is in difficulty | The exposure is a bad-debt risk, and any continuing work may be unwise |

Each implies a different response. Guessing between them would be worse than leaving the
question open.

### How to close it

None of this needs new systems, only someone to look:

1. **The QuickBooks A/R detail for Macdonald Joinery** - what was invoiced against what was
   paid, and what is outstanding. Note the bank feed is stale, but the sales ledger is not
   dependent on it.
2. **Email correspondence, March to June 2026** - a completion, a dispute or a cancellation
   normally leaves a trail.
3. **The Smartsheet project register** - whether an FP project for Macdonald work closed out in
   April or May.
4. **Ask the director.** This is the fastest route and the answer is probably known.

## Open questions

- **Why did payments fall 86% in May 2026?** Contract completed, lost, disputed, or withheld.
- Is there an outstanding receivable, and how old is it?
- Is any work still in progress for this customer? The steady ~£8,000 a month suggests
  something is.
- What is the customer's full legal name and company number? The statements show only
  "MACDONALD JOINERY", and no contract, order or invoice from them is held in `Raw/`.
- What replaces this revenue? No pipeline or sales ledger forecast exists in this knowledge base.

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-05 | Created from the six statement CSVs | `Outputs/change-log-2026-09-05-wiki-from-bank-data.md` |

## Sources

[^1]: All six statement CSVs in [`Raw/Finance/`](../../Raw/Finance/), categorised and reconciled 2026-09-05.
