# Fishbone Construction Ltd — Knowledge Base (version-controlled mirror)

This repository is a **version-controlled mirror** of the
[Fishbone Construction Ltd - Knowledge Base](https://drive.google.com/drive/folders/13IQdim0JhKmoQvJBmJmnMhreJqg55xTr)
Google Drive folder. It exists to give the documentation history, diffs, and review — things
Google Docs revision history doesn't give you at a glance.

**Google Drive remains the working copy.** Edit there. This repo is where those edits get
recorded over time. When the two disagree, Drive wins.

## Start here

- **[`CLAUDE.md`](CLAUDE.md)** — standing context and all the rules. Read it before working
  in this knowledge base, in either copy.
- **[`wiki/index.md`](wiki/index.md)** — every article.
- **[`outputs/kb-registers.md`](outputs/kb-registers.md)** — what has been processed, what
  changed when, and the index of dated change-log entries.

## Layout

```
CLAUDE.md                  standing context (authoritative)
README.md                  this file
archive/                   manifest of superseded copies (content is Drive-only — see below)
outputs/                   dated change-log entries + kb-registers.md
raw/                       index files only; no source material (see below)
wiki/
├── index.md               every article is listed here
├── _templates/article.md  front matter and section skeleton
├── Customers/             Macdonald Joinery, AT UK Interiors
├── Decisions/             why the knowledge base is shaped the way it is
├── Finance/               the bank account, receipts, debt, lending, HMRC
├── Processes/             data capture and accounting systems
├── Projects/              FP 2401 Goathland Avenue
├── Suppliers/             subcontractors, trade suppliers
└── *.md                   five legacy documents, still Google Docs on Drive
```

## What is deliberately NOT in here

This repo holds **documentation only**.

- **Source material** — supplier invoices, bank statement CSVs, Companies House filings — stays
  on Drive in `Raw/`. `.gitignore` blocks `*.csv`, `*.xlsx` and `*.pdf` so it cannot arrive by
  accident. `raw/` here holds only the `INDEX.md` that says what those files are.
- **Rate and budget data** — lives in Smartsheet (the `Сlassifier` sheet and the per-project
  Budget sheets). The wiki describes that data; it never duplicates it.
- **Personal data** — subcontractors are named individuals. Articles resting on bank data give
  totals and limited-company names only, and point at the Drive-only CSVs for the rest.
- **The content of superseded files.** `Archive/` on Drive holds the previous copy of every
  standing file that has been replaced, each titled with the reason it was replaced. Here,
  [`archive/README.md`](archive/README.md) mirrors that **listing** but not the file contents:
  git already versions everything in this repo, and the archived titles are where the
  information actually lives. This is the one place the mirror is deliberately partial.

## The five legacy documents

Five articles pre-date the current structure and are still Google Docs at the root of `Wiki/`
on Drive. They are mirrored here as Markdown at `wiki/*.md`, and listed in `wiki/index.md`
under "Unfiled". Whether to convert and refile them is an open decision for the owner.

| Article | Drive original |
|---|---|
| [Change Log](wiki/change-log.md) (**closed 2026-09-05**) | [Doc](https://docs.google.com/document/d/1yaATUPhHuuXOvJ1oi-DLi-gWn1ykTXoYXMhntgOjntc/edit) |
| [Database Structure](wiki/database-structure.md) | [Doc](https://docs.google.com/document/d/1B0QcXDWazh8KlgOXV8Ei7T-cW4ZegGhLwuTuGvfmvoY/edit) |
| [FP 2401 Goathland Avenue — Actuals Processing Instructions](wiki/fp-2401-goathland-avenue-actuals-processing-instructions.md) | [Doc](https://docs.google.com/document/d/1L9LR-lo6zZopDsVXLL_wBEKfKFk1RSniTYkzNeqX6Ik/edit) |
| [Processing Workflow](wiki/processing-workflow.md) | [Doc](https://docs.google.com/document/d/1Ll7U39oormzFJBqZUVBYIWFuLHUSh7DOYQ3RwCVTSsA/edit) |
| [Wiki Maintenance Guidelines](wiki/wiki-maintenance-guidelines.md) | [Doc](https://docs.google.com/document/d/1mXih5Syp9WkcWuKU68pm6WXoSF8hhjOGJaSx9qoO6Ww/edit) |

Two of those Drive links changed on 2026-09-05: the Change Log and the Goathland instructions
were both re-issued and their previous copies archived, so they have new document ids. The
links above are the live ones.

## A note on paths

Drive uses `Wiki/`, `Outputs/`, `Raw/` and `Archive/`; this repo uses lowercase `wiki/`,
`outputs/`, `raw/` and `archive/`. Article *content* is mirrored verbatim, but relative links
that cross a top-level folder differ in case between the two copies. Where a Drive document
links `../Wiki/Customers/at-uk-interiors.md`, the mirror names the file in backticks instead of
linking it, so the repo has no broken links and the Drive copy keeps its working ones.

Mirrored as of **2026-09-05**.
