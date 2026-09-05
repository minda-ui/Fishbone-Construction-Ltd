---
title: Subcontractors
category: Suppliers
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
  - ../Finance/hsbc-current-account.md
  - ../Finance/hmrc.md
  - ../Customers/macdonald-joinery.md
  - ../Suppliers/trade-suppliers.md
---

# Subcontractors

The company's largest operating cost: **£190,647 over the six months to 21 August 2026**,
paid to 68 distinct payees. It is also the cost that responded correctly when revenue fell,
which is the one genuinely encouraging thing in the six-month data.

> **Sensitive.** Most payees are named individuals. Individual names and amounts are not
> reproduced here; they are in the statement CSVs in `Raw/Finance/`, which are Drive-only and
> never mirrored to git. Limited companies are named because a company is not personal data.

## Key facts

| Item | Value | Source |
|---|---|---|
| Total, six months to 21 Aug 2026 | £190,647 | [^1] |
| Distinct payees | 68 | [^1] |
| Paid to limited companies | £66,571 (35%) | [^1] |
| Paid to individuals | £124,076 (65%) | [^1] |
| Peak month (22 Feb - 21 Mar) | £58,471 | [^1] |
| Latest month (22 Jul - 21 Aug) | £18,464 | [^1] |

## Details

### The trend, and why it is good news

| Statement month | Subcontractors | Materials | Combined |
|---|---:|---:|---:|
| 22 Feb - 21 Mar | £58,471 | £4,249 | £62,721 |
| 22 Mar - 21 Apr | £54,482 | £1,685 | £56,167 |
| 22 Apr - 21 May | £27,763 | £23,138 | £50,901 |
| 22 May - 21 Jun | £19,379 | £16,895 | £36,273 |
| 22 Jun - 21 Jul | £12,088 | £6,560 | £18,647 |
| 22 Jul - 21 Aug | £18,464 | £6,854 | £25,317 |

Subcontractor spend fell 68% between March and July, over the same period that
[Macdonald Joinery](../Customers/macdonald-joinery.md) receipts fell 86%. The labour base is
genuinely variable: when work stops, the cost stops, with roughly a month's lag. Payroll -
employed staff rather than subcontract labour - stayed flat at about £9,100 a month throughout.

That is the difference between this cost base and the debt: one scales, the other does not.
See [Debt service](../Finance/debt-service.md).

### Composition

Payments are made against invoice references, typically weekly or fortnightly, and most payees
appear repeatedly - the largest individual payee received 19 separate payments over the six
months, another 25. This is a regular, ongoing labour supply, not casual engagement.

Limited-company subcontractors identifiable from the statements:

| Company | Six months | Pattern |
|---|---:|---|
| ANTN Projects Ltd | £30,637 | 12 payments against named job references (Initio 003-010, Rolex 001-002, Gap 001, gap/bbc002) |
| GAP Builders Ltd | £11,372 | 2 payments, invoice N 001 |
| Forth England Ltd | £15,000 (approx) | 8 payments, sequential invoice numbers Inv-1454 to Inv-1597 |
| Torin Construction | £1,840 | 1 payment, INV-0085 |

The ANTN Projects references ("Initio", "Rolex", "Gap") name jobs that do not appear anywhere
else in this knowledge base. They are not FP-prefixed project codes, so either they are the
subcontractor's own job names or the company runs work outside the FP numbering.

### The CIS question

The company pays 68 subcontractors in the construction industry. **Nothing in this knowledge
base addresses the Construction Industry Scheme at all** - not whether contractors are
verified, whether deductions are being made at 20% or 30% or gross, whether monthly CIS300
returns are being filed, or whether the deductions are being paid over.

That is a significant gap, not a minor one. CIS failures carry automatic penalties per return
per month, and the pattern in [HMRC](../Finance/hmrc.md) - no payment to HMRC leaving this
account between 22 April and 21 August - is consistent with CIS deductions not being paid over
as well as with PAYE. Neither is established.

## Open questions

- **Is CIS being operated?** Verification, deduction rates, monthly CIS300 returns, and payment
  over of deductions. None of it is documented here.
- Are these subcontractors correctly treated as self-employed rather than employed? 68 payees,
  many paid regularly over months, is the pattern HMRC looks at.
- What are "Initio", "Rolex" and "Gap"? Job names appearing on ANTN Projects payments that
  match no project in this knowledge base.
- Is there a subcontractor ledger anywhere showing what is owed as against what has been paid?
  The statements show payments out but not liabilities.
- Are there subcontract agreements on file? None is in `Raw/`.

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-05 | Created from the six statement CSVs | `Outputs/change-log-2026-09-05-wiki-from-bank-data.md` |

## Sources

[^1]: All six statement CSVs in [`Raw/Finance/`](../../Raw/Finance/), categorised and reconciled 2026-09-05. Individual payee detail is in the CSVs and is deliberately not reproduced in this article.
