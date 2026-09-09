# Fishbone Construction Ltd - Knowledge Base

> **Status: AUTHORITATIVE. Version 6, 2026-09-09**, superseding v5 of the same day (in
> `Archive/`). One word changed: §1's live-data-sources table now says write access to the
> group Document Register is **confirmed**, not untested - a scripted add-then-delete test row
> proved it, then removed itself; detail in
> `Wiki/Processes/group-document-numbering-and-filing.md` and
> `Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md`. v5 added that table
> row in the first place, adopting the Fishbone Group's cross-company **Document Register**
> policy (v1.1) at the owner's instruction after its policy notice was found sitting in `Raw/`,
> including a naming collision to watch for against the existing local `FCD`/`FCT` numbering.
> v4 superseded v3 of 2026-09-05, which added the **Assets** wiki category and
> `Raw/Vehicles/`, for the owner's three company vehicles (one confirmed so far), and recorded
> that v3 itself had been edited in place on 2026-09-06 - the operational-update banner, the §5
> strikethrough and the §7 qualification below were added directly to the live file, without
> archive-then-recreate and without a version bump. The edit was traced, read in full alongside
> the Wiki article it points at, and found to be genuine, careful work (a Construction
> Smartsheet email-intake pipeline, properly sourced) - not reverted. But the file that states
> archive-then-recreate as a rule should not itself be the one place the rule was skipped, so it
> was noted per §6d rule 2 (retract in place, don't delete) rather than silently absorbed. v3
> superseded v2, whose §7 listed "why did Macdonald Joinery stop paying?" as the first open
> question, answered that evening. v2 superseded v1, whose §7 said the wiki was "almost empty"
> four hours before twelve articles were built.
> Modelled on the live `CLAUDE.md` of the `Fishbone Commercial Properties Ltd - Knowledge Base`.
> The rules in sections 1, 2, 4 and 6d were adopted from that file rather than re-derived,
> because each of them has a real failure behind it and those failures are recorded there. What
> is added here is specific to this company: it trades, it has projects, subcontractors,
> suppliers and lenders, and its knowledge base has a job the other two do not - see section 0.
> `README.md` is a short pointer to this file. Where the two differ, this file wins.

> **Operational update, 2026-09-06:** The owner authorised a separate Construction Smartsheet workspace and the housekeeping process, then restricted it to **info@fishboneconstruction.co.uk only**. Minda's separate mailbox is excluded. The owner also waived all mirror requirements; historical mirror instructions below do not apply. Read [Email intake, document register and tasks](Wiki/Processes/email-to-tasks.md) for the live sheet IDs, numbering, ownership, task-write/closure authority and safe archive procedure. Daily intake is scheduled at 07:00 local time (construction-info-inbox); the first unattended run is not yet verified. The historical no-automation statements below are superseded for this routine only.

This file gives Claude the context it needs to work in this knowledge base without
re-explaining the setup each session: what this KB is for (§0), where the database lives (§1),
how the Wiki is maintained (§2), how new items are processed (§3), how the change log works
(§4), what runs automatically (§5, nothing yet), the governance boundary automation operates
under (§6), and a standing snapshot of the company with its open questions (§7).

---

## 0. Start every session here

**Before doing anything else, read the newest change-log entries in `Outputs/`.** They are
named `change-log-YYYY-MM-DD-<slug>.md`, one per session or run. `Outputs/kb-registers.md`
lists every one of them in order in its `Change-log entries` table - start there rather than
sorting filenames, because entries from the same day sort by slug, not by time of day. Then
scan that same file's `Processed items` table for rows still `pending` or `partial`.

This applies to every kind of session: a one-off question, a drafting request, a Smartsheet
edit, not only formal Raw processing. Another session may already have investigated the same
thing or corrected the same figure.

**For what is actually known about the company, start at `Wiki/index.md`**, not at the change
log. Since 2026-09-05 the wiki carries the substance; change-log entries record what happened
in a session and are never revised.

**What this knowledge base is for.** It is not a standalone archive. The owner's instruction of
2026-09-04 was: *"this KB is collection of real time data, processing it, document it and pass
to Fishbone Group KB."* This is a **pipeline node**. Raw operational data (bank statements,
invoices, Smartsheet rows) arrives here, is processed and documented, and the result is meant
to feed the parent Fishbone Group knowledge base. Work here should be written so it can be
handed upward: sourced, dated, and free of conclusions that only make sense inside this file.

