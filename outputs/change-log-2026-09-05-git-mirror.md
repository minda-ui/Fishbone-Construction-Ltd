# 2026-09-05 - Drive mirrored to the git repository

Owner asked for everything to be mirrored to `minda-ui/Fishbone-Construction-Ltd`. Before this
the repo carried five Markdown files - the legacy wiki documents as at 2026-09-02 - and nothing
created since. It was roughly 100 KB behind.

## What was mirrored

| Path in the repo | Files |
|---|---|
| `CLAUDE.md` | v2, 23.8 KB |
| `README.md` | rewritten; the old one listed five articles and two dead document ids |
| `wiki/index.md`, `wiki/_templates/article.md` | 2 |
| `wiki/Customers/`, `wiki/Decisions/`, `wiki/Finance/`, `wiki/Processes/`, `wiki/Projects/`, `wiki/Suppliers/` | 13 articles |
| `outputs/` | `kb-registers.md` + 4 dated change-log entries, including this one |
| `raw/FP 2401_131 Goathland Avenue/INDEX.md` | 1 |
| `archive/README.md` | manifest only - see below |

Every wiki article was written to disk from the same text uploaded to Drive and the byte counts
compared file by file. All thirteen match exactly.

## Two documents brought up to date, not just copied

- **`wiki/change-log.md`.** The repo copy still had the pre-closure header, pointed at a Drive
  document id that is now the archived copy, and carried the six-month bank entry inline. It now
  carries the closure banner, points at the re-issued document, and ends by naming
  `outputs/change-log-2026-09-05-six-month-bank-data.md` as where that entry moved to. The four
  historical entries above it are untouched.
- **`wiki/fp-2401-goathland-avenue-actuals-processing-instructions.md`.** Rewritten from the
  re-issued Drive document: supplier subfolders, the `Outputs/` change log, and the document
  reading limits learned on 2026-09-05.

## Where the mirror is deliberately not exact

Two deviations, both recorded rather than silently absorbed.

**1. `Archive/` content is not mirrored.** `archive/README.md` reproduces the listing - every
archived filename and the reason in it - but not the files themselves. Git already versions
everything in this repo, so copying nine superseded drafts across would store the same
information twice, and the information that matters is in the titles. The `CLAUDE.md` §1 rule
that Drive and git `Archive/` folders must be comparable **by name** is satisfied; the rule that
both copies be mirrored is not, and that is the deviation.

**2. Path case differs, so a few links do.** Drive uses `Wiki/`, `Outputs/`, `Raw/`, `Archive/`;
the repo uses lowercase. Article content is verbatim, but a relative link that crosses a
top-level folder cannot be identical in both. Where a Drive document links
`../Wiki/Customers/at-uk-interiors.md`, the mirror names the file in backticks instead, so
neither copy has a broken link. Noted in the repo `README.md`.

## Two corrections made on Drive to keep the copies honest

Mirroring surfaced a divergence rather than creating one, which is the useful side effect of
copying a thing carefully.

- **`Wiki/Decisions/2026-09-05-kb-skeleton-adopted.md`** carried an open question - "the wiki
  holds almost no substance yet" - that twelve articles had answered four hours later. Rather
  than let the mirror quietly improve on Drive, the Drive article was re-issued with the
  question marked closed and the previous copy archived. Both copies now say the same thing.
- **`Archive/` was counted, not estimated.** Nine files. The manifest says so and says when it
  was counted, per `CLAUDE.md` §6d rule 3 - a rule this session had already breached once.

## Notes for next session

- The repo now stands as a complete copy of the Drive knowledge base as at 2026-09-05, with the
  two exceptions above. Any Drive edit from here needs the same-session mirror update that
  `CLAUDE.md` §1 requires.
- Nothing in this entry changes what is actually known about the company. The open questions in
  `CLAUDE.md` §7 are unchanged, and the first of them - why Macdonald Joinery stopped paying -
  is still unanswered.
