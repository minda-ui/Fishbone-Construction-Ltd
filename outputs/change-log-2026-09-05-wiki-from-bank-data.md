# 2026-09-05 - Wiki built from the six months of bank data

Owner chose this over three alternatives (investigating the Macdonald collapse, migrating the
legacy Google Docs, mirroring to git). The problem it fixes: everything this knowledge base had
learned about the company lived in change-log entries, which are **written once and never
revised**. That is the right home for "what happened in a session" and the wrong home for facts
that change - a balance, a customer relationship, a lender position. Twelve articles now carry
those facts where they can be updated.

## Created

Five new category folders - `Finance/`, `Customers/`, `Suppliers/`, `Projects/`, `Processes/` -
and twelve articles.

| Article | What it carries |
|---|---|
| `Finance/hsbc-current-account.md` | The account itself, six months, the reconciliation method, monthly closing balances, the undocumented second account 24241061 |
| `Finance/trading-receipts.md` | Receipts by month and source; supersedes the £16,855/month run-rate figure |
| `Finance/debt-service.md` | £350,803 over six months, by lender |
| `Finance/funding-circle-flexipay.md` | Drawn against repaid; net minus £22,104; the former-name trap |
| `Finance/related-party-funding.md` | £319,460 from the group and the directors |
| `Finance/hmrc.md` | The four-month silence, Time to Pay, VAT, the CIS gap |
| `Customers/macdonald-joinery.md` | The 86% collapse, what it caused, and the four ways to find out why |
| `Customers/at-uk-interiors.md` | `draft` - records an unresolved classification worth £25,447 |
| `Suppliers/subcontractors.md` | £190,647, 68 payees, the cost base that did scale, and the CIS question |
| `Suppliers/trade-suppliers.md` | Fifteen suppliers, concentration, accounts still in the old name |
| `Projects/fp-2401-goathland-avenue.md` | The only documented project; scope inferred from what was bought |
| `Processes/data-capture-and-accounting-systems.md` | Dext and the QuickBooks feed both broken, silently; the QuickBooks integrity defects |

`Wiki/index.md` and `Outputs/kb-registers.md` were re-issued to list them; both previous copies
archived with their reason.

## What changed in the telling, not just the filing

Three things read differently once written up as articles rather than as findings.

**1. The £16,855 figure is now explicitly superseded, in the place a reader will look.** It was
derived from June-August alone and treated as a run rate. Six months show it is the floor after
a collapse: the three months before averaged over £50,000 from third parties. The 13-week cash
flow forecast of 4 September rests on it and has still not been re-issued.

**2. The August "recovery" mostly is not one.** Third-party receipts read £34,064 in the 22 July
to 21 August month, against £10,542 the month before. But £15,000 of it is
`Wiki/Customers/at-uk-interiors.md`, whose status as a customer is unresolved, and £10,140 was a
one-off from Formbuild Installations on 31 July. Macdonald itself paid £8,660 - flat. Writing
the month out line by line made that visible in a way the monthly total did not.

**3. Fishbone Properties money arrives labelled "Loan Payback".** £221,050 of the £232,870 gross
inflow from that company is described that way. If the wording reflects the substance, Fishbone
Properties is **repaying a debt it already owed this company** rather than lending new money -
which means this company has been consuming an asset, not incurring a liability, and the
intercompany balance runs the other way from the assumption made so far. Nothing here
establishes which it is, and a reference on a bank line is not evidence of the legal character
of a payment. It is now an open question on the article rather than an unexamined word in a CSV.

## A gap that had not been named before

**CIS.** The company pays 68 subcontractors in the construction industry, £190,647 over six
months, most of them named individuals paid repeatedly over months. Nothing in this knowledge
base addresses the Construction Industry Scheme at all - not verification, not deduction rates,
not monthly CIS300 returns, not payment over of deductions.

It is recorded as an open question on `Suppliers/subcontractors.md` and cross-referenced from
`Finance/hmrc.md`, because the four-month absence of any HMRC payment from the bank account is
consistent with CIS deductions not being paid over as well as with PAYE. Neither is established
and both are checkable.

The employment-status question sits alongside it: 68 payees, many paid regularly over months,
is the pattern HMRC examines.

## Handling of personal data

`Suppliers/subcontractors.md` is the first article where §2's sensitive-data rule bites. 65% of
subcontract spend goes to named individuals. The article gives totals, counts, the trend and the
limited companies by name; it does not reproduce individual names or amounts, and says so
explicitly, pointing to the Drive-only CSVs instead. Articles resting on bank data are marked
`sensitive: true`.

## Status of the Processed items register

The six statement CSVs moved from `partial` to `done`. They were `partial` because their
findings existed only in change-log entries; that was the whole point of this session and it is
now closed.

## Not done

- **`Customers/at-uk-interiors.md` is a `draft` on purpose.** It records that a classification
  is unresolved and what turns on it. Writing it as settled either way would have been a guess
  worth £25,447 of the six-month receipts figure.
- **No article for Formbuild Installations.** One receipt of £10,140 in six months is not yet a
  relationship; it is noted in `Finance/trading-receipts.md` as an open question.
- **One article per supplier was not written.** Fifteen suppliers, most with a single invoice.
  `Suppliers/trade-suppliers.md` covers the base and `Raw/FP 2401_131 Goathland Avenue/INDEX.md`
  covers the files. Splitting it out would be filing for its own sake.
- **The five legacy Google Docs are still unfiled** at the root of `Wiki/`, still listed under
  "Unfiled" in `index.md`, still awaiting an owner decision.
- **The git mirror still carries none of this.** Only `wiki/change-log.md` has been updated in
  `minda-ui/Fishbone-Construction-Ltd` this session.

## Notes for next session

- The wiki now has substance but almost no coverage of what happens next: no pipeline, no
  contracted work, no forecast that reflects the six-month data. The 13-week forecast is the
  obvious thing to re-issue, and it should state that £16,855 is a post-collapse figure.
- **The Macdonald question is still open and is still the most important one.** Four concrete
  routes to close it are listed on that article: the QuickBooks A/R detail, email correspondence
  March-June, the Smartsheet project register, and asking the director.
- Two articles now carry group-level questions that cannot be answered from inside this
  knowledge base - the intercompany balance direction with Fishbone Properties Ltd, and the
  duplicate Sebastian Pabis exposure. Both are candidates to pass to Fishbone Group, per
  `CLAUDE.md` §0.