**Before drawing any conclusion about a counterparty name, check the sister knowledge bases.**
There are at least three others on this Drive - `Fishbone Properties Ltd - Knowledge Base`,
`Fishbone Commercial Properties Ltd - Knowledge Base`, and the group `Loans` database - and
facts about related parties live in them. This is not advice. On 2026-09-04 a whole analysis
was built on the belief that "Fishbone Drylining" credits were income from a sister company.
They were this company drawing down its own lending facility under its former name, and the
group Loans wiki had said so on 21 August. The Loans folder had not been searched.

---

## 1. Database structure

### Where it lives

- **Primary copy: Google Drive**, `My Drive / Fishbone Construction Ltd - Knowledge Base`
  (folder id `13IQdim0JhKmoQvJBmJmnMhreJqg55xTr`). Source of truth.
- **Mirror: git repository** `minda-ui/Fishbone-Construction-Ltd`, branch
  `claude/fishbone-construction-5uqgot`. Synced from Drive, never the other way. Sensitive
  Raw files (bank statements, invoices) are Drive-only; `.gitignore` blocks `*.csv`, `*.xlsx`
  and `*.pdf`. The mirror carries the archived files' **listing** but not their content - see
  `archive/README.md` in the repo.
- When the two disagree, Drive wins.

### Folders

```
Fishbone Construction Ltd - Knowledge Base/
├── CLAUDE.md        <- this file (standing context)
├── README.md        <- short human-facing pointer to this file
├── Archive/         <- superseded versions of replaced files, each named with its reason
├── Raw/             <- source material exactly as received; never edited
│   ├── Email/                          <- captured message evidence, Construction intake pilot
│   ├── Finance/                        <- HSBC 04212819 statement CSVs
│   ├── FP 2401_131 Goathland Avenue/   <- project invoices, one folder per supplier + INDEX.md
│   └── Vehicles/                       <- one folder per vehicle + INDEX.md; see Wiki/Assets/
├── Wiki/            <- index.md, _templates/, and one article per entity or topic in:
│   │                   Assets/ Customers/ Decisions/ Finance/ Processes/ Projects/ Suppliers/
│   │                   (Contracts/ and People/ are named in index.md but hold nothing yet)
│   └── (five legacy Google Docs still sit at the Wiki root - see index.md, "Unfiled")
└── Outputs/         <- deliverables built from the Wiki, the dated change-log entries,
                        and kb-registers.md (§4)
```

