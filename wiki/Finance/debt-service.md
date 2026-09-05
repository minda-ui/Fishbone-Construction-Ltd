---
title: Debt service
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
  - ../Finance/funding-circle-flexipay.md
  - ../Finance/trading-receipts.md
  - ../Finance/related-party-funding.md
---

# Debt service

What the company actually pays its lenders each month, taken from the bank statements rather
than from any schedule. **£350,803 over the six months to 21 August 2026**, against £204,309 of
third-party customer receipts in the same period.

## Key facts

| Item | Value | Source |
|---|---|---|
| Total debt service, six months | £350,803 | [^1] |
| Average per month | £58,467 | [^1] |
| Funding Circle share | £205,255, 59% of the total | [^1] |
| Funding Circle monthly average | £34,209 | [^1] |
| Funding Circle direct debits per month | between 25 and 37 | [^1] |
| Facilities appearing in the statements | 9 | [^1] |

## Details

### By lender, six months to 21 August 2026

| Lender | Six months | Notes |
|---|---:|---|
| Funding Circle | £205,255 | Revolving FlexiPay, paid by many small GoCardless direct debits. See [Funding Circle FlexiPay](funding-circle-flexipay.md) |
| iwoca | £100,861 | All in Jun-Aug; £80,807 of it in August, a refinance rather than a run rate |
| LendingCrowd | £14,330 | £2,388 a month, unvarying |
| Nucleus | £13,959 | £1,994, taken twice in some months |
| Haydock (HP) | £7,556 | £1,210 a month |
| HSBC loan | £3,105 | £518 a month, unvarying |
| MotoNovo (HP) | £2,759 | £460 a month, unvarying |
| SSAS loanback | £2,604 | £401-£501 a month by standing order |
| Tower Leasing | £373 | One payment, August only |
| **Total** | **£350,803** | |

### The shape of the problem

Funding Circle by statement month: £29,015, £36,766, £34,222, £31,895, £38,368, £34,990.

That figure barely moves. Over the same six months third-party customer receipts fell from
£75,322 to under £10,000 a month, and subcontractor and material spend fell with them - the
variable cost base did what a variable cost base should. Debt service did not move at all,
because it cannot.

Operating cash flow before debt was **positive £27,639** in the 22 February to 21 March period
and negative in all five months since, **minus £119,057** over the six months as a whole. After
debt service and HMRC the six-month cash requirement was **£497,071**, an average of £82,845 a
month, and every pound of it came from related parties - see
[Related-party funding](related-party-funding.md).

### The August figure is not a run rate

August debt service reads £123,240. Of that, £80,807 went to iwoca and £59,451 of new borrowing
came in on the other side. That is a refinance. Stripping it out, the underlying monthly debt
service across the six months is roughly £42,000 to £45,000.

### On the Payment Calendar

The group Loans database keeps a Payment Calendar covering twelve fixed-schedule facilities. It
**correctly excludes** the revolving FlexiPay books, which that database tracks separately as
Book 1 and Book 2, so the calendar is not defective. The gap is that no single document
anywhere consolidates the two. A reader of the calendar alone understates cash leaving the
company by roughly £18,700 a month.

## Open questions

- What are the terms of each facility - rate, term, security, personal guarantees? None of that
  is in this knowledge base; the group Loans database holds it and is authoritative.
- Is the iwoca facility now closed, or was August a partial repayment? The statements show a
  large repayment and a new drawdown in the same month but not what either instrument is.
- What was the £59,451 drawn in August, and on what terms? It appears as
  "FUNDING CIRCLE LIM / FCT5805" and is treated here as new borrowing.
- Tower Leasing appears once, in August. What is the asset and what is the schedule?

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-05 | Created from the six statement CSVs | `Outputs/change-log-2026-09-05-wiki-from-bank-data.md` |

## Sources

[^1]: All six statement CSVs in [`Raw/Finance/`](../../Raw/Finance/), categorised and reconciled 2026-09-05.
