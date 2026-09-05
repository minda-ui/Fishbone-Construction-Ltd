---
title: HSBC current account 04212819
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
  - ../Finance/trading-receipts.md
  - ../Finance/debt-service.md
  - ../Finance/related-party-funding.md
  - ../Finance/hmrc.md
  - ../Suppliers/subcontractors.md
  - ../Processes/data-capture-and-accounting-systems.md
---

# HSBC current account 04212819

The company's main trading account and the only one this knowledge base has data for. Six
monthly statements covering **22 February to 21 August 2026** have been categorised, and the
categorisation reconciled against every printed running balance. This article is the entry
point to everything derived from them.

## Key facts

| Item | Value | Source |
|---|---|---|
| Period covered | 22 Feb 2026 to 21 Aug 2026, six statement months | [^1] |
| Transactions | 1,848 | [^1] |
| Opening balance, 22 Feb 2026 | £326.66 | [^2] |
| Closing balance, 21 Aug 2026 | £5,867.23 | [^3] |
| Net movement over six months | +£5,541 | [^1] |
| Total paid in | £891,445 | [^1] |
| Total paid out | £885,905 | [^1] |
| Reconciliation | All 160 printed running balances recomputed and matched to the penny | [^1] |
| Unclassified residue | 21 transactions, £1,039 (0.1% of throughput) | [^1] |

## Details

**The account runs at close to nil.** It ends five of the six months between £50 and £11,388,
and the low point is £50.87 on 21 July 2026. Nearly £900,000 passed through it in six months
against a balance that never held more than about £11,000. It is a conduit, not a reserve.

Monthly closing balances and net movement:

| Statement month | Closing balance | Net movement |
|---|---:|---:|
| 22 Feb - 21 Mar | £465.67 | +£139 |
| 22 Mar - 21 Apr | £4,860.76 | +£4,395 |
| 22 Apr - 21 May | £6,182.25 | +£1,321 |
| 22 May - 21 Jun | £11,388.00 | +£5,206 |
| 22 Jun - 21 Jul | £50.87 | -£11,337 |
| 22 Jul - 21 Aug | £5,867.23 | +£5,816 |

A net movement near zero every month is not stability. It is the arithmetic result of
related-party money arriving in whatever amount the month's shortfall demanded - see
[Related-party funding](related-party-funding.md). The account balance carries no information
about whether the business is solvent, which is why the categorisation matters.

**What flows through it**, monthly averages over the six months:

| | Per month |
|---|---:|
| Trading cash in (customers, VAT refunds, group job work) | £37,486 |
| Operating cash out (subcontractors, materials, payroll, overheads) | (£57,328) |
| **Operating cash flow before debt** | **(£19,843)** |
| Debt service, all facilities | (£58,467) |
| HMRC direct payments | (£4,535) |
| **Cash requirement after debt** | **(£82,845)** |
| Own FlexiPay drawdowns and new borrowing | £30,526 |
| Related-party funding, net in | £53,243 |
| **Net movement** | **+£923** |

The August debt-service figure (£123,240) is inflated by an iwoca refinance and is not a run
rate - see [Debt service](debt-service.md).

### The reconciliation, and why it is stated

Each statement prints a running balance on the last transaction of each day. The opening
balance was derived from the first printed balance by working backwards through that day's
movements, then the balance was walked forward transaction by transaction and compared against
every printed value. All 160 matched exactly, in all six months. Nothing is missing from the
categorisation and nothing is counted twice.

This check is what makes the derived figures usable. Without it a categorisation is an
assertion. `CLAUDE.md` §3d makes it a standing requirement before any figure from a statement
is quoted.

### A second account exists and is not documented

Account **24241061** transferred a net £7,877 into this account across 24 separate transfers in
the 22 February to 21 March period, then effectively stopped: net minus £50 in March-April,
plus £52 in April-May, and nil in the three months after. In the 22 July to 21 August period 14
transfers passed both ways and netted to zero.

Its balance, purpose and current state are unknown to this knowledge base.

## Open questions

- What is account 24241061 for, what is its balance, and why did the transfers stop in March?
- Are there other company accounts? The six statements are for one account only, and no
  statement or list of accounts has been supplied for anything else.
- The QuickBooks bank feed for this account has been stale since at least 2 September 2026, so
  nothing after 21 August is visible anywhere. See
  [Data capture and accounting systems](../Processes/data-capture-and-accounting-systems.md).

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-05 | Created from the six statement CSVs | `Outputs/change-log-2026-09-05-wiki-from-bank-data.md` |

## Sources

[^1]: All six statement CSVs in [`Raw/Finance/`](../../Raw/Finance/), categorised and reconciled 2026-09-05. Method and totals: `Outputs/change-log-2026-09-05-six-month-bank-data.md`.
[^2]: [`Raw/Finance/20260321_04212819.csv`](../../Raw/Finance/20260321_04212819.csv), derived from the first printed running balance.
[^3]: [`Raw/Finance/20260821_04212819.csv`](../../Raw/Finance/20260821_04212819.csv), final printed running balance.