**Raw/** is immutable. Corrections arrive as new files. Verbal information from the owner or a
director is written up as `Raw/YYYY-MM-DD_owner-note_<subject>.md`, statement separated from
commentary, so the Wiki can cite it. **Nothing is deleted or moved out of Raw.** Files may be
reorganised *within* Raw into subfolders, as the Goathland invoices were on 2026-09-05, but a
folder that is reorganised gets an `INDEX.md` recording what each file is, because the point of
the reorganisation is to make the folder legible and a move without a record does the opposite.

**Wiki/** holds Markdown articles with the front matter in `Wiki/_templates/article.md`. Every
article is listed in `Wiki/index.md`. Categories: Assets, Contracts, Customers, Decisions,
Finance, People, Processes, Projects, Suppliers. Five legacy Google Docs still sit at the root
of `Wiki/` and are listed in `index.md` under "Unfiled" - see its open questions.

**Assets** is for company-owned physical assets - vehicles so far - kept apart from `Finance/`
deliberately: a vehicle article is about the asset (insurance, MOT, mileage, condition), not
about how it was financed, which is the group Loans database's material and stays there,
linked rather than copied. See `Wiki/Decisions/2026-09-09-assets-category-and-vehicles-workspace.md`.

**Outputs/** are snapshots. Anything worth keeping is written into the Wiki, not left in
Outputs. Standing always-current files are a deliberate exception to the write-once rule:
`Outputs/kb-registers.md` carries current state, so it is replaced rather than appended.

**Archive/** is never edited or deleted. Drive files cannot be edited in place by the tooling,
so every replacement of a standing file - `CLAUDE.md`, `README.md`, `Outputs/kb-registers.md`,
`Wiki/index.md`, a Wiki Google Doc - follows **archive-then-recreate**: rename the old file
`<title> (archived YYYY-MM-DD, superseded by <reason>).md`, move it into `Archive/`, upload the
new file, mirror both to git. **Dated change-log entries are never replaced at all** (§4), so
they never enter this cycle.

Two rules on archive hygiene, inherited:
- **Keep the original extension at the end of the archived title** (`… <reason>).md`). Drive
  titles and their git mirrors must match character for character, or the two `Archive/`
  folders cannot be compared by name.
- **The archive suffix must name a specific reason**, not "superseded". Done consistently, the
  `Archive/` listing becomes this file's own changelog, readable without opening anything.

### Live data sources (override Raw for these datasets)

| Dataset | Live source | Status |
|---|---|---|
| Project budgets and rates | Smartsheet **Сlassifier** (note the Cyrillic С), sheet id `6344783272478596`, workspace "1. General"; and **FP 2401_Budget**, sheet id `8653045758035844`, workspace "3. Project Delivery" | Live. The Classifier is the master rate library across all projects; the Budget is per project. |
| Group lending | The group **Loans** database (separate Drive folder, id `1kW9XA7ADnvVH700XYnFTFbKa3SeNtqip`), its Wiki and its Smartsheet Repayment Plan | Live, and **authoritative over this KB** on any lender or related-party question. Read it before concluding anything about a counterparty. |
| Company financials | QuickBooks Online via the Intuit connector | **Degraded. Bank feed stale since at least 2 September 2026**; Intuit consent expiring. Detail and the known integrity defects: `Wiki/Processes/data-capture-and-accounting-systems.md`. |
| Bank transactions | None live. HSBC CSV exports dropped into `Raw/Finance/` | Snapshots; process as Raw items. Six months processed, 22 Feb to 21 Aug 2026. Next file expected: 22 Aug to 21 Sep. |
| Document capture | Dext | **Failing since 24 August 2026.** Uploads error. Until fixed, invoices arrive by hand. |
| Companies House filings | None live. Company number **07948220** | Late-filing penalties of £375 and £150 charged 20 April 2026, so filing dates are not being met. Check manually. |
| Cross-company document register | Fishbone Group **Document Register** (Smartsheet, sheet id `7352854736144260`), workspace "Fishbone Group - Documents" | **Adopted 2026-09-09 (policy v1.1).** This company's prefix is `FC` - distinct from the pre-existing local `FCD`/`FCT` numbering in the Construction Smartsheet workspace, which keeps working for existing entries; new qualifying documents route to the group register from here. Read and write access both confirmed 2026-09-09. Rules: `Wiki/Processes/group-document-numbering-and-filing.md`. |

When a live source exists, pull it fresh each session and log the sync in the change log even
if nothing changed, so the next session knows how fresh the Wiki is.

---

## 2. Wiki maintenance guidelines

- One subject per article. Front matter mandatory (`title, category, status, sensitive, created,
  updated, sources, related`). Status `draft | active | superseded | archived`.
- Every fact from a source is cited with a relative link into `Raw/` (or the live source URL)
  and a location inside it. Unsupported statements are marked `(unverified)`.
- Links between articles are relative, kebab-case, bidirectional (`related:` both ends).
  Link the first mention. Never link to `Outputs/`.
- If a linked article does not exist yet, create a stub in `draft` status with an "Open
  questions" section rather than leaving a dead link.
- **Sensitive personal data is never quoted into the Wiki**; point to the Raw file and set
  `sensitive: true`. `Wiki/Suppliers/subcontractors.md` is the worked example: 65% of
  subcontract spend goes to named individuals, so the article gives totals, counts and the
  limited companies by name, and sends the reader to the Drive-only CSVs for the rest.
- Keep a "Changes" section at the foot of every article naming the change-log entry that drove
  each edit. Bump `updated` on every edit.
- **An article that records an unresolved question is worth more than one that guesses.** Write
  it as `draft`, state what turns on the answer, and say how to close it.
  `Wiki/Customers/at-uk-interiors.md` is the example.
- **Claims in this file are re-verified, not repeated.** If a task is about to act on a claim
  here that it can cheaply re-check against the live source, do so first.

---

## 3. Workflow for processing new items

### 3a. Live sources
1. Check the change log for the last sync of that source.
2. Pull current rows (Smartsheet `get_columns` then `get_sheet_summary`; QuickBooks
   `company_info` then the report tools).
3. Diff against the Wiki; update articles in place, moving old values to "Changes".
4. Cite the live source URL in the article.
5. Log the sync with a timestamp, even if nothing changed.
6. Anomalies are flagged in the article's "Open questions", not fixed by guessing.

### 3b. Raw items
**Detect** (list `Raw/` and its subfolders, diff against the `Processed items` table of
`Outputs/kb-registers.md`), **Register** as `pending` before starting, **Read and classify**
(respecting §3d), **Extract**, **Update the Wiki** with citations and cross-links both ways,
**Check** links and front matter, **Log** (`done` or `partial`), **Outputs only when
requested**, **Commit** one batch per commit to the git mirror.

A Raw item is `done` only when its findings are in a **wiki article**. Findings that exist only
in a change-log entry are `partial`: entries are written once and never revised, so a fact that
will change is in the wrong place. The six Finance CSVs sat at `partial` for that reason until
2026-09-05.

### 3c. Invoices into Classifier and Budget
This project has its own detailed procedure, and it is the one task with a written
session-starter: `Wiki/FP 2401 Goathland Avenue - Actuals Processing Instructions`. Follow it
rather than improvising. Its core rules: never guess a code match, stop and ask; convert units
to the Budget's unit; cite invoice number, date and the calculation in the Notes; confirm each
item before writing to Smartsheet unless told to run a whole batch.

### 3d. Reading limits, learned so far
- **Bank statement CSVs read cleanly**, but the categorisation must be **reconciled against
  the printed running balances** before any figure is quoted. All six statements to 21 August
  2026 reconcile to the penny; that check is what makes the figures usable.
- **Any PDF with side-by-side tables is read as an image, not as extracted text.** In a sister
  Fishbone workspace on 02/09/2026 three side-by-side tables in a bank statement flattened into
  interleaved columns and a real £11,000 payment was missed.
- **Screwfix "Order History" screenshot PDFs have no text layer.** Text extraction returns only
  "Account Details _ Screwfix Website". They must be rasterised and read visually. 40+ of the
  68 Screwfix files in `Raw/FP 2401_131 Goathland Avenue/` are of this kind.
- **Screwfix classic invoices print a gross "Unit Price".** Use the **Net** column, never the
  printed unit price. Screenshot-style order histories state values inclusive of VAT; ex-VAT is
  gross / 1.2, and where a whole-order discount applies each line's share is estimated
  proportionally by list price and **flagged as estimated** in the Budget Notes.
- **Photographed till receipts (B&Q, JT Dove, YESSS) OCR well** through Drive's own image
  reading, including the VAT analysis block. The transaction date sometimes does not survive.

---

## 4. Change log

**One file per session or run**, in `Outputs/`, named `change-log-YYYY-MM-DD-<slug>.md`. A
second run on the same day takes its own slug; a follow-up to an entry already written takes
`-addendum`, then `-addendum-2`. Adopted 2026-09-05, matching the two sister knowledge bases.

**An entry is written once and never edited.** That is the whole point of the design: no
archive-then-recreate, no timestamped snapshots, no rewriting a large file to add a paragraph.
If something in a past entry turns out to be wrong, **write a new entry that references it** -
never go back and change the old one. The reader must be able to see what was believed at the
time.

**The old single `Change Log` Google Doc in `Wiki/` is closed**, not deleted. It holds the four
session entries from 25 August to 5 September 2026 and remains the record of that period. It
carries a banner saying logging has moved. Do not append to it.

**What does not go in a dated entry** lives in `Outputs/kb-registers.md`, a standing file
replaced by archive-then-recreate when a row is added:

| Table | Answers |
|---|---|
| `Change-log entries` | Every entry file, newest first. The chronology; filename sort does not give it |
| `Processed items` | What has been taken out of `Raw/`, and its status. §3b's Detect step diffs `Raw/` against this table |
| `Wiki structure changes` | When articles and categories were created, renamed or repointed, and why |
| `Outputs produced` | Deliverables built from the Wiki, and who asked for them |

---

## 5. Automated processes

~~**None are live.**~~ Corrected 2026-09-06: Construction info inbox intake is scheduled; see the
operational update and Wiki process. Everything in the following original table remains a
proposal, in priority order, and each must satisfy §6a before it is created.

| Proposed routine | Cadence | Would do | Prerequisite |
|---|---|---|---|
| Bank statement processor | Monthly, on the 22nd | Detect a new HSBC CSV in `Raw/Finance/`, categorise it, reconcile against the printed balances, append the month to `Wiki/Finance/` articles, write a change-log entry. | Nothing. The categoriser and its reconciliation already exist as a script; it needs a home in the KB. |
| Data-capture watchdog | Daily | Check that Dext uploads and the QuickBooks bank feed are working, and flag the day they stop rather than the week someone notices. | Nothing. Both are currently broken and nobody was alerted. |
| Lender payment reconciler | Weekly | Reconcile the Funding Circle direct debits (25 to 37 a month) against the group Loans Repayment Plan, and flag a schedule that has changed. | Read access to the group Loans Smartsheet, which exists. |
| Compliance monitor | Monthly | Companies House filing dates, VAT return dates, HMRC Time to Pay instalments, **CIS300 returns**. | A written list of the company's actual filing obligations. There is none. |
| Supplier statement matcher | Monthly | Match `Raw/` invoices to supplier statements and to the bank, per supplier folder. | The supplier folders now exist; supplier statements do not. |

---

## 6. Governance

### 6a. What automation may do unattended, and what needs a human

**May, without asking:** read Drive, Smartsheet and QuickBooks; file documents into `Raw/`;
reorganise `Raw/` into subfolders with an `INDEX.md`; create or update Wiki articles per §2 and
§3; rewrite standing Outputs files; write new change-log entries; flag anomalies and risks
inside Drive files.

**Must never do without an explicit human decision:** send, reply to or forward external email
(drafting for a human is fine); file anything with Companies House or HMRC; make or authorise a
payment, or commit the company to an obligation; **write to the Smartsheet Classifier or
Budget** without confirming the item, per §3c; contact a lender, HMRC, a subcontractor, a
supplier or a customer; change Drive or Smartsheet sharing; delete anything from `Raw/`;
resolve an ambiguous or contradictory finding by guessing.

If a routine's prompt ever conflicts with this list, this section wins.

### 6b. Data access
- **Not yet checked for this knowledge base.** The sister KBs both ran an explicit access
  review; this one has not. Until it is done, do not assume the folder is owner-only. A
  quarterly sweep is proposed in §5.
- Bank statements and invoices stay Drive-only and are never copied into git.
- Subcontractor invoices carry individuals' names and payment details. Treat subcontractor,
  payroll, lender and director documents as `sensitive: true`. All six `Wiki/Finance/` articles
  and `Wiki/Suppliers/subcontractors.md` are marked so.
- Cross-company facts are **linked** between knowledge bases, never copied, so there is one
  place to correct each fact.

### 6c. Revisiting this document
Update §0 to §3 when structure or process changes; §4 is maintained continuously; §5 must be
kept current as routines are created, changed or retired; §6 is revisited deliberately, not
silently rewritten; §7 is refreshed whenever a Raw item changes the picture. Every replacement
of this file goes through archive-then-recreate and gets a change-log entry.

### 6d. Maintaining this file

1. **Check the section list survives a replacement, and check outbound references too.** Before
   writing a new version, list this file's headings; after writing it, confirm every heading is
   still present and every `§` cross-reference resolves. Then open every file this document
   points at and confirm it still contains what is claimed. A reference out of this file is
   exactly as breakable as one inside it. *This rule produced v2: §7 of v1 said the wiki was
   almost empty, which stopped being true four hours later.*
2. **Retract in place; never delete a claim that was believed.** A statement here that turns out
   to be wrong gets struck through, dated and corrected, not removed. A sister file carried a
   fabricated "known bug" for 17 days, propagated into other documents, because nobody
   re-checked it.
3. **A number inherited from an earlier session is not evidence. Count it, or do not state it.**
   *Breached on 2026-09-05 in `Wiki/index.md`, which claimed four archived copies of itself
   where three existed. The correction created the fourth.*
4. **Detailed rule sets live in the Wiki, not here.** When a rule needs more than a short
   paragraph, put it in a `Wiki/Processes/` article and link to it.
5. **Archive-then-recreate applies to this file too, with no exceptions for a well-intentioned
   edit.** *Breached between 2026-09-05 and 2026-09-09: v3 was edited in place (the operational
   banner, §5 and §7) with no archived predecessor and no version bump - the work behind the
   edit was genuine and careful, which is exactly why the process gap could have gone unnoticed
   indefinitely. Caught only because a routine edit session diffed the live file's byte size
   against what it expected to find.* If a change is worth making to this file, it is worth
   the thirty seconds archive-then-recreate costs.

---

## 7. Company snapshot and open questions (as of 2026-09-05)

**The Wiki is the authoritative record; start at `Wiki/index.md`.** Since 2026-09-05 it carries
twelve articles built from six months of reconciled bank data. This section is a one-screen
orientation and every claim in it is sourced in an article - go there for the detail and the
citations.

- **Company** 07948220, England and Wales, registered office 6 Beverley Place, Wallsend
  NE28 7BH. Trades from Unit 30-32, Point Pleasant Industrial Estate, Wallsend. Managing
  director Mindaugas Gaudiesius; A Prutkovas also a director. **Renamed from FISHBONE DRYLINING
  LTD. to FISHBONE CONSTRUCTION LTD. on 31 October 2024** - several trade and lending accounts
  still carry the old name, and documents in that name are this company's own.
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
  facility supplied none of it - net minus £22,104. £319,460 came from Fishbone Properties Ltd
  and the directors, about £53,000 a month. → `Wiki/Finance/related-party-funding.md`

**Open questions, in priority order.** Each is stated in full, with how to close it, on the
article named.

~~1. Why did Macdonald Joinery stop paying?~~ **Answered 2026-09-05: the customer has no
projects.** Kept visible per §6d rule 2. It was the top question for one day, and closing it
promoted the two below, which had been second and third.

1. **What replaces the revenue?** 80% of third-party receipts came from one customer who now has
   no work, and **no other customer, contract or pipeline is recorded anywhere in this knowledge
   base**. The concentration risk has already materialised. Nothing in `Raw/`, the wiki or
   Smartsheet says what the company expects to invoice after August 2026.
   → `Wiki/Customers/macdonald-joinery.md`, `Wiki/Finance/trading-receipts.md`
2. **Do Fishbone Properties Ltd and the directors know they are funding ~£53,000 a month?** This
   question changed character on 2026-09-05. If that money was being advanced in expectation
   that Macdonald would come back, the basis for it has gone. Also: is the money labelled "Loan
   Payback" the repayment of a debt owed *to* this company, which would invert the intercompany
   balance? → `Wiki/Finance/related-party-funding.md`
3. **Is the HMRC Time to Pay arrangement current or in default?** No payment to HMRC left the
   account between 22 April and 21 August 2026. Both readings produce identical bank statements.
   → `Wiki/Finance/hmrc.md`
4. **Is CIS being operated?** 68 subcontractors, £190,647 over six months, and nothing in this
   knowledge base addresses verification, deduction rates, CIS300 returns or payment over.
   → `Wiki/Suppliers/subcontractors.md`
5. **No contract of any kind is held in `Raw/`** - not a customer contract, subcontract
   agreement, lease or facility agreement. Every financial article describes an arrangement
   whose written terms are unknown. → `Wiki/index.md`, Contracts
6. Is AT UK Interiors a customer or a related party? £25,447 of six-month receipts turns on it.
   → `Wiki/Customers/at-uk-interiors.md`
7. Reconnect the QuickBooks bank feed and fix Dext; explain the £2,866 against £433,119 net
   income disagreement. → `Wiki/Processes/data-capture-and-accounting-systems.md`
8. What is account 24241061, and what is its balance?
   → `Wiki/Finance/hsbc-current-account.md`

---

*Standing context for the Fishbone Construction Ltd knowledge base. Version 6, 2026-09-09,
superseding v5 of the same day, v4 of the same day, v3 of 2026-09-05 (which was itself edited
in place on 2026-09-06 - see the header and §6d rule 5), and v2 and v1 before it. See
`Wiki/Decisions/2026-09-05-kb-skeleton-adopted.md`,
`Wiki/Decisions/2026-09-09-assets-category-and-vehicles-workspace.md`,
`Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md`,
`Outputs/change-log-2026-09-05-kb-skeleton-and-raw-tidy.md`,
`Outputs/change-log-2026-09-05-wiki-from-bank-data.md`,
`Outputs/change-log-2026-09-05-macdonald-answered.md`,
`Outputs/change-log-2026-09-09-vehicle-workspace-created.md`,
`Outputs/change-log-2026-09-09-group-document-numbering-adopted.md` and
`Outputs/change-log-2026-09-09-group-document-numbering-write-access-confirmed.md`.*
