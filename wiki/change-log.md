# Change Log

> **Mirror of:** [Wiki/Change Log](https://docs.google.com/document/d/16mrZzs9dWDZ-qP7wIgCvv9WFF9hCN8WQAZOQDfNcBJ0/edit) (Google Drive)
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

---

**See also:** [Processing Workflow](processing-workflow.md) · [Database Structure](database-structure.md) · [Wiki Maintenance Guidelines](wiki-maintenance-guidelines.md)
