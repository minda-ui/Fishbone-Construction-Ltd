# Database Structure

> **Mirror of:** [Wiki/Database Structure](https://docs.google.com/document/d/1B0QcXDWazh8KlgOXV8Ei7T-cW4ZegGhLwuTuGvfmvoY/edit) (Google Drive)
> Drive is the working copy. See [README](../README.md) before editing here.

**Last updated:** 2026-08-25

## 1. Overview

The master rate database is the Smartsheet "Сlassifier" sheet (note: name begins with a
Cyrillic С, not Latin C — search accordingly), located in the "1. General" Smartsheet
workspace.

- **Sheet link:** https://app.smartsheet.eu/sheets/RwmFP73FW3JMgHX59mGmjfGFm8hmVPJPxwMjcxC1
- **Sheet ID:** `6344783272478596`

This is the single source of truth for construction cost rates (material, plant, and
labour) used across estimating and pricing work. All other outputs (proposals, cost
plans, comparisons) should trace back to this sheet rather than duplicating rate data
elsewhere.

## 2. Columns

| # | Column | Type | Purpose |
|---|--------|------|---------|
| 0 | Code | Text/Number | Hierarchical or item code (see Section 3) |
| 1 | Description | Text/Number | Item name |
| 2 | Unit | Text/Number | Unit of measure (m2, m3, nr, week, service, l.m, t, bag, pcs, etc.) |
| 3 | Material +Plant Rate (without VAT) | Text/Number | Material/plant unit rate, ex-VAT |
| 4 | Labour Commercial Rate | Text/Number | Client-facing labour rate |
| 5 | Labour Internal Rate | Text/Number | Internal cost labour rate |
| 6 | Note | Text/Number | Free-text notes |
| 7 | Link to supplier | Text/Number | Supplier URL for the priced item |
| 8 | Join | Text/Number, FORMULA | Auto-concatenates Code + Description. Do not edit manually — blank cells here are not a data gap, they just haven't recalculated. |

## 3. Coding scheme

Two layers of rows coexist in the same sheet:

### a) Section headers (decimal outline, no rates)

Format: `1.0`, `1.1`, `1.1.1` ...

These are category/subcategory headers used purely for grouping. They typically have no
Unit or rate values.

### b) Priced items (prefixed codes, carry rate data)

Format: `[Prefix][Section]-[Sequence]`, e.g. `L9.2-001`, `M5-003`, `P3-001`

Prefixes:

- `L` = Labour item (rate lives in col 4/5)
- `M` = Material item (rate lives in col 3)
- `P` = Plant item (rate lives in col 3, sometimes overlapping with Material)

## 4. Sections

Top-level, as of last review — sheet may extend further.

1. Preliminaries (site setup, temporary services, security, safety, temporary works, cleaning)
2. Professional fees (staff, design fees, surveys & reports, utilities connection, testing & commissioning, statutory approvals, insurances & warranties)
3. Demolition
4. Utilities (electricity, water, foul, gas, surface water drainage, BT)
5. Roads and Landscaping
6. Groundworks
7. Substructure
8. Scaffolding
9. Superstructure (brickwork, structural metalwork, timberframe, ...)

Sheet contains 1,116 rows total — later sections beyond 9 have not yet been fully
catalogued in the Wiki. Update this list as new sections are reviewed.

## 5. Known data gaps

Many item rows have Unit set but no rate populated yet (e.g. most Groundworks and
Substructure line items, several Utilities trenching items). These are candidates for
rate research, typically sourced via the "Link to supplier" workflow — see
[Processing Workflow](processing-workflow.md).

## 6. Related Smartsheet assets in "1. General" workspace

- Contacts Database
- Rates for Sourcing
- Templates (folder)

Confirm current relationships between these and the Classifier before assuming linkage —
not yet documented.

---

**See also:** [Processing Workflow](processing-workflow.md) · [Wiki Maintenance Guidelines](wiki-maintenance-guidelines.md) · [Change Log](change-log.md)
