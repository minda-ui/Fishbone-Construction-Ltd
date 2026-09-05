# Archive — manifest

On Drive, `Archive/` holds the previous copy of every standing file that has been replaced,
each renamed `<original> (archived YYYY-MM-DD, superseded by <specific reason>)`. Done
consistently, that listing becomes the knowledge base's own changelog: you can read what
changed and why without opening anything.

**This directory mirrors the listing, not the contents.** Git already versions every file in
this repo, so duplicating superseded copies here would store the same information twice. The
part that carries the meaning — the reason in each title — is below. The full content of each
archived file is on Drive.

This is the one place the mirror is deliberately partial. It is recorded in
`outputs/change-log-2026-09-05-git-mirror.md`.

## Contents of `Archive/` on Drive

Counted 2026-09-05: **nine files**, all archived that day. The knowledge base was assembled and
revised in a single session, which is why every entry shares a date.

| Archived file | Superseded because |
|---|---|
| `2026-09-05-kb-skeleton-adopted.md (archived …, superseded by copy closing the open question about the empty wiki, which 12 articles answered later that day).md` | Its open question was answered four hours after it was written |
| `CLAUDE.md (archived …, superseded by v2 after 12 wiki articles were built and §7's claim that the wiki was almost empty became false).md` | §7 said the wiki was almost empty; it stopped being true the same day |
| `Change Log (archived …, superseded by the copy carrying the banner that logging moved to Outputs)` | Google Doc. Session logging moved to dated files in `Outputs/`; the doc was re-issued with a banner saying so |
| `FP 2401 Goathland Avenue - Actuals Processing Instructions (archived …, superseded by copy repointed at the supplier subfolders and the Outputs change log)` | Google Doc. Its "Reference locations" block pointed at the flat Raw folder and at the now-closed Change Log |
| `index.md (archived …, superseded by copy with the Change Log link corrected after that doc was re-issued).md` | Pointed at the pre-closure copy of the Change Log |
| `index.md (archived …, superseded by copy fixing the Goathland instructions link, which wrongly pointed at the Change Log doc).md` | Two entries pointed at the same document |
| `index.md (archived …, superseded by copy correcting the Archive count, which said four superseded copies where three existed).md` | A number asserted without counting — `CLAUDE.md` §6d rule 3 |
| `index.md (archived …, superseded by copy listing the 12 articles built from the six-month bank data).md` | The wiki gained five categories and twelve articles |
| `kb-registers.md (archived …, superseded by copy recording the wiki build and the Finance CSVs moving from partial to done).md` | The six statement CSVs moved from `partial` to `done` once their findings reached wiki articles |

Titles are abbreviated here with `…` in place of the repeated `2026-09-05`; on Drive each
carries the full date.

Four of the nine are copies of `index.md`. Three of those four record a defect in the file that
replaced it — two broken links and one count stated without counting. That is the manifest doing
its job: the failures are legible from the listing alone.
