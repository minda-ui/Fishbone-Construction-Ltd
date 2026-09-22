# Fishbone Construction Ltd - Knowledge Base

> **Status: AUTHORITATIVE. Version 12, 2026-09-22**, superseding v11 of 2026-09-11 (in `Archive/`).
> **This version adds §4d, recording Anna (AI Construction Assistant) as an authorised contributor
> to this KB on Minda's sanction of 2026-09-22 (Hub AWT-0077), and corrects this file's citation of
> the shared house rules document from v1.1 to v1.3 in three places - this banner, the §0-§5
> introduction and the closing note. The house rules reached v1.2 and then v1.3 on 2026-09-12
> (adding the Collaboration Space & Smartsheet boundary, §10, and the related-party cross-linking
> requirement, §11); this file had cited v1.1 since v11 was written, and Anna's own charter had the
> same stale citation. The §4d entry is deliberately one short paragraph - the detail lives in
> `Wiki/Decisions/2026-09-22-anna-construction-adviser-write-access.md`, per §4c rule 3. Nothing
> else in this file changed.**
>
> **v11, 2026-09-11** restructured the file around the Fishbone Group's shared house rules document,
> `Wiki/Process-Fishbone-Systems-House-Rules.md` (v1.3), in the Fishbone Group's Wiki folder.
> Sections that stated conventions common to every company KB - the folder pattern, the
> archive-then-recreate mechanics, the Wiki article discipline, the change-log file convention,
> the shared governance baseline, and the rules for maintaining a standing control file - now link
> to that document instead of restating it, per Minda's instruction to shrink this file (alongside
> Fishbone Holdings Ltd's) and compare before and after. Nothing that is specific to this company -
> its folder ids, its live-data-source table, its project procedures, its reading-limits lessons,
> its own governance additions, or its company snapshot and open questions in §7 - has moved or
> been shortened. See the before/after report filed alongside this replacement for the detail of
> what changed. This file keeps its own version history in this banner, not a separate change-log
> section; the closing note at the foot of the file lists every version this one supersedes.
>
> **The pre-v11 version history, kept in full below because it is this company's own institutional
> memory, not a restatement of shared rules:** v10 corrected v9's §1 live-data-sources table to say
> the group Document Register policy was at v1.3, not v1.2 - found on a `/Raw` check the day after
> v9. v1.3 resolves two *other* companies' change requests (`FM-CR-0001`, `FP-CR-0001`; not this
> KB's) with two clarifications: self-assigned 4-digit property codes (not applicable - this KB
> owns no property) and a Gmail-thread-id-plus-transcription pattern for email attachments that
> can't be captured into Drive (directly relevant to this KB's own info-mailbox pipeline, which has
> carried that exact gap since 2026-09-06 - using the new pattern on the existing backlog is
> separate, undecided work). The same `/Raw` check also found a new inbound document,
> `22910 FISHBONE.pdf` - a software quote from Kosmosoft Engineering S.r.l. for "SmartCABINET"
> CAD/CAM software, addressed to the company's old name; registered `pending` in
> `Outputs/kb-registers.md`, not yet written into the Wiki or the group register, because its OCR
> is noisy on the pricing lines and proceeding is the owner's decision, not this KB's to assume.
> Detail in `Wiki/Processes/group-document-numbering-and-filing.md`,
> `Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md` and
> `Outputs/change-log-2026-09-10-v1.3-and-kosmosoft-quote.md`. v9 recorded §1's live-data-sources
> table correcting the policy version to v1.2 after `FC-CR-0001` (this KB's own change request) was
> accepted - detail in `Outputs/change-log-2026-09-09-v1.2-adopted.md`. v8 recorded §1's
> live-data-sources table gaining the MSEM court case's remaining 8 local documents
> (`FCD0000015`-`FCD0000023`, minus `FCD0000018` which was already `FC0000001`), registered as
> `FC0000002`-`FC0000009`, at the owner's explicit instruction. Detail in
> `Wiki/Processes/group-document-numbering-and-filing.md`,
> `Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md`,
> `Outputs/change-log-2026-09-09-msem-case-documents-registered.md` and
> `Outputs/change-log-2026-09-09-v1.2-adopted.md`. v7 recorded §1's live-data-sources table gaining
> this KB's **first real registration** in the group Document Register - `FC0000001`, the MSEM UK
> Ltd v Fishbone Construction Ltd claim form (County Court claim 019JE538), already local as
> `FCD0000018`. v6 changed one word, confirming write access to that register with a scripted
> add-then-delete test row. v5 added the table row in the first place, adopting the Fishbone
> Group's cross-company **Document Register** policy (v1.1) at the owner's instruction after its
> policy notice was found sitting in `Raw/`, including a naming collision to watch for against the
> existing local `FCD`/`FCT` numbering. v4 superseded v3 of 2026-09-05, which added the **Assets**
> wiki category and `Raw/Vehicles/`, for the owner's three company vehicles (one confirmed so far),
> and recorded that v3 itself had been edited in place on 2026-09-06 - the operational-update
> banner, the §5 strikethrough and the §7 qualification below were added directly to the live file,
> without archive-then-recreate and without a version bump. The edit was traced, read in full
> alongside the Wiki article it points at, and found to be genuine, careful work (a Construction
> Smartsheet email-intake pipeline, properly sourced) - not reverted. But the file that states
> archive-then-recreate as a rule should not itself be the one place the rule was skipped, so it
> was noted (retract in place, don't delete - now the house rules document's §7 rule 2) rather than
> silently absorbed. v3 superseded v2, whose §7 listed "why did Macdonald Joinery stop paying?" as
> the first open question, answered that evening. v2 superseded v1, whose §7 said the wiki was
> "almost empty" four hours before twelve articles were built.
> Modelled on the live `CLAUDE.md` of the `Fishbone Commercial Properties Ltd - Knowledge Base`.
> `README.md` is a short pointer to this file. Where the two differ, this file wins.

> **Operational update, 2026-09-06:** The owner authorised a separate Construction Smartsheet
> workspace and the housekeeping process, then restricted it to **info@fishboneconstruction.co.uk
> only**. Minda's separate mailbox is excluded. The owner also waived all mirror requirements;
> historical mirror instructions below do not apply. Read
> [Email intake, document register and tasks](Wiki/Processes/email-to-tasks.md) for the live sheet
> IDs, numbering, ownership, task-write/closure authority and safe archive procedure. Daily intake
> is scheduled at 07:00 local time (construction-info-inbox); the first unattended run is not yet
> verified. The historical no-automation statements below are superseded for this routine only.

This file gives Claude the context it needs to work in this knowledge base without re-explaining
the setup each session: what this KB is for (§0), where the database lives and what's
company-specific about it (§1), how new items are processed here (§2), what runs automatically
(§3, nothing yet beyond the info-mailbox intake), the governance additions specific to this
company (§4), and a standing snapshot of the company with its open questions (§5). Conventions
shared with every other Fishbone company KB - the folder pattern, archive-then-recreate, document
numbering, Wiki article discipline, the change-log file convention, the shared governance
baseline, and how to maintain a standing control file - are **not restated here**; they live in
`Wiki/Process-Fishbone-Systems-House-Rules.md` (v1.3) in the Fishbone Group's Wiki folder. Read
that document once, then this one for what's specific to Fishbone Construction Ltd.

---

## 0. Start every session here

**Before doing anything else, read the newest change-log entries in `Outputs/`** per the shared
change-log convention (house rules §5), then scan `Outputs/kb-registers.md`'s `Processed items`
table for rows still `pending` or `partial`. This applies to every kind of session, not only
formal Raw processing - another session may already have investigated the same thing.

**For what is actually known about the company, start at `Wiki/index.md`**, not the change log.
Since 2026-09-05 the wiki carries the substance; change-log entries record what happened in a
session and are never revised.

**What this knowledge base is for.** It is not a standalone archive. The owner's instruction of
2026-09-04 was: *"this KB is collection of real time data, processing it, document it and pass to
Fishbone Group KB."* This is a **pipeline node**. Raw operational data (bank statements, invoices,
Smartsheet rows) arrives here, is processed and documented, and the result is meant to feed the
parent Fishbone Group knowledge base. Work here should be written so it can be handed upward:
sourced, dated, and free of conclusions that only make sense inside this file.

