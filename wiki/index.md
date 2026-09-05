# Wiki index

Entry point for the Fishbone Construction Ltd knowledge base.
Every article must be listed here. Categories and articles are alphabetical.
Maintenance rules: `../CLAUDE.md`, section 2.

Line format: `- [Title](Category/file-name.md) - one-line description`

> **Start here if you want the picture in one line:** the company's only substantial customer
> stopped paying in May 2026 because that customer has no work, the cost base followed revenue
> down but the debt did not, and since then the gap has been filled by about £53,000 a month
> from the group and the directors. No replacement revenue is recorded anywhere.
> [Macdonald Joinery](Customers/macdonald-joinery.md) →
> [Debt service](Finance/debt-service.md) →
> [Related-party funding](Finance/related-party-funding.md).

## Contracts

_(none yet: no customer contract, subcontract agreement, lease or facility agreement is held in
`Raw/`. This is a real gap - every financial article below describes an arrangement whose terms
are unknown.)_

## Customers

- [AT UK Interiors Ltd](Customers/at-uk-interiors.md) - `draft`. £25,447 received against job references, but the counterparty may be a related party. Unresolved
- [Macdonald Joinery](Customers/macdonald-joinery.md) - the only substantial customer, 80% of receipts; payments fell 86% in May 2026 because the customer has no projects. Nothing replaces the revenue

## Decisions

- [Standard KB skeleton adopted](Decisions/2026-09-05-kb-skeleton-adopted.md) - what was copied from the Fishbone Commercial Properties Ltd model, what was changed for a trading company, and what was deliberately left alone

## Finance

- [Debt service](Finance/debt-service.md) - £350,803 over six months across nine facilities; the cost that did not fall when revenue did
- [Funding Circle FlexiPay facility](Finance/funding-circle-flexipay.md) - drew £183,151, repaid £205,255; supplied no net cash. Held in the company's former name
- [HMRC - PAYE, Time to Pay and VAT](Finance/hmrc.md) - no payment to HMRC left the account between 22 April and 21 August 2026
- [HSBC current account 04212819](Finance/hsbc-current-account.md) - the main account; six months categorised and reconciled to every printed balance
- [Related-party funding](Finance/related-party-funding.md) - £319,460 from the group and the directors covered a £497,071 shortfall
- [Trading receipts](Finance/trading-receipts.md) - what the company was actually paid for work, by month and by source

## People

_(none yet: the directors M Gaudiesius and A Prutkovas appear throughout the finance articles
and have no article of their own)_

## Processes

- [Data capture and accounting systems](Processes/data-capture-and-accounting-systems.md) - Dext and the QuickBooks bank feed are both broken and nothing alerted anyone; the QuickBooks integrity defects

## Projects

- [FP 2401 - 131 Goathland Avenue](Projects/fp-2401-goathland-avenue.md) - the only documented project; 99 supplier documents, scope inferred from what was bought

## Suppliers

- [Subcontractors](Suppliers/subcontractors.md) - £190,647 to 68 payees; the cost base that did scale, and the unexamined CIS question
- [Trade suppliers](Suppliers/trade-suppliers.md) - fifteen merchants; three accounts still in the company's former name

## Unfiled (Google Docs, at the root of `Wiki/`)

These pre-date the skeleton. They are live and authoritative; they are simply not yet in a
category folder or in Markdown. In this git mirror they appear as `wiki/*.md` at this level.

- [Change Log](https://docs.google.com/document/d/1yaATUPhHuuXOvJ1oi-DLi-gWn1ykTXoYXMhntgOjntc/edit) - the four historical session entries, 25 August to 5 September 2026. **Closed 2026-09-05: no longer appended to.** Session logging moved to dated files in `Outputs/`. Mirror: [`change-log.md`](change-log.md)
- [Database Structure](https://docs.google.com/document/d/1B0QcXDWazh8KlgOXV8Ei7T-cW4ZegGhLwuTuGvfmvoY/edit) - the Smartsheet Classifier and Budget sheets, and how they relate. Belongs in `Processes/`. Mirror: [`database-structure.md`](database-structure.md)
- [FP 2401 Goathland Avenue - Actuals Processing Instructions](https://docs.google.com/document/d/1L9LR-lo6zZopDsVXLL_wBEKfKFk1RSniTYkzNeqX6Ik/edit) - copy-paste session-starter for the invoice-to-actuals task. Re-issued 2026-09-05. Belongs in `Projects/`. Mirror: [`fp-2401-goathland-avenue-actuals-processing-instructions.md`](fp-2401-goathland-avenue-actuals-processing-instructions.md)
- [Processing Workflow](https://docs.google.com/document/d/1Ll7U39oormzFJBqZUVBYIWFuLHUSh7DOYQ3RwCVTSsA/edit) - how a Raw item becomes Classifier and Budget rows. Belongs in `Processes/`. Mirror: [`processing-workflow.md`](processing-workflow.md)
- [Wiki Maintenance Guidelines](https://docs.google.com/document/d/1mXih5Syp9WkcWuKU68pm6WXoSF8hhjOGJaSx9qoO6Ww/edit) - the original wiki rules. Now partly superseded by `../CLAUDE.md` section 2. Belongs in `Processes/`. Mirror: [`wiki-maintenance-guidelines.md`](wiki-maintenance-guidelines.md)

## Open questions on this wiki

- Should the five Google Docs above be converted to Markdown and moved into category folders?
  It would make the wiki uniform and diffable, but it changes URLs the owner has been using and
  the "Reference locations" block inside the Goathland instructions. Not done without an
  instruction.
- **No `Contracts/` article exists because no contract is held.** Every financial article
  describes an arrangement - a lending facility, a Time to Pay, an intercompany loan, a customer
  relationship - whose written terms are unknown to this knowledge base.
- **Nothing here covers what happens next: no sales pipeline, no contracted work, no quote, no
  forecast that reflects the six-month data.** As of 2026-09-05 this is the knowledge base's
  first open question, not its last - the customer behind 80% of receipts has no projects, and
  nothing is recorded that would replace them. The 13-week cash flow forecast of 4 September
  rests on a superseded receipts assumption, was built before that was known, and has not been
  re-issued.

---

Superseded copies of this file sit in `Archive/`, each titled with its reason, per
`../CLAUDE.md` §1. One of them exists only because an earlier copy asserted a count without
counting, which `../CLAUDE.md` §6d rule 3 forbids. The current total is in
[`../archive/README.md`](../archive/README.md), which states when it was counted; the archived
contents are Drive-only.
