# 2026-09-05 - Standard KB skeleton applied; Raw invoices grouped by supplier

Owner asked for this knowledge base to be brought up to the standard of the two sister KBs. It
had never had the skeleton applied: `Raw/` and a flat `Wiki/`, no `CLAUDE.md`, no `README.md`,
an empty `Outputs/`, no `Archive/`.

## Created

| Path | What it is |
|---|---|
| `CLAUDE.md` | Standing context, version 1. Modelled on the live `CLAUDE.md` of `Fishbone Commercial Properties Ltd - Knowledge Base`, which was itself built from a survey of the CLAUDE.md files on this Drive. Its §1, §2, §4 and §6d rules were adopted rather than re-derived, because each has a real failure behind it recorded there. |
| `README.md` | Short pointer to `CLAUDE.md`. |
| `Archive/` | Did not exist. For superseded copies of replaced standing files, named `<original> (archived YYYY-MM-DD, superseded by <reason>)`. |
| `Outputs/kb-registers.md` | The four standing tables: change-log entries, processed items, wiki structure changes, outputs produced. `Outputs/` was completely empty before today. |
| `Outputs/change-log-2026-09-05-six-month-bank-data.md` | The six-month bank analysis entry, moved here from the Google Doc. |
| `Wiki/index.md` | Lists every article. |
| `Wiki/_templates/article.md` | Front matter and section skeleton for new articles. |
| `Wiki/Decisions/` | New category, with one article recording this decision. |
| `Raw/FP 2401_131 Goathland Avenue/INDEX.md` | What each of the 99 files in that folder actually is. |

## Change logging moved out of the Google Doc

Per owner instruction, the single `Wiki/Change Log` Google Doc is **closed, not deleted**. It
carries a banner at the top saying logging has moved to `Outputs/`, and it keeps all four of its
historical entries verbatim. The previous copy was archived rather than overwritten, because
Drive has no in-place edit for a Google Doc and adding the banner means recreating the file:
`Archive/Change Log (archived 2026-09-05, superseded by copy carrying the moved-to-Outputs
banner)`.

The reasoning is the sister KB's, and it is about write cost, not tidiness. That KB's monolith
had reached 44,895 bytes and grew about 5 KB a session; every entry meant rewriting the whole
file and archiving the previous copy, which is why its `Archive/` held 14 timestamped snapshots,
some two minutes apart. One file per run, written once, removes that entirely. This KB's doc was
only 19 KB but on exactly the same trajectory - it had been fully rewritten twice today already.

## `Raw/` tidied

**The Companies House PDF was renamed.** `application-pdf.pdf` said nothing about its contents.
Read first, then renamed to
`2024-10-31 Companies House certificate of change of name - Fishbone Drylining Ltd to Fishbone
Construction Ltd (07948220).pdf`. It is a certificate of incorporation on change of name plus
the NM01 filing and the special resolution, company 07948220, dated 31 October 2024.

**The 99 project documents were grouped by supplier.** They sat in one flat folder,
`Raw/FP 2401_131 Goathland Avenue/`, 91 of them named only by their numeric Dext transaction id.

*A correction to the request:* the instruction described these as being in `Raw/Finance/`. They
are not. `Raw/Finance/` holds exactly six files, the HSBC statement CSVs. The receipt scans -
including `21561043400.jpeg`, the example given - are in the Goathland project folder. The work
was done there.

**Each of the 99 files was opened and read**, and the supplier taken from the document itself.
Nothing was inferred from file size or from the id prefix, both of which cluster suggestively
and would have been wrong: the 45 KB PDFs are not one supplier, and neither are the 133 KB ones.

| Files | Folder |
|---:|---|
| 68 | `Screwfix and Plumbfix/` |
| 7 | `B and Q Trade Point/` |
| 7 | `Galaxy Insulation and Dry Lining/` |
| 3 | `Victorian Plumbing/` |
| 2 | `Consumer Unit World/` |
| 2 | `JT Dove/` |
| 2 | `YESSS Electrical/` |
| 8 | `Other suppliers (single invoices)/` - CEF, IronmongeryDirect, J P McDougall (Dulux), Lilley Tile and Stone, National Plastics, NT Steel Services, Quay Timber, SP Partitions |
| **99** | |

**Supplier, not month.** Every document falls between 16 April and 24 August 2026 and most are
June, so grouping by month would have put almost everything in one folder. Supplier is the
division that actually separates them - and it is the one that matches how the money leaves the
bank, so a supplier folder can be reconciled against a supplier's line in the statement
categorisation.

**Files were not renamed.** The Dext id is the link back to Dext and to the Budget and
Classifier notes written when this batch was processed on 2026-08-25. Renaming would have broken
that. `INDEX.md` in the folder carries the identification instead: every file, its supplier, and
its document date.

## Two references repaired, not left dangling

This is the `CLAUDE.md` §6d rule 1 outbound check - the rule that exists because a sister KB left
three references pointing at sections that had been archived.

`Wiki/FP 2401 Goathland Avenue - Actuals Processing Instructions` is a copy-paste session
starter, and its "Reference locations" block named two things that changed today: the Raw folder
(now has supplier subfolders) and `Wiki/Change Log` (now closed). Both were repaired and the
previous copy archived. Anyone pasting the old block would have been told to read a closed
document and would have found an empty-looking Raw folder.

## Findings on reading these documents

Recorded because they will recur, and are now in `CLAUDE.md` §3d.

- **Screwfix "Order History" screenshot PDFs have no text layer.** Text extraction returns the
  single string `Account Details _ Screwfix Website` and nothing else - no date, no line items,
  no total. 40+ of the 68 Screwfix files are of this kind. They must be rasterised and read
  visually, which is what the 2026-08-25 session did.
- **Photographed till receipts OCR well** through Drive's own image reading, including the VAT
  analysis block - B&Q Trade Point, JT Dove, YESSS Electrical and National Plastics all read
  cleanly. The transaction date sometimes does not survive.
- **Many documents are addressed to Fishbone Drylining Ltd**, or to "FISHBONE DRY LINING". That
  is this company under its former name, and several trade accounts were never updated after the
  October 2024 change. Screwfix, Consumer Unit World and IronmongeryDirect all still hold the old
  name; one Consumer Unit World order even went to `minda@fishbonedrylining.co.uk`. This is the
  same trap that produced the misreading corrected on 2026-09-04.

## Not done, deliberately

- **The five legacy Google Docs in `Wiki/` were not moved into category folders.** They are live
  and correct; converting them to Markdown and foldering them changes URLs the owner uses and
  the reference block inside the Goathland instructions. Listed in `Wiki/index.md` under
  "Unfiled" with the question put to the owner.
- **No access review.** Both sister KBs ran one and found things. This one has not been checked
  and `CLAUDE.md` §6b says so rather than assuming it is owner-only.
- **`Outputs/` still does not hold the Solvency Briefing or the 13-week forecast.** They have
  been flagged as unfiled in every entry since 2026-09-05 and this does not change that - they
  were built before the six-month data existed, so filing them should mean re-issuing them.

## Notes for next session

- The wiki is still almost empty of substance. Six months of reconciled bank data, fifteen
  suppliers and a customer collapse all live in change-log entries, which are written once and
  never revised - the wrong home for facts that change. Building `Finance/`, `Customers/`,
  `Suppliers/` and `Projects/` articles from those entries is the largest outstanding task.
- The git mirror `minda-ui/Fishbone-Construction-Ltd` does not yet carry any of today's new
  files. Only `wiki/change-log.md` has been updated there.