**Before drawing any conclusion about a counterparty name, check the sister knowledge bases.**
There are at least three others on this Drive - `Fishbone Properties Ltd - Knowledge Base`,
`Fishbone Commercial Properties Ltd - Knowledge Base`, and the group `Loans` database - and facts
about related parties live in them. This is not advice. On 2026-09-04 a whole analysis was built
on the belief that "Fishbone Drylining" credits were income from a sister company. They were this
company drawing down its own lending facility under its former name, and the group Loans wiki had
said so on 21 August. The Loans folder had not been searched.

---

## 1. Database structure

### Where it lives

- **Primary copy: Google Drive**, `My Drive / Fishbone Construction Ltd - Knowledge Base` (folder
  id `13IQdim0JhKmoQvJBmJmnMhreJqg55xTr`). Source of truth.
- **Mirror: git repository** `minda-ui/Fishbone-Construction-Ltd`, branch
  `claude/fishbone-construction-5uqgot`. Synced from Drive, never the other way. Sensitive Raw
  files (bank statements, invoices) are Drive-only; `.gitignore` blocks `*.csv`, `*.xlsx` and
  `*.pdf`. The mirror carries the archived files' **listing** but not their content - see
  `archive/README.md` in the repo.
- When the two disagree, Drive wins.

### Folders

