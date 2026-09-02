# Processing Workflow (Raw → Classifier)

> **Mirror of:** [Wiki/Processing Workflow](https://docs.google.com/document/d/1Ll7U39oormzFJBqZUVBYIWFuLHUSh7DOYQ3RwCVTSsA/edit) (Google Drive)
> Drive is the working copy. See [README](../README.md) before editing here.

**Last updated:** 2026-08-25

## 1. Purpose

Defines how new items land in the Raw folder, get reviewed, and end up correctly priced
and coded in the Classifier Smartsheet (or elsewhere, if out of scope).

## 2. What goes in "Raw"

Anything not yet processed: supplier quotes, scraped price lists, new item requests, PDFs
of catalogues, spreadsheets from subcontractors, photos of spec sheets, etc. Raw is a
staging area only — nothing in Raw should be treated as authoritative for pricing.

## 3. Step-by-step process

### Step 1 — Intake

New file(s) added to Raw. No action required at this point beyond noting they exist.

### Step 2 — Triage

For each item in a Raw file, determine:

a) Does it already exist in the Classifier (check Code/Description via Smartsheet search
   or `find_in_sheet`)?
b) If yes → this is a rate UPDATE, not a new item.
c) If no → this is a NEW ITEM needing a new Code.

### Step 3 — Classify (new items only)

Assign a Code following the existing scheme (see
[Database Structure](database-structure.md)):

- Confirm which top-level section (1.0–9.0+) the item belongs to, or propose a new
  section if genuinely novel.
- Assign prefix: `L` (labour), `M` (material), `P` (plant).
- Assign next available sequence number within that section/prefix.
- Fill Description and Unit.

### Step 4 — Price

- Material/Plant rate → column "Material +Plant Rate (without VAT)"
- Labour Commercial Rate and Labour Internal Rate → respective columns
- Always populate "Link to supplier" with the source URL/quote reference the rate came
  from — this is mandatory, not optional (it's how the rate gets audited later).
- Use "Note" for anything a future reader needs to know (e.g. rate is regional, rate
  excludes delivery, quote expires).

### Step 5 — Write to Classifier

Add the row(s) to the Сlassifier sheet (sheet_id `6344783272478596`) via Smartsheet
tools. For rate updates to an existing row, edit in place rather than duplicating the
row.

### Step 6 — Log the change

Add an entry to the [Change Log](change-log.md) — what was processed, source, number of
rows added/updated, and date. This is what lets a new session pick up where the last one
left off without re-deriving context.

### Step 7 — Clear Raw (optional)

Once a Raw file's items are fully processed and logged, it can be archived or removed
from Raw so the folder only shows what's still pending. Confirm with the owner before
deleting; moving to an "Archive" subfolder is the safer default if unsure.

## 4. Outputs

Any deliverable generated from the Classifier data (a filtered export, a client-facing
rate schedule, a comparison report) goes in Outputs, not Wiki or Raw.

## 5. Quality checks before closing out a batch

- No new row lacks a Code, Unit, or at least one rate.
- No new Material/Plant/Labour item is missing a supplier link.
- Section numbering wasn't duplicated or skipped inconsistently.
- Change Log entry added.

---

**See also:** [Database Structure](database-structure.md) · [Wiki Maintenance Guidelines](wiki-maintenance-guidelines.md) · [Change Log](change-log.md)
