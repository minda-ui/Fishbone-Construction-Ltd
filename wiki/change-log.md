# Change Log

> **Mirror of:** [Wiki/Change Log](https://docs.google.com/document/d/1x-LVAcvQRi99NNSa-9zPReMOrqZqIwh9eXwm34al94w/edit) (Google Drive)
> Drive is the working copy. See [README](../README.md) before editing here.

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

## [2026-09-05] — Remaining three Finance CSVs processed; six months of bank data now complete

### Raw processed

- `Raw/Finance` — the three outstanding HSBC account 04212819 statement CSVs (20260321,
  20260421, 20260521), covering 22 February to 21 May 2026. With the three already processed
  on 2 to 5 September, the full six months **22 February to 21 August 2026** are now
  categorised — 1,848 transactions.
- **Reconciliation:** every one of the 160 printed running balances across the six statements
  was recomputed from the opening balance and matched to the penny. Nothing is missing and
  nothing is double-counted.
- Unclassified residue across six months is 21 transactions totalling £1,039 (0.1% of
  turnover). Acceptable; itemised in the working file.

**Classifier changes:** none.
**Budget changes:** none.
**Wiki changes:** this Change Log entry only (plus its Drive original).

### Findings

**8. The customer base has collapsed, and it happened in May.**
Macdonald Joinery, the only substantial third-party customer, paid:

| Statement period | Received |
|---|---:|
| 22 Feb – 21 Mar | £63,832 |
| 22 Mar – 21 Apr | £56,687 |
| 22 Apr – 21 May | £17,712 |
| 22 May – 21 Jun | £7,722 |
| 22 Jun – 21 Jul | £8,372 |
| 22 Jul – 21 Aug | £8,660 |

A fall of 86% from the February–March level, concentrated in a single month. Total third-party
customer receipts fell the same way: £75,322 in the February–March period to £7,749 in
May–June. The £16,855 a month of trading receipts reported in the previous entry is therefore
**not a steady state** — it is the floor after a collapse, and the three months before it
looked like a different company.

> **ACTION REQUIRED:** establish why. Was a Macdonald contract completed, lost, disputed, or
> is payment simply being withheld? Nothing in this knowledge base answers that, and it is the
> single most important open question about the business.

**9. Costs did follow revenue down — the variable cost base works.**
Subcontractors and materials fell from £62,721 (February–March) to £18,647 (June–July),
tracking the revenue fall. Payroll stayed flat at about £9,100 a month. So the trading
operation is not the immediate problem: it scales.

**10. The problem is that debt service did not fall at all.**
Funding Circle took £34,209 a month on average across the six months, in between 25 and 37
separate direct debits per month, and the figure barely moves: £29,015, £36,766, £34,222,
£31,895, £38,368, £34,990. Total debt service across all facilities was £350,803 over six
months.

Operating cash flow before debt was **positive £27,639** in the February–March period and
negative in all five months since — **negative £119,057** over the six months as a whole.
After debt service and HMRC, the six-month cash requirement was **£497,071**, an average of
£82,845 a month.

**11. The company has been kept alive by related parties, not by lending.**

| Six months to 21 Aug 2026 | Amount |
|---|---:|
| Related-party funding, net in | **£319,460** (£53,243/mo) |
| — of which Fishbone Properties loans | £209,230 |
| — of which director loans | £97,900 |
| Own FlexiPay drawdowns | £123,700 |
| New borrowing drawn (August refinance) | £59,451 |
| Repaid to Funding Circle | (£205,255) |

The FlexiPay facility is **net negative £22,104** over six months. It supplied no net cash.
The entire £497,071 shortfall was funded by the group and the directors.

This changes the framing of the previous entry. The question is not whether the lender
facility is amortising — it is, but that is second order. The question is how long Fishbone
Properties Ltd and the directors can keep putting in £53,000 a month, and whether they have
been told that is what they are doing.

**12. HMRC direct payments stopped on 22 April.**
The statements show HMRC NDDS Time to Pay debits of £4,000 (27 Feb), £4,000 (6 Mar) and
£6,649.67 (13 Mar), then a single PAYE/NIC payment of £12,562.03 on 22 April. From 22 April to
21 August — four months — no payment to HMRC left this account. That is consistent with
finding 5 above (Time to Pay refinanced onto FlexiPay, paid lender to HMRC without touching
the current account) rather than contradicting it, but it should be **confirmed against the
HMRC account rather than inferred**. If the arrangement is in fact in default, that is a
different and more urgent problem.

**13. VAT refunds are running, not VAT payments.**
HMRC refunded £10,108.69 on 12 March and £8,915.43 on 12 June — £19,024 over six months. A
construction company in a repayment position on VAT is normal under the domestic reverse
charge, but it should be checked that returns are being filed on time given the Companies
House late-filing penalties of £375 and £150 charged on 20 April.

**14. A second company bank account is being drained.**
Account 24241061 transferred a net £7,877 into 2819 across 24 separate transfers in the
February–March period, then effectively stopped (net −£50, +£52, then nil). Its balance and
purpose are not documented anywhere in this knowledge base.

**15. Two counterparties need a definitive classification.**

- **AT UK Interiors Ltd** paid £10,447.61 (with job reference FC0204) in March and £15,000 in
  August, but also appears on loan-labelled transactions. Treated here as a customer receipt
  where a job reference is present. Confirm whether it is a customer, a group entity, or both.
- **Fishbone Properties Ltd** appears on both job-referenced trading transactions (net £1,580
  over six months, in both directions) and loan transactions (£209,230 net in). The split is
  inferred from the reference text on each line and should be confirmed against the ledgers.

### Notes for next session

- `Raw/Finance` is now fully processed. The next statement to look for covers 22 August to
  21 September 2026.
- The full categorisation and the trend tables are in the working file
  `six_month_analysis.txt`; the per-category monthly figures are in `cats6.json`.
- The 13-week cash flow forecast produced on 4 September was built on the June to August data
  only. Its trading receipt assumption of £16,855 a month is now known to be a post-collapse
  figure, which the forecast should state explicitly.
- `Outputs/` is still empty. The Solvency Briefing and the 13-week forecast still need filing
  there.
- Open question for the group: this knowledge base is meant to feed Fishbone Group. Findings 8
  and 11 both cross entity boundaries — the Macdonald relationship and the £209,230 that
  Fishbone Properties has put in — and neither can be resolved from inside this knowledge base
  alone.

---

**See also:** [Processing Workflow](processing-workflow.md) · [Database Structure](database-structure.md) · [Wiki Maintenance Guidelines](wiki-maintenance-guidelines.md)
