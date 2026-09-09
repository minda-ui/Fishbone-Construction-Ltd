# Knowledge base registers - Fishbone Construction Ltd

Standing indexes over the whole knowledge base. Unlike the dated change-log entries beside this
file, which are written once and never touched again, this file is current state: it is
replaced (archive-then-recreate, per `CLAUDE.md` §1) whenever a row is added.

Three of its four tables answer "what is the state of the knowledge base now", not "what
happened in a session". The fourth, the entry index, is the chronology.

**This copy merges two versions that were written concurrently and both went live at once**
(2026-09-09, around 07:58 and 08:05) - one added the MSEM court-case workspace, the other added
this session's vehicle-workspace addendum; neither knew about the other's row when it was
written. Both archived copies are kept, titled with this as the reason. If a third concurrent
write happens again, check for more than one live `kb-registers.md` before trusting a single
read of this file.

## Change-log entries

One file per session or run, in `Outputs/`, newest first. Never edited after it is written; a
correction is a new entry that references the old one.

| Date | Entry | File |
|---|---|---|
| 2026-09-09 | Rest of the MSEM case registered in the group Document Register (FC0000002-FC0000009); CLAUDE.md replaced by v8 | `Outputs/change-log-2026-09-09-msem-case-documents-registered.md` |
| 2026-09-09 | First real document registered in the group Document Register (FC0000001, MSEM claim form); CLAUDE.md replaced by v7 | `Outputs/change-log-2026-09-09-first-group-register-document.md` |
| 2026-09-09 | Group Document Register: write access confirmed; CLAUDE.md replaced by v6 | `Outputs/change-log-2026-09-09-group-document-numbering-write-access-confirmed.md` |
| 2026-09-09 | Group document-numbering policy (v1.1) adopted; CLAUDE.md replaced by v5 | `Outputs/change-log-2026-09-09-group-document-numbering-adopted.md` |
| 2026-09-09 | MSEM UK Ltd case workspace built for claim 019JE538 (BBC Cardiff dispute) | `Outputs/change-log-2026-09-09-msem-case-workspace.md` |
| 2026-09-09 | Vehicle workspace addendum: Wiki/Assets category, CLAUDE.md v4, and a folder mix-up corrected | `Outputs/change-log-2026-09-09-vehicle-workspace-created-addendum.md` |
| 2026-09-09 | County Court claim 019JE538: trial date and allocation notice registered | `Outputs/change-log-2026-09-09-court-notice-019je538.md` |
| 2026-09-09 | Vehicles workspace created; Ford Transit identified, two vehicles still awaited (written retrospectively) | `Outputs/change-log-2026-09-09-vehicle-workspace-created.md` |
| 2026-09-09 | Morning intake: closed the Mail Register gap, added the Fishbone Holdings dividend finding | `Outputs/change-log-2026-09-09-morning-intake.md` |
| 2026-09-08 | Morning intake; SiteDocs progress and three follow-ups | `Outputs/change-log-2026-09-08-morning-intake.md` |
| 2026-09-06 | Info-only Smartsheet workspace, eight tasks, archive pilot and scheduled intake | `Outputs/change-log-2026-09-06-info-workspace-setup.md` |
| 2026-09-06 | Construction inbox housekeeping review; proposal only | `Outputs/change-log-2026-09-06-inbox-housekeeping-review.md` |
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

**Three entries touch "vehicle workspace" or overlapping 2026-09-09 subjects** because multiple
sessions were editing this knowledge base concurrently that day. Read all of them for the full
picture; none was overwritten.

## Processed items

Status: `pending` = registered, not started · `partial` = started, work remains (see notes) ·
`done` = fully reflected in the wiki · `skipped` = deliberately not processed (reason in notes).

