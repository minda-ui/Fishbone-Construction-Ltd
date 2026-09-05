---
title: Data capture and accounting systems
category: Processes
status: active
sensitive: false
created: 2026-09-05
updated: 2026-09-05
sources:
  - ../../Raw/Finance/20260821_04212819.csv
related:
  - ../Finance/hsbc-current-account.md
  - ../Finance/hmrc.md
  - ../Suppliers/trade-suppliers.md
  - ../Projects/fp-2401-goathland-avenue.md
---

# Data capture and accounting systems

**The company's automated bookkeeping has been broken since late August 2026 and nothing
alerted anyone.** Every figure in this knowledge base comes from manually exported CSVs and
hand-read invoices, not from a live feed. This article records the state of the systems, because
a reader who assumes the accounts are current will be wrong.

## Key facts

| System | State as of 2026-09-05 | Source |
|---|---|---|
| Dext (document capture) | **Failing since 24 August 2026.** Uploads error | [^1] |
| QuickBooks bank feed | **Stale since at least 2 September 2026** | [^1] |
| Intuit consent | Expiring | [^1] |
| HSBC statements | Manual CSV export into `Raw/Finance/`, current to 21 Aug 2026 | [^2] |
| Smartsheet Classifier and Budget | Live and working | [^3] |
| Companies House filings | Late-filing penalties charged 20 Apr 2026 | [^2] |

## Details

### How the breakage was found

The HSBC 2819 balance read **exactly £18,592.62** in QuickBooks on both 2 and 4 September 2026.
An identical balance two days apart on an account that turns over £150,000 a month is not a
quiet week; it is a feed that has stopped. Dext upload failures dated from 24 August.

Neither failure raised an alert. Both were found by someone happening to look, more than a week
after the first one started. That is the actual finding here: the failure mode is silent, and
nothing in the current setup would catch the next one either.

`CLAUDE.md` §5 proposes a daily data-capture watchdog for exactly this. It is not built.

### Consequences for anything read from QuickBooks

Reconnecting the bank feed needs an HSBC login and cannot be done without the owner. Until it
is:

- **QuickBooks bank balances and any cash figure derived from them are stale.** Do not quote
  them.
- The sales and purchase ledgers are not fed by the bank feed and remain usable, with the
  caveats below.
- Anything after 21 August 2026 is invisible everywhere. The next HSBC statement (22 Aug to
  21 Sep) is the only route to current data.

### Known integrity defects in QuickBooks

Recorded 2026-09-04 and not since re-checked:

| Defect | Detail |
|---|---|
| Net income disagreement | Balance sheet reports net income of £2,866 at 2 September; the P&L for the same date reports a loss of £433,119 |
| A/P disagreement | A/P aging totals £57,034 against £52,222 in the balance sheet - a difference of £4,812 |
| A/R display error | The A/R aging summary shows a headline of £106,968 which double-counts subtotal rows. The correct figure is £55,656 and ties exactly to the balance sheet |
| Duplicate party | Sebastian Pabis appears as £50,506 owed by this company per A/P, and separately as a £35,000 related-party loan to Fishbone Properties Ltd per the group Loans database, never repaid. Either two exposures of about £85,000, or one debt against the wrong entity |

The A/R headline is a display artefact and the underlying figure is sound. The net income
disagreement is not explained and is large enough to matter.

### The manual chain that currently substitutes

| Data | How it actually gets here |
|---|---|
| Bank transactions | Owner exports HSBC CSV monthly into `Raw/Finance/`; categorised and reconciled against printed balances |
| Supplier invoices | Emailed or photographed, dropped into the project folder in `Raw/`, read one by one |
| Project costs | Hand-entered into the Smartsheet Classifier and Budget, per the FP 2401 session-starter |
| Lender positions | The group Loans database, maintained separately |

This works, and the six-month bank analysis it produced reconciles to the penny. It does not
scale and it is not timely: the analysis was possible only because someone spent a session on
it.

## Open questions

- **When will the QuickBooks bank feed be reconnected?** Needs an HSBC login and the owner.
- **Why is Dext failing?** Subscription, credential or integration - not diagnosed.
- What explains the £2,866 against £433,119 net income disagreement in QuickBooks?
- Are the statutory accounts now filed, and what were the April penalties for?
- Should the bank-statement categoriser become a routine? It exists as a working script with a
  reconciliation check; it has no home in the knowledge base and runs only when someone runs it.

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-05 | Created from the findings of 2026-09-04 and 2026-09-05 | `Outputs/change-log-2026-09-05-wiki-from-bank-data.md` |

## Sources

[^1]: Observed 2026-09-02 and 2026-09-04; recorded in `Wiki/Change Log` (closed), entry dated 2026-09-05, findings 6 and 7.
[^2]: [`Raw/Finance/`](../../Raw/Finance/) statement CSVs; Companies House penalties appear as debits dated 20 Apr 2026.
[^3]: `Wiki/FP 2401 Goathland Avenue - Actuals Processing Instructions`.
