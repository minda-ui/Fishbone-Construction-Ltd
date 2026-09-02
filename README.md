# Fishbone Construction Ltd — Knowledge Base (version-controlled mirror)

This repository is a **version-controlled mirror of the Wiki** from the
[Fishbone Construction Ltd - Knowledge Base](https://drive.google.com/drive/folders/13IQdim0JhKmoQvJBmJmnMhreJqg55xTr)
Google Drive folder. It exists to give the documentation history, diffs, and review —
things Google Docs revision history doesn't give you at a glance.

**Google Drive remains the working copy.** Edit articles there. This repo is where those
edits get recorded over time.

## What's in here

| Article | Drive original |
|---|---|
| [Database Structure](wiki/database-structure.md) | [Doc](https://docs.google.com/document/d/1B0QcXDWazh8KlgOXV8Ei7T-cW4ZegGhLwuTuGvfmvoY/edit) |
| [Processing Workflow](wiki/processing-workflow.md) | [Doc](https://docs.google.com/document/d/1Ll7U39oormzFJBqZUVBYIWFuLHUSh7DOYQ3RwCVTSsA/edit) |
| [Wiki Maintenance Guidelines](wiki/wiki-maintenance-guidelines.md) | [Doc](https://docs.google.com/document/d/1mXih5Syp9WkcWuKU68pm6WXoSF8hhjOGJaSx9qoO6Ww/edit) |
| [Change Log](wiki/change-log.md) | [Doc](https://docs.google.com/document/d/16mrZzs9dWDZ-qP7wIgCvv9WFF9hCN8WQAZOQDfNcBJ0/edit) |
| [FP 2401 Goathland Avenue — Actuals Processing Instructions](wiki/fp-2401-goathland-avenue-actuals-processing-instructions.md) | [Doc](https://docs.google.com/document/d/1DhIWxjLuwahp1LbZp7QlV9OXg7WZWHh5mq-LL_FKzd8/edit) |

Mirrored as of **2026-09-02**. All five articles carried "Last updated: 2026-08-25" at
that point.

## What is deliberately NOT in here

This repo holds **documentation only**. Keep the following out of it:

- **Rate and budget data** — lives in Smartsheet (the `Сlassifier` sheet and the
  per-project Budget sheets). The Wiki describes that data; it never duplicates it.
- **Raw source material** — supplier invoices, quotes, bank statements and the like stay
  in `Raw/` on Drive. `.gitignore` blocks the common formats as a backstop.
- **Outputs** — generated reports and exports belong in `Outputs/` on Drive.

## Where the real systems live

- **Classifier** (master rates, all projects) — Smartsheet, workspace "1. General",
  sheet_id `6344783272478596`.
  [Open sheet](https://app.smartsheet.eu/sheets/RwmFP73FW3JMgHX59mGmjfGFm8hmVPJPxwMjcxC1)
  Note the sheet name begins with a **Cyrillic С**, not a Latin C — search accordingly.
- **FP 2401_Budget** — Smartsheet, workspace "3. Project Delivery" > folder "FP 2401_131
  Goathland Avenue", sheet_id `8653045758035844`.
- **Drive knowledge base** — `Raw/` (unprocessed input), `Wiki/` (mirrored here),
  `Outputs/` (deliverables).

## Keeping the mirror honest

A stale mirror is worse than no mirror, because it looks authoritative. So:

1. When you change an article in Drive, update the matching file here **in the same
   session** — the same rule the
   [Wiki Maintenance Guidelines](wiki/wiki-maintenance-guidelines.md) already apply to
   the Wiki itself.
2. One commit per article change, with a message saying what changed and why — that's the
   whole point of having this in git.
3. Keep the wording verbatim. This is a mirror, not a rewrite. Structural markdown
   (headings, lists, tables, links) is fine; changing what an article *says* is an edit
   that belongs in Drive first.
4. If Drive and this repo disagree, **Drive wins.** Fix the repo, don't fix Drive from
   the repo.
5. New Wiki article on Drive → add it here and to the table above.

## Conventions inherited from the Wiki

Each article opens with a `Last updated: YYYY-MM-DD` line and ends with a "See also"
list. Both are load-bearing — see the
[Wiki Maintenance Guidelines](wiki/wiki-maintenance-guidelines.md).
