# FP 2401_131 Goathland Avenue — Actuals Processing Instructions

> **Mirror of:** [Wiki/FP 2401 Goathland Avenue - Actuals Processing Instructions](https://docs.google.com/document/d/1DhIWxjLuwahp1LbZp7QlV9OXg7WZWHh5mq-LL_FKzd8/edit) (Google Drive)
> Drive is the working copy. See [README](../README.md) before editing here.

**Last updated:** 2026-08-25

Copy-paste the block below to start a new session on this task.

---

<!-- COPY FROM HERE -->

Project: FP 2401_131 Goathland Avenue — process invoices into actual figures.

**Reference locations:**

- Classifier (master rates, all projects): Smartsheet sheet "Сlassifier" (note: Cyrillic
  С), sheet_id `6344783272478596`, in workspace "1. General".
- Budget (this project): Smartsheet sheet "FP 2401_Budget", sheet_id
  `8653045758035844`, in workspace "3. Project Delivery" > folder "FP 2401_131 Goathland
  Avenue".
- Invoices to process: Google Drive folder "Fishbone Construction ltd/Raw/FP 2401_131
  Goathland Avenue".
- Change Log (session history): Google Drive "Fishbone Construction ltd/Wiki/Change Log"
  — read this first to see what's already been processed, so nothing gets double-counted.

**Task:** Read every invoice in the Raw folder above that hasn't already been logged in
the Change Log. For each line item on each invoice:

1. Match the line item to a Budget Code.
   - If the Code already exists as a row in FP 2401_Budget → go to step 2.
   - If the Code exists in the Сlassifier but not yet in FP 2401_Budget → I'll add it to
     Budget as an actuals-only row (no Quantity-plan), so it doesn't distort the current
     budget total but still captures real cost data for future estimating.
   - If the item has no matching Code anywhere → stop and confirm with me. If I confirm
     it's genuinely new, add it to the Сlassifier first (following the existing Code
     convention: prefix L/M/P + section number + sequence, e.g. M15-035), positioned in
     the correct section, then mirror it into Budget as an actuals-only row.
   - If the match is ambiguous (different spec/size, unclear unit conversion, or multiple
     Budget rows share the same Code) → stop and ask me before writing anything. Never
     guess.

2. Convert the invoice quantity/unit to match the Budget/Classifier unit (e.g. sheets →
   m², bags → kg, lengths → l.m.). If multiple invoices or lines cover the same Code,
   compute a weighted average rate across all of them unless I say to keep them separate.

3. Update the Budget row: Quantity-actual, Actual Rate, and Notes for actual. Notes must
   always cite the invoice number, date, and the calculation used (so it's auditable
   later).

4. Work through items one at a time and confirm each with me before writing to
   Smartsheet — unless I've explicitly said to go ahead with the whole batch.

5. If an invoice is clearly for a different project, flag it to me before doing anything
   with it (don't process or delete without confirming).

6. When a batch is done, append a new dated entry to the Wiki/Change Log — never
   overwrite previous entries. Include: which Raw files were processed, what changed in
   the Classifier, what changed in the Budget, any Wiki changes, and anything the next
   session needs to know (open questions, assumptions made, gaps still outstanding).

<!-- COPY TO HERE -->

---

## Notes on conventions established so far

- New Classifier lines get Note field: "Sourced from [Supplier] invoice [number]
  ([date]): [breakdown]."
- New Budget actuals-only lines get Notes for actual: "[Supplier] invoice [number]
  ([date]), [breakdown]. No plan quantity set — actuals only, logged for future budget
  reference."
- Duplicate-coded Budget rows (same Code, different Note/room) are only split on my
  explicit instruction (e.g. evenly across rooms) — otherwise ask which row applies.

---

**See also:** [Processing Workflow](processing-workflow.md) · [Database Structure](database-structure.md) · [Change Log](change-log.md)
