# Change Log

> **Mirror of:** [Wiki/Change Log](https://docs.google.com/document/d/1yaATUPhHuuXOvJ1oi-DLi-gWn1ykTXoYXMhntgOjntc/edit) (Google Drive)
> Drive is the working copy. See [README](../README.md) before editing here.
> **CLOSED 2026-09-05 — do not add entries. See the foot of this file.**

**Purpose:** record every processing session against the Classifier database (rows
added/updated, Raw files processed, Wiki articles touched) so a new session has full
context without re-deriving it. Add a new dated entry per session — **do not overwrite
prior entries.**

**Entry format:**

```
[YYYY-MM-DD] — Summary
  Raw processed: <file(s) or "none">
  Classifier changes: <rows added / rows updated / "none">
  Budget changes: <rows added / rows updated / "none">
  Wiki changes: <articles created or updated / "none">
  Notes: <anything the next session should know>
```

---

## [2026-08-25] — Workspace set up

- **Raw processed:** none
- **Classifier changes:** none (existing Сlassifier sheet reviewed and documented, not
  modified)
- **Wiki changes:** Created "Database Structure", "Wiki Maintenance Guidelines",
  "Processing Workflow", "Change Log" (this file)
- **Notes:** Google Drive folder "Fishbone Construction ltd" created with Raw / Wiki /
  Outputs subfolders.

---

## [2026-08-25] — FP 2401_131 Goathland Avenue: first invoice batch (9 files)

- **Raw processed:** 9 invoices (Galaxy Insulation x7, J P McDougall/Dulux x1, JT Dove x1
  out-of-scope, trashed).
- **Classifier changes:** 4 new lines (M15-035/036/037, M14-020).
- **Budget changes:** Actuals for M15-018, M15-027, M15-033, M18-001 (both rows, 50/50
  split), M18-002 (both rows, 50/50 split), plus actuals-only rows for the 4 new codes.
- **Wiki changes:** Created "FP 2401 Goathland Avenue - Actuals Processing Instructions"
  (copy-paste session-starter).

---

## [2026-08-25] — FP 2401_131 Goathland Avenue: large invoice batch (60+ files) — COMPLETE

**Raw processed:** Full batch of Screwfix/Plumbfix, JT Dove, National Plastics, Lilley
Tile, YESSS Electrical, Consumer Unit World, B&Q Trade Point, and further Screwfix
Order-History PDFs (~50 files total this session). One JT Dove invoice trashed earlier
(fence posts, wrong project). One Screwfix order (K8/Fc2518, No Nonsense PostFix
Concrete) confirmed as legitimate spend under a second director's card (Andrejus
Prutkovas) — same project, different reference code "Fc2518".

Two Screwfix orders (A26535801768 FloPlast Strap Boss £10.78, A26536426419 McAlpine
P-Trap £8.34) carried reference "FC2522" — owner confirmed this is a DIFFERENT PROJECT.
Both files trashed from this project's Raw folder (not processed into Budget/Classifier).

