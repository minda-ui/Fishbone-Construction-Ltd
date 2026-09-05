# Knowledge base registers - Fishbone Construction Ltd

Standing indexes over the whole knowledge base. Unlike the dated change-log entries beside this
file, which are written once and never touched again, this file is current state: it is
replaced (archive-then-recreate, per `CLAUDE.md` §1) whenever a row is added.

Three of its four tables answer "what is the state of the knowledge base now", not "what
happened in a session". The fourth, the entry index, is the chronology.

## Change-log entries

One file per session or run, in `Outputs/`, newest first. Never edited after it is written; a
correction is a new entry that references the old one.

| Date | Entry | File |
|---|---|---|
| 2026-09-05 | Macdonald Joinery: the owner answered why | `Outputs/change-log-2026-09-05-macdonald-answered.md` |
| 2026-09-05 | Drive mirrored to the git repository | `Outputs/change-log-2026-09-05-git-mirror.md` |
| 2026-09-05 | Wiki built from the six months of bank data - 12 articles, 5 categories | `Outputs/change-log-2026-09-05-wiki-from-bank-data.md` |
| 2026-09-05 | Standard KB skeleton applied; Raw invoices grouped by supplier | `Outputs/change-log-2026-09-05-kb-skeleton-and-raw-tidy.md` |
| 2026-09-05 | Remaining three Finance CSVs processed; six months of bank data complete | `Outputs/change-log-2026-09-05-six-month-bank-data.md` |
| 2026-09-05 | Bank data processed; company identity correction; solvency and cash analysis | `Wiki/Change Log` (closed Google Doc), entry dated 2026-09-05 |
| 2026-08-25 | FP 2401 Goathland Avenue: large invoice batch (60+ files) - COMPLETE | `Wiki/Change Log` (closed Google Doc) |
| 2026-08-25 | FP 2401 Goathland Avenue: first invoice batch (9 files) | `Wiki/Change Log` (closed Google Doc) |
| 2026-08-25 | Workspace set up | `Wiki/Change Log` (closed Google Doc) |

The four oldest entries live in the single `Change Log` Google Doc in `Wiki/`, which was the
logging mechanism until 2026-09-05. It is **closed, not deleted**: it is still the record of
that period and carries a banner pointing here. Everything from 2026-09-05 onward is a dated
file in this folder.

## Processed items

Status: `pending` = registered, not started · `partial` = started, work remains (see notes) ·
`done` = fully reflected in the wiki · `skipped` = deliberately not processed (reason in notes).

| Raw path | Processed (date) | Status | Wiki articles created / updated | Notes |
|---|---|---|---|---|
| `Raw/Finance/20260321_04212819.csv` | 2026-09-05 | done | Finance/hsbc-current-account, Finance/trading-receipts, Finance/debt-service, Finance/funding-circle-flexipay, Finance/related-party-funding, Finance/hmrc, Customers/macdonald-joinery, Customers/at-uk-interiors, Suppliers/subcontractors, Suppliers/trade-suppliers | HSBC 04212819, 22 Feb to 21 Mar 2026. Categorised and reconciled to every printed balance. Sensitive: financial data. Drive-only. |
| `Raw/Finance/20260421_04212819.csv` | 2026-09-05 | done | same as above | HSBC 04212819, 22 Mar to 21 Apr 2026. |
| `Raw/Finance/20260521_04212819.csv` | 2026-09-05 | done | same as above | HSBC 04212819, 22 Apr to 21 May 2026. |
| `Raw/Finance/20260621_04212819.csv` | 2026-09-03 | done | same as above | HSBC 04212819, 22 May to 21 Jun 2026. |
| `Raw/Finance/20260721_04212819.csv` | 2026-09-03 | done | same as above | HSBC 04212819, 22 Jun to 21 Jul 2026. |
| `Raw/Finance/20260821_04212819.csv` | 2026-09-03 | done | same as above | HSBC 04212819, 22 Jul to 21 Aug 2026. |
| `Raw/2024-10-31 Companies House certificate of change of name - Fishbone Drylining Ltd to Fishbone Construction Ltd (07948220).pdf` | 2026-09-04 | done | Finance/funding-circle-flexipay, Suppliers/trade-suppliers | Certificate of incorporation on change of name plus the NM01 and the special resolution. Renamed 2026-09-05 from `application-pdf.pdf`. |
| `Raw/FP 2401_131 Goathland Avenue/` (99 invoice and receipt files) | 2026-08-25, re-read 2026-09-05 | done | Projects/fp-2401-goathland-avenue, Suppliers/trade-suppliers | Processed into ~40 new Classifier codes and the FP 2401 Budget on 2026-08-25. Every file re-read 2026-09-05 to identify its supplier; grouped into 8 supplier folders; see that folder's `INDEX.md`. |
| `Raw/2026-09-05_owner-note_macdonald-joinery-has-no-projects.md` | 2026-09-05 | done | Customers/macdonald-joinery | Owner (Managing Director) verbal statement written up by the assistant: Macdonald Joinery has no projects. Answers what five months of bank data could not. In Drive `Raw/` and the mirror. |
| `Raw/FP 2401_131 Goathland Avenue/INDEX.md` | 2026-09-05 | skipped | none | Folder index written by this KB, not source material. Registered so §3b Detect does not re-flag it. |