```
Fishbone Construction Ltd - Knowledge Base/
├── CLAUDE.md        <- this file (standing context)
├── README.md        <- short human-facing pointer to this file
├── Archive/         <- superseded versions of replaced files, each named with its reason
├── Raw/             <- source material exactly as received; never edited; kept permanently
│   ├── Email/                          <- captured message evidence, Construction intake pilot
│   ├── Finance/                        <- HSBC 04212819 statement CSVs
│   ├── FP 2401_131 Goathland Avenue/   <- project invoices, one folder per supplier + INDEX.md
│   └── Vehicles/                       <- one folder per vehicle + INDEX.md; see Wiki/Assets/
├── Wiki/            <- index.md, _templates/, and one article per entity or topic in:
│   │                   Assets/ Customers/ Decisions/ Finance/ Processes/ Projects/ Suppliers/
│   │                   (Contracts/ and People/ are named in index.md but hold nothing yet)
│   └── (five legacy Google Docs still sit at the Wiki root - see index.md, "Unfiled")
└── Outputs/         <- deliverables built from the Wiki, the dated change-log entries,
                        and kb-registers.md (house rules §5)
```

This KB follows the shared four-folder pattern (house rules §1) with one point worth stating
explicitly: **this KB keeps everything in `Raw/` permanently, as an archive**, not as an inbox -
the more common pattern of the two the house rules document describes (§1's note contrasts it
with Fishbone Holdings Ltd, which runs `Raw/` as an inbox instead). Files may be reorganised
*within* Raw into subfolders, as the Goathland invoices were on 2026-09-05, but a folder that is
reorganised gets an `INDEX.md` recording what each file is, because the point of the
reorganisation is to make the folder legible and a move without a record does the opposite.