**Classifier changes:** ~40 new material/fitting lines added across M13, M14, M15, M16,
M17, M18 sections — plumbing fittings (solder-ring vs push-fit kept as distinct codes per
owner's instruction), electrical fittings/cable, bathroom fixtures, ducting/extractor
components, fixings (multiple screw/washer sizes), sealants/adhesives. Full code list:
M13-005/006, M14-021 to M14-025, M15-038/039, M16-027 to M16-069 (with some gaps),
M17-023 to M17-032, M18-007/008. See Classifier sheet directly for full detail.

**Budget changes:**

- Accumulated/updated existing-code actuals: M16-009 (50 pcs total), M16-012 (200 pcs
  total), M16-005 TRVs, M16-001 Boiler, M16-014, M17-007, M17-018, M17-019, M19-009 (both
  duplicate rows, 50/50 split), M5-005 Postcrete, M15-012 CLS timber, M15-036 Angle Bead,
  M20-010 Stair Nosings, M13-004 Architraves.
- New actuals-only rows added for all ~40 new Classifier codes above, plus 3
  existing-Classifier-but-not-yet-in-Budget codes: M17-001 (6242Y cable), M17-011 (dry
  lining box), M17-017 (3-gang light switch).

A fabricated entry was briefly written to M17-012 (13A 2-Gang Socket) in error, not
backed by any real invoice — caught and reverted to blank before session end. No bad data
remains in the sheet for this code.

**Rate methodology used throughout:**

- JT Dove invoices show ex-VAT prices directly in their line-item columns — verified
  against printed Goods/VAT totals.
- Screwfix/Plumbfix classic invoices (format "Qty | Unit Price | Sub | Discount | Value |
  Gross | Net | VAT") — used the Net column, NOT the printed "Unit Price" (which is
  gross/inc-VAT).
- Screwfix "Order History" screenshot-style PDFs (no text layer, required
  download+rasterize+visual read) explicitly state "all values displayed inclusive of
  VAT" — ex-VAT was computed as gross/1.2. For multi-item orders with a whole-order
  discount code, each line's ex-VAT share was estimated proportionally by list price,
  noted as "(proportionally estimated w/ discount)" in each row's Notes.
- Some B&Q Trade Point mixed-basket receipts required the same proportional-list-price
  estimation, noted as "(proportionally estimated)".

**Wiki changes:** none this session.

**Notes for next session:**

- This batch is COMPLETE — Raw folder should now only contain files processed above (the
  two FC2522 files have been removed). Check for any newly added files before starting.
- Solder-ring vs push-fit fitting distinction (M16-009/M16-014 vs M16-036/037) is now an
  established convention — apply consistently to any future plumbing fitting invoices.
- Several rates were "proportionally estimated" rather than taken from an itemised,
  undiscounted line — flagged in each affected row's Notes for future audit if needed.
- The Budget sheet is now very large (~380+ rows) — consider whether a periodic
  cleanup/audit pass is worthwhile once this project nears completion.

## [2026-09-05] — Bank data processed; company identity correction; solvency and cash analysis

Covers work carried out 2 to 5 September 2026. No invoice processing and no Smartsheet
writes were made in this period.

**Raw processed:**

- `Raw/Finance` — three HSBC account 04212819 statement CSVs (20260621, 20260721,
  20260821), covering 22 May to 21 August 2026. Every transaction categorised, and the
  categorisation reconciled against the printed statement balances so nothing was missed.
- `Raw/application-pdf.pdf` — Companies House certificate of incorporation on change of
  name, company 07948220. Read and acted on; see finding 1.
- **Still unprocessed:** the remaining three Finance CSVs (20260321, 20260421, 20260521),
  covering 22 February to 21 May 2026.

**Classifier changes:** none.

**Budget changes:** none.

**Wiki changes:** none in Drive. Separately, the five Wiki articles were mirrored into this
repository on 2026-09-02. Drive remains the working copy; this repo is a mirror and must be
updated in the same session as any Drive edit.

### Findings

**1. "Fishbone Drylining" credits are this company paying itself, not sales.**
Companies House confirms company 07948220 changed its name from FISHBONE DRYLINING LTD. to
FISHBONE CONSTRUCTION LTD. on 31 October 2024. Bank credits described as "Fishbone Drylining
FC2603 / FC2505 / FC2522 / FC2605 / FLEXIPAY" are therefore not receipts from a related
company — they are this company drawing down its own Funding Circle FlexiPay facility, still
held under the former name, and paying the money into its own account. That is £28,067 a
month on the three-month average. This was already documented in the group Loans database
Wiki on 21 August 2026; it was missed here because the Loans folder was not searched at the
outset. **Lesson:** check the group Loans database and the other entity knowledge bases
before drawing conclusions about any counterparty name.

**2. Genuine trading receipts are £16,855 a month**, not the £44,921 a first reading of the
statements suggests. Third-party customers £12,355 a month (Macdonald Joinery is the only
substantial payer; the one-off Formbuild receipt of £10,140 on 31 July is excluded from the
run rate), plus Fishbone Properties £4,500 a month. Everything else classified as a receipt
on first pass was own borrowing.

**3. Actual debt service is approximately £43,307 a month.** Funding Circle alone took
£31,895 (June), £38,368 (July) and £34,990 (August) — an average of £35,084 a month across
between 27 and 37 separate direct debits. The remainder is Nucleus £1,994, LendingCrowd
£2,388, Haydock £1,210, HSBC £518, MotoNovo £460, SSAS standing orders £434, Tower Leasing
£373 and director loans £846.

*On the Payment Calendar:* it covers the twelve fixed-schedule facilities and correctly
excludes the revolving FlexiPay books, which the Loans database tracks separately as Book 1
and Book 2. The calendar is not defective. The gap is that no single figure anywhere
consolidates the two, so a reader of the calendar alone understates cash leaving the company
by roughly £18,700 a month.

**4. Answer to the open question on Loans database Book 1.** Book 1 asked, on 21 August,
whether its persistently negative net cash movement reflected normal draw-timing or a
widening structural funding gap. **It is structural.** Over June to August the facility drew
£28,067 a month and repaid £35,084 a month — net −£7,017 a month. Book 1's own lifetime
figure agrees at −£125,908. The facility is amortising, so the cash it supplies falls every
month while the repayments it demands do not.

**5. HMRC is being paid, but with borrowed money.** An earlier reading in this session found
no HMRC payment on three months of statements and wrongly concluded PAYE was going unpaid.
The Loans database Book 1 records £54,258.57 paid directly to HMRC under a Time to Pay
arrangement funded by FlexiPay. The money moves from lender to HMRC without passing through
the current account, which is why it is invisible on the statements. The substance is that an
interest-free HMRC arrangement has been converted into fee-bearing debt at an overall rate of
8.53%. Worth asking HMRC whether it would extend Time to Pay directly instead.

**6. The data collection layer is currently down.** Dext document uploads have been failing
since 24 August. The QuickBooks bank feed has not updated — the HSBC 2819 balance read
exactly £18,592.62 on both 2 and 4 September, and the Intuit consent is expiring. Every
figure in this entry therefore comes from manually exported CSVs, not from a live feed.
Reconnecting the bank feed needs an HSBC login and cannot be done without the owner.

**7. Data integrity items outstanding.**

- QuickBooks balance sheet reports net income of £2,866 at 2 September where the P&L for the
  same date reports a loss of £433,119.
- A/P aging totals £57,034 against £52,222 in the balance sheet — a difference of £4,812.
- The A/R aging summary displays a headline of £106,968 which double-counts subtotal rows;
  the correct figure is £55,656 and ties exactly to the balance sheet.
- Sebastian Pabis appears twice across the group records: £50,506 owed by this company per
  QuickBooks A/P, and separately a £35,000 related-party loan to Fishbone Properties Ltd per
  the Loans database, on which no payment has ever been made. Either two distinct exposures
  of about £85,000 combined, or one debt recorded against the wrong entity. Material either
  way.

### Outputs produced — not yet filed

- *Fishbone Construction — Solvency Briefing v2, 4 Sep 2026* (Word). Balance-sheet and
  cash-flow solvency assessment, with the director duties that follow.
- *Fishbone 13-Week Cash Flow Forecast* (Excel). Weeks commencing 7 September to 30 November
  2026, driven from an editable assumptions sheet, with three scenarios and the categorised
  bank data as its evidence base.

Both currently exist only outside this knowledge base. `Outputs/` remains empty. They should
be filed there so they are reproducible and citable.

### Notes for next session

- Three Finance CSVs (February to May 2026) remain unprocessed.
- `Outputs/` is empty and the two deliverables above need filing into it.
- The group Loans database has the same problem: its Wiki cites
  `Outputs/Fishbone_Loan_Repayment_Plan.xlsx` as the live source of truth, but that folder is
  empty and the current workbook (3 September, 99KB) sits in a Downloads folder instead.
  Three superseded copies also sit loose in the Drive root.
- The Loans database Wiki predicted that if a third related-party loan surfaced it would be
  worth asking whether there is a common cause. A third has surfaced: the Smartsheet
  Repayment Plan lists "Sasha (director loan)" alongside Eugene and Sebik.

---

## Where the rest of the log lives

**This document was closed on 5 September 2026 and is no longer appended to.**

Session logging moved to one dated file per run in `Outputs/` on Drive, mirrored here as
[`outputs/`](../outputs/). Files are named `change-log-YYYY-MM-DD-<slug>.md`, written once and
never edited: a correction is a new entry that references the old one.

Start at [`outputs/kb-registers.md`](../outputs/kb-registers.md). Its "Change-log entries" table
lists every entry in order, newest first, including the four historical entries held above. Do
not sort filenames instead — entries from the same day sort by slug, not by time of day.

**Why:** Google Drive has no in-place edit, so every addition to this document meant rewriting
the whole file and archiving the previous copy. It had already been fully rewritten twice on
5 September alone. A sister knowledge base let the same pattern run until its change log reached
44,895 bytes and its `Archive/` held fourteen snapshots of it, some two minutes apart. The cost
was per write, not per byte.

**This document is not deleted.** It remains the record of 25 August to 5 September 2026, and the
four entries above are unchanged. The rules for the new arrangement are in
[`CLAUDE.md`](../CLAUDE.md), section 4.

The entry that used to sit below this point — *Remaining three Finance CSVs processed; six months
of bank data now complete* — was the first written under the new arrangement and now lives at
[`outputs/change-log-2026-09-05-six-month-bank-data.md`](../outputs/change-log-2026-09-05-six-month-bank-data.md).
Nothing was lost in the move.

**See also:** [Processing Workflow](processing-workflow.md) · [Database Structure](database-structure.md) · [Wiki Maintenance Guidelines](wiki-maintenance-guidelines.md)
