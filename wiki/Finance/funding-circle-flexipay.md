---
title: Funding Circle FlexiPay facility
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
  - ../../Raw/2024-10-31 Companies House certificate of change of name - Fishbone Drylining Ltd to Fishbone Construction Ltd (07948220).pdf
related:
  - ../Finance/debt-service.md
  - ../Finance/trading-receipts.md
  - ../Finance/related-party-funding.md
  - ../Finance/hmrc.md
---

# Funding Circle FlexiPay facility

A revolving facility, still held in the company's former name, which the company draws on and
repays continuously. It is the largest single item on the bank statements in both directions.
Over six months it **supplied no net cash at all**.

## Key facts

| Item | Value | Source |
|---|---|---|
| Drawn, six months to 21 Aug 2026 | £183,151 | [^1] |
| Repaid, same period | £205,255 | [^1] |
| **Net** | **minus £22,104** | derived |
| Repayment method | 25 to 37 separate direct debits a month | [^1] |
| Held in the name | Fishbone Drylining Ltd, the company's former name | [^2] |

## Details

### Drawn against repaid, by statement month

| Month | Drawn | Repaid | Net |
|---|---:|---:|---:|
| 22 Feb - 21 Mar | £20,000 | £29,015 | (£9,015) |
| 22 Mar - 21 Apr | £19,500 | £36,766 | (£17,266) |
| 22 Apr - 21 May | - | £34,222 | (£34,222) |
| 22 May - 21 Jun | £34,800 | £31,895 | +£2,905 |
| 22 Jun - 21 Jul | £30,000 | £38,368 | (£8,368) |
| 22 Jul - 21 Aug | £78,851 | £34,990 | +£43,862 |
| **Total** | **£183,151** | **£205,255** | **(£22,104)** |

August includes £59,451 of new borrowing drawn alongside the £80,807 iwoca repayment; treating
that as facility drawdown flatters the month. On the five months before it the facility is net
negative in four.

### Why this matters more than it looks

The group Loans database asked on 21 August 2026 whether Book 1's persistently negative net
cash movement reflected normal draw timing or a widening structural gap. **It is structural.**
The facility is amortising: the cash it supplies falls every month while the repayments it
demands do not. Book 1's own lifetime figure agrees, at minus £125,908.

But the six-month view puts that in proportion. The company's cash requirement after debt over
the same period was £497,071. A facility running at minus £22,104 net is not what kept the
company trading, and fixing it would not close the gap. What kept the company trading was
[related-party funding](related-party-funding.md).

### The name trap

Credits described **"Fishbone Drylining FC2603 / FC2505 / FC2522 / FC2605 / FLEXIPAY"** are
this company paying itself: drawdowns on its own facility, held under the name it traded as
before 31 October 2024. They are not receipts from a related company.

This was misread once in this knowledge base, on 2026-09-04, and £28,067 a month of borrowing
was counted as income. The fact had already been recorded in the group Loans database wiki on
21 August; the Loans folder had not been searched. `CLAUDE.md` §0 now carries a standing
instruction to check the sister knowledge bases before concluding anything about a counterparty
name.

Several trade suppliers also still hold the old name - see
[Trade suppliers](../Suppliers/trade-suppliers.md).

## Open questions

- What is the facility limit, and how much headroom remains?
- What are the fees? The group Loans database puts the overall rate on the HMRC-funding portion
  at 8.53%, but the facility's own pricing is not recorded here.
- Book 1 and Book 2 are tracked in the group Loans database. Are both still open, and does
  either have a repayment end date?
- Is the facility being renewed, and on what basis, given the fall in turnover?

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-05 | Created from the six statement CSVs | `Outputs/change-log-2026-09-05-wiki-from-bank-data.md` |

## Sources

[^1]: All six statement CSVs in [`Raw/Finance/`](../../Raw/Finance/), categorised and reconciled 2026-09-05.
[^2]: [Companies House certificate of change of name](../../Raw/2024-10-31%20Companies%20House%20certificate%20of%20change%20of%20name%20-%20Fishbone%20Drylining%20Ltd%20to%20Fishbone%20Construction%20Ltd%20(07948220).pdf), company 07948220, 31 October 2024.