| Raw path | Processed (date) | Status | Wiki articles created / updated | Notes |
|---|---|---|---|---|
| `MSEM UK Ltd Claim - BBC Cardiff` folder (Drive, owned by lana@fishboneconstruction.co.uk; not this KB's Raw/) plus `Raw/2026-09-09 Claimant's N180...pdf` | 2026-09-09 | done | none (sensitive legal correspondence; tracked in Tasks/Document Register and the case folder's own INDEX.md, per the FCT00007/FCD0000007 pattern) | Pre-existing case folder discovered and indexed rather than duplicated - see `Outputs/change-log-2026-09-09-msem-case-workspace.md`. Registered FCD0000017-FCD0000023; opened FCT00015-FCT00018. **The Claim form (local FCD0000018) additionally registered 2026-09-09 in the group Document Register as FC0000001** - this KB's first real (non-test) entry there; file renamed in place to the ID convention, not moved. See `Outputs/change-log-2026-09-09-first-group-register-document.md`. **The case's other 8 local documents (FCD0000015, 016, 017, 019, 020, 021, 022, 023) additionally registered 2026-09-09 in the group Document Register as FC0000002-FC0000009**, at the owner's explicit instruction; two files renamed in place in this KB's own Raw/, six renamed in place in Collaboration Space; a claimant contact's home address and a live Money Claims Online security code were deliberately excluded from the shared register. See `Outputs/change-log-2026-09-09-msem-case-documents-registered.md`. |
| `Raw/2026-09-09 County Court Lincoln - Notice of Trial Date and Allocation to Small Claims Track - claim 019JE538 (MSEM UK LTD v Fishbone Construction Ltd).pdf` | 2026-09-09 | done | none (sensitive legal correspondence; tracked in Tasks/Document Register only, per the FCT00007/FCD0000007 pattern) | Scanned notice, uploaded directly to Raw/ (not via email). Renamed from `Document_2026-09-09_073700.pdf`. Registered as FCD0000015; FCT00007 updated with the new hearing (19 Nov 2026), evidence-exchange deadline (21 Oct 2026) and claimant trial-fee deadline (22 Oct 2026). No filing, response or contact made. |
| `Raw/Vehicles/INDEX.md` | 2026-09-09 | skipped | Assets/vehicles | Folder index written by this KB, not source material. Registered so §3b Detect does not re-flag it. Vehicle #1 (Ford Transit HT22BWP) confirmed against bank data and the group Loans database; Haydock Finance ruled out as machinery, not a vehicle; Tower Leasing and vehicles #2/#3 still open. Findings written up in both `Wiki/Assets/vehicles.md` and the 2026-09-09 vehicle-workspace change-log entries. |
| `Raw/2026-09-09_group-policy_document-numbering-and-filing-v1.1.md` | 2026-09-09 | skipped | Processes/group-document-numbering-and-filing, Decisions/2026-09-09-group-document-numbering-policy-adopted | Group-wide policy notice from the Fishbone Group knowledge base (not a business document - explicitly marked "do not register on the Document Register"). **Adopted 2026-09-09** at the owner's instruction: rules written up in the two Wiki articles named, `CLAUDE.md` §1 gets one pointer row. Establishes a single cross-entity Document Register (Smartsheet, sheet id `7352854736144260`) with 7-digit per-entity-prefixed IDs (`FC` for Construction), running alongside - not replacing - the existing local `FCT`/`FCD` numbering, whose back-catalogue migration is the group's own follow-on. **Read and write access both confirmed 2026-09-09** (write via a scripted add-then-delete test row, immediately removed). **First real registration also 2026-09-09: FC0000001**, the MSEM court claim's Claim form. Left in place in `Raw/`, not moved - see the Decisions article. |
| Raw/Email/2026-09-09-morning-intake.json | 2026-09-09 | done | Processes/email-to-tasks, Finance/related-party-funding | Four message bodies (Tower Leasing follow-up, SiteDocs cancellation confirmation, Pensions Regulator re-enrolment reminder, FY2025 dividend request). Tasks/Document Register entries (FCT00001 update, FCT00004, FCT00012-FCT00014; FCD0000012-FCD0000014) were already written by the scheduled routine before this session; this session added the four missing Mail Register rows (FCM0000079-FCM0000082), the two Wiki updates above, and this entry. Attachment capture, the starred-count discrepancy and the 25 August historical backlog remain outstanding. |
| Raw/Email/2026-09-08-morning-intake.json | 2026-09-08 | partial | Processes/email-to-tasks | Eight bodies captured, three new tasks; portal and attachment evidence pending. |
| Raw/Email/2026-09-06-info-pilot.json | 2026-09-06 | partial | Processes/email-to-tasks | Fourteen message bodies captured; eight follow-ups. Attachments, entity routing and complete source review remain pending. |
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

**`Raw/Vehicles/` is a live intake point.** The owner will upload vehicle documents into it over
time; each new document should get its own row here (`pending` on arrival) per §3b, and the
folder's own `INDEX.md` should be kept current alongside this table.

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
| 2026-09-06 | Created `Wiki/Processes/email-to-tasks.md`; indexed in `index.md`; `Raw/Email/` established as the source folder for captured message bodies | Owner-authorised Construction Smartsheet workspace and info-mailbox intake pipeline. `CLAUDE.md` was updated in place with an operational-update banner rather than through archive-then-recreate - corrected below |
| 2026-09-09 | Created `Raw/Vehicles/` (INDEX.md plus one vehicle subfolder); no Wiki article yet at this point | Owner identified the company's vehicles; vehicle 1 (Ford Transit HT22BWP) confirmed against bank data and the group Loans database, two more awaited |
| 2026-09-09 | Created `Wiki/Assets/` category and `Wiki/Assets/vehicles.md`; created `Wiki/Decisions/2026-09-09-assets-category-and-vehicles-workspace.md`; `Wiki/index.md` re-issued to list both; `CLAUDE.md` replaced by v4 (folding the 2026-09-06 in-place edit into proper archive-then-recreate, adding the Assets/Vehicles workspace to §1, and adding §6d rule 5 on that gap) | Closes the "no Wiki article yet" gap left by the row above |
| 2026-09-09 | Added `INDEX.md` to the pre-existing (non-KB) `MSEM UK Ltd Claim - BBC Cardiff` Drive folder; no Wiki article | Consolidates the claim 019JE538 case papers and a readiness checklist. Deliberately outside `Wiki/`, matching the sensitive-legal-matter pattern already used for FCT00007/FCD0000007. |
| 2026-09-09 | Created `Wiki/Processes/group-document-numbering-and-filing.md` and `Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md`; `Wiki/index.md` re-issued to list both; `CLAUDE.md` replaced by v5 (one new row in §1's live-data-sources table) | Owner instruction to adopt the Fishbone Group's document-numbering policy (v1.1). Detailed rules kept in the Wiki per §6d rule 4, not inlined into `CLAUDE.md` |
| 2026-09-09 | Both Wiki articles above updated (write-access confirmed, open questions trimmed); `CLAUDE.md` replaced by v6 (one word in §1's table) | Owner instruction to confirm write access to the group Document Register; confirmed by a scripted add-then-delete test |
| 2026-09-09 | Both Wiki articles above updated again (first real registration recorded); `CLAUDE.md` replaced by v7 (one addition to §1's table) | Owner instruction to register the MSEM court claim's Claim form as `FC0000001`, the first real (non-test) entry in the group Document Register |
| 2026-09-09 | Both Wiki articles above updated again (rest of the MSEM case recorded); `CLAUDE.md` replaced by v8 (one addition to §1's table) | Owner instruction to register `FCD0000015`-`FCD0000023`; the case's remaining 8 local documents registered as `FC0000002`-`FC0000009` |

## Outputs produced

| Output path | Date | Built from | Requested by |
|---|---|---|---|
| `Outputs/inbox-housekeeping-plan-2026-09-06.md` | 2026-09-06 | Construction mailbox and sister-KB procedures; proposal only | Owner |
| `info-mailbox-archive-pilot-2026-09-06.json` | 2026-09-06 | Info-mailbox pilot run (immutable rollback manifest) | Owner |
| `inbox-processing-state.json` | 2026-09-06 | Info-mailbox pilot run (standing partial intake state) | Owner |
| `Fishbone Construction - Solvency Briefing v2 - 4 Sep 2026.docx` | 2026-09-04 | The June-August bank categorisation and the group Loans database | Owner |
| `Fishbone 13-Week Cash Flow Forecast.xlsx` | 2026-09-04 | The same categorisation, driven from an editable assumptions sheet | Owner |

**Both of the last two still exist only outside this knowledge base**, and both are now doubly
out of date: they rest on a trading receipts assumption of £16,855 a month that
`Wiki/Finance/trading-receipts.md` supersedes, and they were built before it was known that the
customer behind most of that figure has no projects. Filing them should mean re-issuing them.