**Wiki/** categories here: Assets, Contracts, Customers, Decisions, Finance, People, Processes,
Projects, Suppliers. Five legacy Google Docs still sit at the root of `Wiki/` and are listed in
`index.md` under "Unfiled" - see its open questions. **Assets** is for company-owned physical
assets - vehicles so far - kept apart from `Finance/` deliberately: a vehicle article is about the
asset (insurance, MOT, mileage, condition), not about how it was financed, which is the group
Loans database's material and stays there, linked rather than copied. See
`Wiki/Decisions/2026-09-09-assets-category-and-vehicles-workspace.md`.

Replacing any standing control file in this KB (`CLAUDE.md`, `README.md`,
`Outputs/kb-registers.md`, `Wiki/index.md`, a Wiki Google Doc) follows the shared
archive-then-recreate convention (house rules §2); this KB also mirrors both the rename and the
new upload to git.

### Live data sources (override Raw for these datasets)

| Dataset | Live source | Status |
|---|---|---|
| Project budgets and rates | Smartsheet **Сlassifier** (note the Cyrillic С), sheet id `6344783272478596`, workspace "1. General"; and **FP 2401_Budget**, sheet id `8653045758035844`, workspace "3. Project Delivery" | Live. The Classifier is the master rate library across all projects; the Budget is per project. |
| Group lending | The group **Loans** database (separate Drive folder, id `1kW9XA7ADnvVH700XYnFTFbKa3SeNtqip`), its Wiki and its Smartsheet Repayment Plan | Live, and **authoritative over this KB** on any lender or related-party question. Read it before concluding anything about a counterparty. |
| Company financials | QuickBooks Online via the Intuit connector | **Degraded. Bank feed stale since at least 2 September 2026**; Intuit consent expiring. Detail and the known integrity defects: `Wiki/Processes/data-capture-and-accounting-systems.md`. |
| Bank transactions | None live. HSBC CSV exports dropped into `Raw/Finance/` | Snapshots; process as Raw items. Six months processed, 22 Feb to 21 Aug 2026. Next file expected: 22 Aug to 21 Sep. |
| Document capture | Dext | **Failing since 24 August 2026.** Uploads error. Until fixed, invoices arrive by hand. |
| Companies House filings | None live. Company number **07948220** | Late-filing penalties of £375 and £150 charged 20 April 2026, so filing dates are not being met. Check manually. |
| Cross-company document register | Fishbone Group **Document Register** (Smartsheet, sheet id `7352854736144260`), workspace "Fishbone Group - Documents" | **Adopted 2026-09-09, now at policy v1.3** (v1.1 → v1.2 same day after `FC-CR-0001`; v1.2 → v1.3 2026-09-10 after two other companies' change requests). Full scheme: house rules §3, linking to `Wiki/Process-Document-Numbering-and-Filing.md`. This company's prefix is `FC` - distinct from the pre-existing local `FCD`/`FCT` numbering in the Construction Smartsheet workspace, which is fully accounted for and migrated; nothing remains to back-fill. Self-assigned 4-digit property codes don't apply - no property owned. |

When a live source exists, pull it fresh each session and log the sync in the change log even if
nothing changed, so the next session knows how fresh the Wiki is.

---

## 2. Workflow for processing new items

Wiki article conventions (front matter, citation, linking, sensitive-data handling) follow the
shared rules in house rules §4 without exception; this KB cites facts into `Raw/` (kept
permanently, per §1 above). `Wiki/Suppliers/subcontractors.md` is this KB's worked example of the
sensitive-data rule: 65% of subcontract spend goes to named individuals, so the article gives
totals, counts and the limited companies by name, and sends the reader to the Drive-only CSVs for
the rest. `Wiki/Customers/at-uk-interiors.md` is the worked example of writing an honest `draft`
article around an open question rather than guessing.

### 2a. Live sources
1. Check the change log for the last sync of that source.
2. Pull current rows (Smartsheet `get_columns` then `get_sheet_summary`; QuickBooks `company_info`
   then the report tools).
3. Diff against the Wiki; update articles in place, moving old values to "Changes".
4. Cite the live source URL in the article.
5. Log the sync with a timestamp, even if nothing changed.
6. Anomalies are flagged in the article's "Open questions", not fixed by guessing.

### 2b. Raw items
**Detect** (list `Raw/` and its subfolders, diff against the `Processed items` table of
`Outputs/kb-registers.md`), **Register** as `pending` before starting, **Read and classify**
(respecting §2d), **Extract**, **Update the Wiki** with citations and cross-links both ways,
**Check** links and front matter, **Log** (`done` or `partial`), **Outputs only when requested**,
**Commit** one batch per commit to the git mirror.

A Raw item is `done` only when its findings are in a **wiki article**. Findings that exist only in
a change-log entry are `partial`: entries are written once and never revised, so a fact that will
change is in the wrong place. The six Finance CSVs sat at `partial` for that reason until
2026-09-05.

### 2c. Invoices into Classifier and Budget
This project has its own detailed procedure, and it is the one task with a written
session-starter: `Wiki/FP 2401 Goathland Avenue - Actuals Processing Instructions`. Follow it
rather than improvising. Its core rules: never guess a code match, stop and ask; convert units to
the Budget's unit; cite invoice number, date and the calculation in the Notes; confirm each item
before writing to Smartsheet unless told to run a whole batch.

### 2d. Reading limits, learned so far
- **Bank statement CSVs read cleanly**, but the categorisation must be **reconciled against the
  printed running balances** before any figure is quoted. All six statements to 21 August 2026
  reconcile to the penny; that check is what makes the figures usable.
- **Any PDF with side-by-side tables is read as an image, not as extracted text.** In a sister
  Fishbone workspace on 02/09/2026 three side-by-side tables in a bank statement flattened into
  interleaved columns and a real £11,000 payment was missed.
- **Screwfix "Order History" screenshot PDFs have no text layer.** Text extraction returns only
  "Account Details _ Screwfix Website". They must be rasterised and read visually. 40+ of the 68
  Screwfix files in `Raw/FP 2401_131 Goathland Avenue/` are of this kind.
- **Screwfix classic invoices print a gross "Unit Price".** Use the **Net** column, never the
  printed unit price. Screenshot-style order histories state values inclusive of VAT; ex-VAT is
  gross / 1.2, and where a whole-order discount applies each line's share is estimated
  proportionally by list price and **flagged as estimated** in the Budget Notes.
- **Photographed till receipts (B&Q, JT Dove, YESSS) OCR well** through Drive's own image reading,
  including the VAT analysis block. The transaction date sometimes does not survive.

Change-log entries for this KB follow the shared file convention (house rules §5) without
exception. **The old single `Change Log` Google Doc in `Wiki/` is closed**, not deleted - it holds
the four session entries from 25 August to 5 September 2026 and carries a banner saying logging
has moved. Do not append to it.

---

## 3. Automated processes

~~**None are live.**~~ Corrected 2026-09-06: Construction info inbox intake is scheduled; see the
operational update and Wiki process. Everything in the following original table remains a
proposal, in priority order, and each must satisfy §4a below before it is created.

| Proposed routine | Cadence | Would do | Prerequisite |
|---|---|---|---|
| Bank statement processor | Monthly, on the 22nd | Detect a new HSBC CSV in `Raw/Finance/`, categorise it, reconcile against the printed balances, append the month to `Wiki/Finance/` articles, write a change-log entry. | Nothing. The categoriser and its reconciliation already exist as a script; it needs a home in the KB. |
| Data-capture watchdog | Daily | Check that Dext uploads and the QuickBooks bank feed are working, and flag the day they stop rather than the week someone notices. | Nothing. Both are currently broken and nobody was alerted. |
| Lender payment reconciler | Weekly | Reconcile the Funding Circle direct debits (25 to 37 a month) against the group Loans Repayment Plan, and flag a schedule that has changed. | Read access to the group Loans Smartsheet, which exists. |
| Compliance monitor | Monthly | Companies House filing dates, VAT return dates, HMRC Time to Pay instalments, **CIS300 returns**. | A written list of the company's actual filing obligations. There is none. |
| Supplier statement matcher | Monthly | Match `Raw/` invoices to supplier statements and to the bank, per supplier folder. | The supplier folders now exist; supplier statements do not. |

---

## 4. Governance

### 4a. What automation may do unattended, and what needs a human

This KB follows the shared governance baseline in house rules §6 without exception, plus one
addition specific to this company: automation must never **write to the Smartsheet Classifier or
Budget** without confirming the item first, per §2c above - never do so unattended even though the
baseline permits updating Wiki articles and standing Outputs files unattended.

If a routine's prompt ever conflicts with this list, this section (and house rules §6) wins.

### 4b. Data access
- **Not yet checked for this knowledge base.** The sister KBs both ran an explicit access review;
  this one has not. Until it is done, do not assume the folder is owner-only. A quarterly sweep is
  proposed in §3.
- Bank statements and invoices stay Drive-only and are never copied into git.
- Subcontractor invoices carry individuals' names and payment details. Treat subcontractor,
  payroll, lender and director documents as `sensitive: true`. All six `Wiki/Finance/` articles
  and `Wiki/Suppliers/subcontractors.md` are marked so.
- Cross-company facts are **linked** between knowledge bases, never copied, so there is one place
  to correct each fact.

### 4c. Maintaining this file

This KB follows the shared rules for maintaining any standing control file (house rules §7)
without exception. Two incidents specific to this file, kept because they are why those rules
exist here and not just in principle: *rule 1 (check every heading and outbound reference survives
a replacement) produced v2 of this file - v1's §5 said the wiki was almost empty, which stopped
being true four hours later.* *Rule 3 (detailed rule sets live in the Wiki, not the control file)
was breached between 2026-09-05 and 2026-09-09: v3 was edited in place (the operational banner,
old §5 and §7) with no archived predecessor and no version bump - the work behind the edit was
genuine and careful, which is exactly why the process gap could have gone unnoticed indefinitely.
Caught only because a routine edit session diffed the live file's byte size against what it
expected to find.* If a change is worth making to this file, it is worth the thirty seconds
archive-then-recreate costs.

Update §0 to §2 when structure or process changes; §3 must be kept current as routines are
created, changed or retired; §4 is revisited deliberately, not silently rewritten; §5 is refreshed
whenever a Raw item changes the picture. Every replacement of this file goes through
archive-then-recreate and gets a change-log entry.

### 4d. Authorised contributors

Besides this KB's own sessions, **Anna - AI Construction Assistant** (Minda's technical
construction adviser) is authorised to write technical construction reference content here, per
Minda's sanction of 2026-09-22 (Hub AWT-0077). Scope, the bars that stay, and the note that her
edits appear on Drive as the owner's rather than under a separate identity:
`Wiki/Decisions/2026-09-22-anna-construction-adviser-write-access.md`.

---

## 5. Company snapshot and open questions (as of 2026-09-05)

**The Wiki is the authoritative record; start at `Wiki/index.md`.** Since 2026-09-05 it carries
twelve articles built from six months of reconciled bank data. This section is a one-screen
orientation and every claim in it is sourced in an article - go there for the detail and the
citations.

- **Company** 07948220, England and Wales, registered office 6 Beverley Place, Wallsend NE28 7BH.
  Trades from Unit 30-32, Point Pleasant Industrial Estate, Wallsend. Managing director Mindaugas
  Gaudiesius; A Prutkovas also a director. **Renamed from FISHBONE DRYLINING LTD. to FISHBONE
  CONSTRUCTION LTD. on 31 October 2024** - several trade and lending accounts still carry the old
  name, and documents in that name are this company's own.
- **What happened** The only substantial customer, Macdonald Joinery, cut its payments 86% in a
  single month in May 2026 and has paid about £8,000 a month since. **The owner confirmed on
  2026-09-05 that the customer has no projects** - no work to place. Not a dispute, not a lost
  contract, not a withheld payment, ~~so there is nothing to chase or resolve.~~ Qualification
  2026-09-06: the info-mailbox pilot found August work correspondence and invoice FC0236 due
  11 September; receipt requires reconciliation. This does not establish future work. See
  Wiki/Processes/email-to-tasks.md. Whether it is temporary is not known. → `Wiki/Customers/macdonald-joinery.md`
- **The cost base worked** Subcontractors and materials fell from £62,721 a month to £18,647,
  tracking revenue down. Payroll held flat at about £9,100.
  → `Wiki/Suppliers/subcontractors.md`
- **The debt did not** £350,803 of debt service over six months, roughly £42,000-£45,000 a month
  underlying, unmoved by the fall in turnover. → `Wiki/Finance/debt-service.md`
- **Who is paying for it** The six-month shortfall after debt was £497,071. The Funding Circle
  facility supplied none of it - net minus £22,104. £319,460 came from Fishbone Properties Ltd and
  the directors, about £53,000 a month. → `Wiki/Finance/related-party-funding.md`

**Open questions, in priority order.** Each is stated in full, with how to close it, on the
article named.

~~1. Why did Macdonald Joinery stop paying?~~ **Answered 2026-09-05: the customer has no
projects.** Kept visible per house rules §7 rule 2. It was the top question for one day, and
closing it promoted the two below, which had been second and third.

1. **What replaces the revenue?** 80% of third-party receipts came from one customer who now has
   no work, and **no other customer, contract or pipeline is recorded anywhere in this knowledge
   base**. The concentration risk has already materialised. Nothing in `Raw/`, the wiki or
   Smartsheet says what the company expects to invoice after August 2026.
   → `Wiki/Customers/macdonald-joinery.md`, `Wiki/Finance/trading-receipts.md`
2. **Do Fishbone Properties Ltd and the directors know they are funding ~£53,000 a month?** This
   question changed character on 2026-09-05. If that money was being advanced in expectation that
   Macdonald would come back, the basis for it has gone. Also: is the money labelled "Loan
   Payback" the repayment of a debt owed *to* this company, which would invert the intercompany
   balance? → `Wiki/Finance/related-party-funding.md`
3. **Is the HMRC Time to Pay arrangement current or in default?** No payment to HMRC left the
   account between 22 April and 21 August 2026. Both readings produce identical bank statements.
   → `Wiki/Finance/hmrc.md`
4. **Is CIS being operated?** 68 subcontractors, £190,647 over six months, and nothing in this
   knowledge base addresses verification, deduction rates, CIS300 returns or payment over.
   → `Wiki/Suppliers/subcontractors.md`
5. **No contract of any kind is held in `Raw/`** - not a customer contract, subcontract agreement,
   lease or facility agreement. Every financial article describes an arrangement whose written
   terms are unknown. → `Wiki/index.md`, Contracts
6. Is AT UK Interiors a customer or a related party? £25,447 of six-month receipts turns on it.
   → `Wiki/Customers/at-uk-interiors.md`
7. Reconnect the QuickBooks bank feed and fix Dext; explain the £2,866 against £433,119 net income
   disagreement. → `Wiki/Processes/data-capture-and-accounting-systems.md`
8. What is account 24241061, and what is its balance?
   → `Wiki/Finance/hsbc-current-account.md`

---

*Standing context for the Fishbone Construction Ltd knowledge base. Version 12, 2026-09-22,
adding §4d (Anna as an authorised contributor) and correcting the citation of the Fishbone Group's
shared house rules document
(`Wiki/Process-Fishbone-Systems-House-Rules.md`, v1.3) for conventions common to every company KB,
superseding v11 of 2026-09-11, v10 of 2026-09-10, v9 of 2026-09-09, v8, v7, v6, v5 and v4 of that same day, v3 of
2026-09-05 (which was itself edited in place on 2026-09-06 - see the header and §4c), and v2 and
v1 before it. See
`Wiki/Decisions/2026-09-05-kb-skeleton-adopted.md`,
`Wiki/Decisions/2026-09-09-assets-category-and-vehicles-workspace.md`,
`Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md`,
`Wiki/Decisions/2026-09-22-anna-construction-adviser-write-access.md`,
`Outputs/change-log-2026-09-05-kb-skeleton-and-raw-tidy.md`,
`Outputs/change-log-2026-09-05-wiki-from-bank-data.md`,
`Outputs/change-log-2026-09-05-macdonald-answered.md`,
`Outputs/change-log-2026-09-09-vehicle-workspace-created.md`,
`Outputs/change-log-2026-09-09-group-document-numbering-adopted.md`,
`Outputs/change-log-2026-09-09-group-document-numbering-write-access-confirmed.md`,
`Outputs/change-log-2026-09-09-first-group-register-document.md`,
`Outputs/change-log-2026-09-09-msem-case-documents-registered.md`,
`Outputs/change-log-2026-09-09-v1.2-adopted.md` and
`Outputs/change-log-2026-09-10-v1.3-and-kosmosoft-quote.md`.*