**The six Finance CSVs moved from `partial` to `done` on 2026-09-05.** They were `partial`
because their findings existed only in change-log entries, which are never revised. Twelve wiki
articles now carry them.

## Wiki structure changes

| Date | Change | Reason |
|---|---|---|
| 2026-08-25 | Created `Wiki/` with four Google Docs: Database Structure, Wiki Maintenance Guidelines, Processing Workflow, Change Log | Initial setup |
| 2026-08-25 | Added `Wiki/FP 2401 Goathland Avenue - Actuals Processing Instructions` | Copy-paste session-starter for the invoice-to-actuals task |
| 2026-09-02 | Five Wiki articles mirrored into `minda-ui/Fishbone-Construction-Ltd` as Markdown | Owner asked for the Wiki to be version-controlled. Drive remains the working copy |
| 2026-09-05 | Created `Wiki/index.md`, `Wiki/_templates/article.md`, `Wiki/Decisions/`, root `CLAUDE.md`, root `README.md`, `Archive/`, `Outputs/kb-registers.md` | The standard skeleton had never been applied to this KB, unlike the two sister KBs |
| 2026-09-05 | `Wiki/Change Log` closed and re-issued with a banner; the previous copy archived. Logging moved to dated `Outputs/change-log-*.md` files | Owner instruction, matching Fishbone Properties Ltd and Fishbone Commercial Properties Ltd |
| 2026-09-05 | `Wiki/FP 2401 Goathland Avenue - Actuals Processing Instructions` re-issued; previous copy archived | Its "Reference locations" block pointed at the flat Raw folder and at `Wiki/Change Log`. Both had changed. §6d rule 1 outbound-reference repair |
| 2026-09-05 | Created categories `Finance/`, `Customers/`, `Suppliers/`, `Projects/`, `Processes/` with 12 articles; `index.md` rebuilt | Owner asked for the six months of bank findings to be moved out of write-once change-log entries into revisable articles |
| 2026-09-05 | `index.md` replaced four times in one session | Three link and count defects, each named in its archived copy's title. The last was a count asserted without counting - §6d rule 3 |
| 2026-09-05 | `Wiki/Decisions/2026-09-05-kb-skeleton-adopted.md` re-issued; previous copy archived | Its open question about the empty wiki was answered by the 12 articles built four hours later. Found while mirroring to git |
| 2026-09-05 | Whole knowledge base mirrored to `minda-ui/Fishbone-Construction-Ltd`; `wiki/change-log.md` and the Goathland instructions mirror brought up to date | The repo carried only the five legacy documents as at 2026-09-02. Two deviations recorded in the entry: `Archive/` is mirrored as a manifest, and path case differs |
| 2026-09-05 | `Wiki/Customers/macdonald-joinery.md` re-issued; `CLAUDE.md` replaced by v3; `Wiki/index.md` re-issued. All three previous copies archived | The owner answered why Macdonald Joinery stopped paying. §7's first open question closed and replaced by "what replaces the revenue?" |

## Outputs produced

| Output path | Date | Built from | Requested by |
|---|---|---|---|
| `Fishbone Construction - Solvency Briefing v2 - 4 Sep 2026.docx` | 2026-09-04 | The June-August bank categorisation and the group Loans database | Owner |
| `Fishbone 13-Week Cash Flow Forecast.xlsx` | 2026-09-04 | The same categorisation, driven from an editable assumptions sheet | Owner |

**Both of these still exist only outside this knowledge base**, and both are now doubly out of
date: they rest on a trading receipts assumption of £16,855 a month that
`Wiki/Finance/trading-receipts.md` supersedes, and they were built before it was known that the
customer behind most of that figure has no projects. Filing them should mean re-issuing them.
