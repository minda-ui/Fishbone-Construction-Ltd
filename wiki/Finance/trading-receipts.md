---
title: Trading receipts
category: Finance
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
  - ../Finance/related-party-funding.md
  - ../Finance/funding-circle-flexipay.md
  - ../Finance/hmrc.md
  - ../Customers/macdonald-joinery.md
  - ../Customers/at-uk-interiors.md
---

# Trading receipts

Money the company received for work done, as distinct from money it borrowed or was lent by
related parties. Separating the two is the single most important step in reading these
statements, and getting it wrong was the biggest error made in this knowledge base.

## Key facts

| Item | Value | Source |
|---|---|---|
| Third-party customer receipts, six months | £204,309 | [^1] |
| Total trading cash in, six months (incl. VAT refunds and group job work) | £224,914 | [^1] |
| Peak month (22 Feb - 21 Mar) | £75,322 from third parties | [^1] |
| Trough month (22 May - 21 Jun) | £7,749 from third parties | [^1] |
| Fall, peak to trough | 90% | derived |
| Concentration | Macdonald Joinery is 80% of all third-party receipts | [^1] |

## Details

### The trend

| Statement month | Third-party customers | Fishbone Properties job work (net) | VAT refunds | Total trading in |
|---|---:|---:|---:|---:|
| 22 Feb - 21 Mar | £75,322 | £11,500 | £10,109 | £96,930 |
| 22 Mar - 21 Apr | £58,387 | (£4,320) | - | £54,067 |
| 22 Apr - 21 May | £18,245 | £5,500 | - | £23,745 |
| 22 May - 21 Jun | £7,749 | (£8,900) | £8,915 | £7,764 |
| 22 Jun - 21 Jul | £10,542 | £1,800 | - | £12,342 |
| 22 Jul - 21 Aug | £34,064 | (£4,000) | - | £30,064 |

The August recovery is not a return to trading. Of that £34,064, **£15,000 came from
[AT UK Interiors](../Customers/at-uk-interiors.md)** whose status as a customer is unresolved,
and **£10,140 was a one-off receipt from Formbuild Installations** on 31 July. Macdonald
Joinery itself contributed £8,660, in line with the three preceding months.

The collapse is documented in [Macdonald Joinery](../Customers/macdonald-joinery.md).

### The £16,855 figure is superseded

An earlier reading, based on the June to August statements alone, put trading receipts at
£16,855 a month and treated that as a run rate. With six months of data that figure is
**the floor after a collapse, not a steady state**: the three months before it averaged over
£50,000 a month from third parties. Any forecast built on £16,855 as a normal level is
describing the post-collapse company, and should say so.

This matters because the 13-week cash flow forecast dated 4 September 2026 was built on exactly
that assumption. It has not been re-issued.

### Fishbone Properties job work is not a receipt stream

Transactions with Fishbone Properties Ltd carrying a job reference net to **£1,580 over six
months and run in both directions** - some months the money comes in, some months it goes out.
An earlier reading treated £4,500 a month of it as customer income. It is not a reliable
receipt stream, and the much larger figure moving between the two companies is lending, not
trading: see [Related-party funding](related-party-funding.md).

### What is not a receipt

Credits described as **"Fishbone Drylining FC2603 / FC2505 / FC2522 / FC2605 / FLEXIPAY"** are
the company drawing down its own Funding Circle facility, still held under its former name.
They are financing, not sales - £123,700 over six months. See
[Funding Circle FlexiPay](funding-circle-flexipay.md). A first pass over the statements
classified these as income and overstated receipts by roughly £28,000 a month.

## Open questions

- Is there a sales ledger or pipeline anywhere that shows what work is actually contracted for
  the months after August 2026? Nothing in this knowledge base answers what the company expects
  to invoice next.
- Is [AT UK Interiors](../Customers/at-uk-interiors.md) a customer or a related party? £25,447
  of the six-month total depends on the answer.
- Was the Formbuild Installations receipt of £10,140 a one-off or the start of something? Only
  one payment appears in six months.

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-05 | Created; supersedes the £16,855/month run-rate figure | `Outputs/change-log-2026-09-05-wiki-from-bank-data.md` |

## Sources

[^1]: All six statement CSVs in [`Raw/Finance/`](../../Raw/Finance/), categorised and reconciled 2026-09-05.
