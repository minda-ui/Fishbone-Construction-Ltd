# FP 2401_131 Goathland Avenue — Actuals Processing Instructions

> **Mirror of:** [Wiki/FP 2401 Goathland Avenue - Actuals Processing Instructions](https://docs.google.com/document/d/1L9LR-lo6zZopDsVXLL_wBEKfKFk1RSniTYkzNeqX6Ik/edit) (Google Drive)
> Drive is the working copy. See [README](../README.md) before editing here.

**Last updated:** 2026-09-05 — Reference locations repointed after the Raw folder was
reorganised into supplier subfolders and session logging moved out of `Wiki/Change Log`. The
previous version of 25 August 2026 is in `Archive/` on Drive.

Copy-paste the block below to start a new session on this task.

---

Project: FP 2401_131 Goathland Avenue — process invoices into actual figures.

**Reference locations:**

- **Classifier** (master rates, all projects): Smartsheet sheet `Сlassifier` (note: Cyrillic С),
  sheet_id `6344783272478596`, in workspace "1. General".
- **Budget** (this project): Smartsheet sheet `FP 2401_Budget`, sheet_id `8653045758035844`, in
  workspace "3. Project Delivery" > folder "FP 2401_131 Goathland Avenue".
- **Invoices to process:** Google Drive folder
  `Fishbone Construction Ltd - Knowledge Base/Raw/FP 2401_131 Goathland Avenue`. Since
  5 September 2026 this folder holds one **subfolder per supplier**, not a flat list — look
  inside all of them. It also holds `INDEX.md`, which names the supplier and document date of
  every file already there; read that before opening anything.
- **Session history:** the dated files `change-log-YYYY-MM-DD-<slug>.md` in the `Outputs` folder,
  indexed newest-first in `Outputs/kb-registers.md`. Read the newest entries and the
  "Processed items" table first, so nothing gets double-counted. (The old single
  `Wiki/Change Log` document is **closed** — it holds the record to 5 September 2026 and is not
  appended to.)
- **Standing rules for the whole knowledge base:** `CLAUDE.md` at the root. Section 3c covers
  this task; section 3d covers what these particular documents do and do not read cleanly.

**Task:** Read every invoice in the Raw folder above (and its supplier subfolders) that hasn't
already been logged in the change log. For each line item on each invoice:

1. **Match the line item to a Budget Code.**
   - If the Code already exists as a row in FP 2401_Budget → go to step 2.
   - If the Code exists in the Сlassifier but not yet in FP 2401_Budget → I'll add it to Budget
     as an actuals-only row (no Quantity-plan), so it doesn't distort the current budget total
     but still captures real cost data for future estimating.
   - If the item has no matching Code anywhere → **stop and confirm with me.** If I confirm it's
     genuinely new, add it to the Сlassifier first (following the existing Code convention:
     prefix L/M/P + section number + sequence, e.g. M15-035), positioned in the correct section,
     then mirror it into Budget as an actuals-only row.
   - If the match is ambiguous (different spec/size, unclear unit conversion, or multiple Budget
     rows share the same Code) → **stop and ask me before writing anything. Never guess.**

2. **Convert the invoice quantity/unit** to match the Budget/Classifier unit (e.g. sheets → m²,
   bags → kg, lengths → l.m.). If multiple invoices or lines cover the same Code, compute a
   weighted average rate across all of them unless I say to keep them separate.

3. **Update the Budget row:** Quantity-actual, Actual Rate, and Notes for actual. Notes must
   always cite the invoice number, date, and the calculation used (so it's auditable later).

4. Work through items **one at a time and confirm each with me** before writing to Smartsheet —
   unless I've explicitly said to go ahead with the whole batch.

5. If an invoice is clearly for a different project, **flag it to me** before doing anything with
   it (don't process or delete without confirming).

6. When a batch is done, write a **new dated file** in `Outputs` named
   `change-log-YYYY-MM-DD-<slug>.md` — never edit an existing one, and never reopen the closed
   `Wiki/Change Log` document. Include: which Raw files were processed, what changed in the
   Classifier, what changed in the Budget, any Wiki changes, and anything the next session needs
   to know (open questions, assumptions made, gaps still outstanding). Then add a row to the
   "Change-log entries" table and update the "Processed items" table in `Outputs/kb-registers.md`.

---

## Conventions established so far

- New Classifier lines get Note field: `Sourced from [Supplier] invoice [number] ([date]): [breakdown].`
- New Budget actuals-only lines get Notes for actual: `[Supplier] invoice [number] ([date]), [breakdown]. No plan quantity set — actuals only, logged for future budget reference.`
- Duplicate-coded Budget rows (same Code, different Note/room) are only split on my explicit
  instruction (e.g. evenly across rooms) — otherwise ask which row applies.

## Reading the documents

Learned 2026-08-25, extended 2026-09-05. See `CLAUDE.md` §3d.

- **Screwfix/Plumbfix classic invoices print a GROSS "Unit Price".** Use the Net column, never
  the printed unit price.
- **Screwfix "Order History" screenshot PDFs have NO TEXT LAYER** — extraction returns only the
  string `Account Details _ Screwfix Website`. They must be downloaded, rasterized and read
  visually. Over 40 of the 68 files in `Screwfix and Plumbfix/` are of this kind. They state
  values inclusive of VAT, so ex-VAT is gross / 1.2; with a whole-order discount, each line's
  share is estimated proportionally by list price and flagged as estimated in the Notes.
- **JT Dove invoices** show ex-VAT prices directly in their line-item columns — verify against
  the printed Goods/VAT totals.
- **Photographed till receipts** (B&Q Trade Point, JT Dove, YESSS Electrical, National Plastics)
  read well through Drive's own image reading, including the VAT analysis block. The transaction
  date sometimes does not survive; `INDEX.md` records which files have no readable date.
- **Many documents are addressed to Fishbone Drylining Ltd** or "FISHBONE DRY LINING". That is
  **this** company under its former name (renamed 31 October 2024). They are our own purchases,
  not a related party's.

The 99 files already in this folder were all processed on 25 August 2026 and are logged in the
closed `Wiki/Change Log`. Check `INDEX.md` and the `Outputs` change log before assuming any file
is new.

---

**See also:** [CLAUDE.md](../CLAUDE.md) · [Wiki index](index.md) · [kb-registers](../outputs/kb-registers.md) · [Database Structure](database-structure.md) · [Processing Workflow](processing-workflow.md)
