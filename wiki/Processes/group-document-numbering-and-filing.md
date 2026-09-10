---
title: Group document numbering and filing (policy v1.3)
category: Processes
status: active
sensitive: false
created: 2026-09-09
updated: 2026-09-10
sources:
  - ../../raw/2026-09-09_group-policy_document-numbering-and-filing-v1.1.md
  - ../../raw/2026-09-09_group-policy_document-numbering-and-filing-v1.2.md
  - ../../raw/2026-09-10_group-policy_document-numbering-and-filing-v1.3.md
related:
  - ../../CLAUDE.md
  - ../Decisions/2026-09-09-group-document-numbering-policy-adopted.md
  - ../Processes/email-to-tasks.md
---

# Group document numbering and filing (policy v1.3)

Adopted 2026-09-09 at v1.1; updated the same day to v1.2; updated again 2026-09-10 to **v1.3**.
The Fishbone Group knowledge base issued a locked, versioned policy to every group KB (Fishbone
Properties, Fishbone Commercial Properties, Fishbone Holdings, Fishbone Construction, Fishbone
Waste, Amfa Furniture, Fishbone SSAS): register every business document across the group
**once**, number it consistently, and file it with the project or company it belongs to. This
article summarises it for this KB; the canonical text is
`Wiki/Process-Document-Numbering-and-Filing.md` (v1.3) in the Fishbone Group database, delivered
here as `Raw/2026-09-10_group-policy_document-numbering-and-filing-v1.3.md` (v1.1 and v1.2
arrived first, on 2026-09-09; all three stay in `Raw/`, per this KB's own immutability rule -
see Sources below). **Do not edit or fork these rules locally** - raise anything that doesn't
fit as a row on the group's Change Requests sheet (below); only the group edits the policy.

## The one register

A single Smartsheet **Document Register** for the whole group, in the **"Fishbone Group -
Documents"** workspace:
[sheet](https://app.smartsheet.eu/sheets/4W2xwP9c2gfCpvWPGJmPHg2P2QwJfxPmWXpCvC21) (sheet id
`7352854736144260`). Columns: `Document No. | Entity (owner) | Direction | Date | Category |
Title | Entities involved | Description | Status | Source key | File link | Location`.

This KB **reads** it (to check whether a document is already registered) and **appends its own
rows**. Never edit or delete another entity's row. **Read and write access both confirmed
2026-09-09.** Read: the sheet was empty when first checked. Write: a scripted add-then-delete
test (a row tagged `TEST-ACCESS-CHECK`, `Entity = FC`, `Status = Void`, added then immediately
removed) confirmed this KB's connection can add and delete rows on the shared sheet. By the time
of the write test, Amfa Furniture Ltd had already added its own first real row (`FA0000001`,
its change-of-name certificate) as an end-to-end proof of concept - the test row was added,
verified, and removed without disturbing it.

## This KB's prefix, and a naming collision to watch for

Fishbone Construction Ltd's prefix in the **group** register is **`FC`** (2 letters). This is a
**different namespace from the existing local Construction Smartsheet workspace**, which already
uses `FCT` (Tasks) and `FCD` (Document Register) - see
[Email intake, document register and tasks](email-to-tasks.md). `FC0000001` (group) and
`FCD0000001` (local) are not the same document register and must not be conflated. The policy's
own transition guidance (below) is what keeps them apart for now.

Other group prefixes: `FP` Properties · `FH` Holdings · `FW` Waste · `FA` Amfa Furniture ·
`FM` Commercial Properties · `FS` SSAS · `FG` group-level.

## ID scheme

`<PREFIX>` + **7 zero-padded digits**, e.g. `FC0000001`. One continuous sequence per entity
(incoming and outgoing share the same counter; filter on `Direction`/`Category` instead of
splitting the sequence). Numbers are **never reused** - a killed or replaced document is marked
`Superseded`/`Void` on its row, and the new version gets a new number that references the old
one. (A document number is 7 digits; a *property* code, e.g. `FP1601`, is 4 - count the digits
if unsure which you're looking at.)

**Property codes (§3/§7, new in v1.3).** A property code is `<PREFIX>` + **4 digits** =
2-digit acquisition year + 2-digit sequence (e.g. `FP1601` = acquired 2016, sequence 01). Each
company **self-assigns** its own property codes on this pattern and records them in its own
property register - there is no central index and the group does not issue codes.
Property-tied documents file in Collaboration Space under `<PROPERTY CODE> - <Address>/
Documents/`; the uncoded `Company/Project/Documents` folder is only for projects that are not a
property. **Not applicable to this KB**: Fishbone Construction Ltd owns no property (its
`Assets` Wiki category covers vehicles only - see `Wiki/Assets/vehicles.md`), so it has no
property codes and no property register to maintain.

## The anti-duplication rule

`one owning entity → one row → one ID → one stored file`. A document that touches more than one
company is recorded **once**, under its owning entity, with the others named in `Entities
involved` - never a second row or number.

**Dedup-on-entry, before minting any number:** search the register by `Source key` (the
document's Google Drive file id, or a Gmail thread id) and by matching title + date +
counterparty. If a row already matches, **reuse that ID** rather than minting a new one, and
record the `Source key` so the same source is never numbered twice.

## What gets a number

Register anything meaningful to the record or audit trail: statutory accounts and CT600s;
certificates; title registers/plans, leases and tenancies; loan/mortgage documents; board and
intercompany letters/minutes; legal, lender, insurer and Companies House/HMRC correspondence;
valuations; completion/redemption statements; property- or project-tied invoices and receipts.

**Do not register:** marketing/newsletters; generic recurring bills with no property/entity tie;
duplicates; routine automated notifications. If it's unclear, raise it - don't guess.

**Tasks are not documents (§6, new in v1.2).** A task, to-do or action item - including an
automation's own action list - is not a business record and gets no Document Register row and
no document ID, whatever channel it arrived through (a task sheet, an email thread that is
itself just a to-do). Keep tasks in a task sheet/tracker (this KB's `FCT` sheet) instead. A
document is registered only once a thread yields a verified business record: an actual stored
file, or an email that is itself the record (its Gmail thread id as `Source key`). This
clarification came out of `FC-CR-0001` (below) and settles that `FCD0000001`-`FCD0000014`
correctly stay off the group register.

**Email-attachment source capture (§5, new in v1.3).** When the record *is* an email
attachment but its bytes can't be captured into Drive (a known limitation of this KB's own
info-mailbox pipeline - most `Raw/Email/*.json` captures note "Attachments remain in Gmail and
are not yet filed/validated"), register the row with the **Gmail thread id as `Source key`**
and a **plain-text transcription** of the attachment as the stored record, flagged as a
transcription in both the Description and the change-log entry. Dedup still works on the stable
thread id; if the binary is captured later, attach it and update `File link` without changing
the ID. This directly addresses the gap the info-mailbox pipeline has carried since 2026-09-06 -
see [Email intake, document register and tasks](email-to-tasks.md) - though retroactively
applying it to the existing captured-but-unfiled attachments is a separate piece of work, not
done as part of adopting this policy update.

## Filing - with the project, in Collaboration Space

Keep the file in the shared **Collaboration Space** library, co-located in the folder of the
thing it belongs to (that project's or property's `Documents/` folder; company-level items in
that company's "Company Documents" folder; group-level `FG` items in the group documents
folder). Name every file `<ID> - <Category> - <Short Title>.<ext>`. The register row's `File
link` and `Location` point back to it. Use Drive **move** (preserves the file id) so existing
links keep resolving. Keep superseded files - never overwrite; set the old row to
`Superseded`/`Void` and register the new version under a new number that references the old one.

## Handing a document to another group company (new in v1.1, §7a)

A document may be passed to another group KB so it can be processed into that KB's own
knowledge, **only** like this:
- The document must **already be on the Document Register**. Drop a copy into the **other KB's
  `Raw/` inbox** - add a new file, never touch anything already there, and nothing outside
  `Raw/` - named with its **existing ID**: `<ID> - <Category> - <Short Title>.<ext>`.
- Add a short covering note to that same `Raw/`, named
  `YYYY-MM-DD_handoff_<fromEntity>-to-<toEntity>_<ID>.md`, saying why it was sent and what (if
  anything) is needed back.
- Annotate the document's **existing** register row: `Direction = Internal`, and "sent to
  `<receiving KB>` `YYYY-MM-DD`". **Never** create a new number, a second register row, or a
  second stored copy.
- Receiving end: a `Raw/` file whose name already carries a document ID is already registered -
  reuse that ID, extract what's needed into the Wiki citing it, and archive the working copy.
  Never re-number it.
- This is the **only** write this KB may make into another KB, and vice versa - it needs Drive
  write access to that KB's `Raw/`; until granted, ask for the file to be copied in instead.
  Personal/credential documents are never registered, so they can never be sent this way.

## Locked rules, one feedback channel

The rules are locked and versioned (currently v1.3). If a document doesn't fit, a rule is
ambiguous, or there's an improvement to suggest, **do not fork the rules** - raise a row on the
group's **Document System - Change Requests** sheet, same workspace:
[sheet](https://app.smartsheet.eu/sheets/hrx6rP255gm8qVVQgX47GjQmqHGWRf576Vmm5hF1) (sheet id
`8918834172004228`). The group reviews the queue and, if a change is warranted, issues a new
policy version and notifies every KB to adopt it - `FC-CR-0001` below is the first instance of
that loop running end to end.

## Transition: what changes now, what doesn't

- **New qualifying business documents** from now on are registered in the **group** register
  (`FC`-prefixed) and filed in Collaboration Space per the rules above, not added to the local
  `FCD` sheet.
- **Each KB may now migrate its own local back-catalogue whenever it's ready (§11, new in
  v1.2)** - deduping on entry against the group register (by `Source key` and by title + date +
  counterparty), and retiring the local sheet once its live entries are migrated. This replaced
  v1.1's "the group runs the migration" position, per `FC-CR-0001` below. For this KB, that
  question is now moot: the local Construction Document Register's back-catalogue outside the
  MSEM case is `FCD0000001`-`FCD0000014`, and all 14 are tasks under the new §6 rule above, so
  none of them migrate regardless of who is allowed to run it.
- The `FCT` Tasks sheet is a task-tracking mechanism, not a document register, and is unaffected
  by this policy either way - if anything, §6 above makes the boundary between the two sheets
  sharper than before.

## First real registration: `FC0000001`

2026-09-09, at the owner's instruction: the MSEM UK Ltd v Fishbone Construction Ltd County
Court claim (019JE538)'s **Claim form** - the document that started the case, already local as
`FCD0000018` - registered as `FC0000001`. It was already filed correctly in Collaboration Space
(`Fishbone Construction / C Legal & Court Cases / MSEM UK Ltd Claim – BBC Cardiff/`); only a
rename to the `<ID> - <Category> - <Short Title>` convention was needed, done in place (same
Drive file id). The local `FCD0000018` row was updated to cross-reference `FC0000001`. Detail:
`Outputs/change-log-2026-09-09-first-group-register-document.md`.

Only the Claim form was registered at first - the case's other local documents
(`FCD0000015`-`FCD0000023`) were not also given group numbers. That was a deliberate limit, not
an oversight, and was recorded as open below.

## The rest of the case: `FC0000002`-`FC0000009`

2026-09-09, later the same day, at the owner's explicit instruction ("register
FCD0000015–FCD0000023"): the case's other 8 local documents were registered too, as
`FC0000002` through `FC0000009` (ascending local-ID order; `FCD0000018` was already
`FC0000001`). Two (`FCD0000015`, `FCD0000016`) are physically in this KB's own `Raw/` and were
renamed in place there, per this KB's own Raw-immutability rule taking precedence over the
group's Collaboration Space filing convention; the other six were already in Collaboration
Space and were renamed in place. All 8 local `FCD` rows were cross-referenced back to their new
`FC` numbers. Two details were deliberately excluded from the shared descriptions: a claimant's
individual contact's home address (personal-data minimisation, as for `FC0000001`), and a live
Money Claims Online security/access code found in one document's covering note (a credential,
not appropriate for a register shared across seven companies). Detail:
`Outputs/change-log-2026-09-09-msem-case-documents-registered.md`.

This shows the previous section's "deliberate limit" was exactly that - a limit tied to the
instruction given at the time, lifted the moment a broader instruction was given. It was not a
policy position that only originating documents get registered.

## The rest of the local back-catalogue: raised as `FC-CR-0001`, resolved the same day

2026-09-09, later the same day again: the owner asked to migrate the rest of the local `FCD`
back-catalogue too. Checking it first (23 rows total; 9 now `FC0000001`-`FC0000009`) found the
remaining 14 (`FCD0000001`-`FCD0000014`) are not documents in the sense the MSEM ones were:
each is a task/email-tracking row from the Construction info-mailbox pipeline, its `File link`
is a Gmail message URL with no stored file or Drive file id, and its Description says the
underlying attachment or record is "not yet filed/validated" or "not verified". Titles read as
action items ("Reconcile Tower Leasing invoice 916284 overdue notice", "Verify Forth England
INV-1627 payment and filing") rather than document titles - closer to the local `FCT` Tasks
mechanism than to a registrable document.

**Not migrated at the time; raised instead as `FC-CR-0001`** on the group's Document System -
Change Requests sheet: whether these 14 rows qualify for the group register at all, and,
separately, whether this KB is expected to run any part of the back-catalogue migration or wait
for a group-run pass. Detail: `Outputs/change-log-2026-09-09-back-catalogue-change-request-raised.md`.

**Resolved the same day: Accepted.** The group reviewed `FC-CR-0001` and replied by delivering
policy **v1.2** to `Raw/` (found on a later check of that folder): (1) task/email-tracking rows
with no verified business record do **not** qualify for the register - confirms the decision not
to migrate the 14; (2) each KB may now migrate its own back-catalogue whenever ready, deduping
on entry - the group no longer runs a central migration. Both are now in the policy text above
(§6 and the Transition section). For this KB specifically, point (2) turns out to be moot: with
point (1) in force, there is no back-catalogue left to migrate - all 23 local `FCD` rows are
accounted for (9 as group documents, 14 correctly excluded as tasks). Detail:
`Outputs/change-log-2026-09-09-v1.2-adopted.md`.

## Policy v1.3: property codes and email-attachment transcription

2026-09-10, found on a `/Raw` check requested by the owner: the group delivered **v1.3**,
resolving two *other* companies' change requests - `FM-CR-0001` (Fishbone Commercial
Properties) and `FP-CR-0001` (Fishbone Properties), both Accepted 2026-09-10. Neither request
was raised by this KB, but the resulting clarifications apply group-wide, per the two new
sections above (property codes; email-attachment transcription). Adopted the same day, per the
same reasoning as v1.2's own adoption: read it, fold the clarifications into this article and
`CLAUDE.md`, leave the notice file in `Raw/`. Detail:
`Outputs/change-log-2026-09-10-v1.3-and-kosmosoft-quote.md`.

## Open questions

- None outstanding on this policy. `FC-CR-0001` is closed (Accepted, resolved 2026-09-09); the
  local back-catalogue question is settled with nothing left to migrate. v1.3 raised no question
  for this KB - property codes don't apply (no property), and the email-attachment
  transcription pattern is available to use going forward but applying it retroactively to the
  existing unfiled attachments is separate, undecided work.

## Sources

The policy text as delivered, in order:
`Raw/2026-09-09_group-policy_document-numbering-and-filing-v1.1.md`,
`Raw/2026-09-09_group-policy_document-numbering-and-filing-v1.2.md` and
`Raw/2026-09-10_group-policy_document-numbering-and-filing-v1.3.md`. Per their instructions
("do not register it on the Document Register and do not assign it a document ID - it is a
policy notice, not a business document... archive this file per your normal workflow"), all
three have been read and adopted here. None has been physically moved or deleted from `Raw/`:
this KB's own rule that "nothing is deleted or moved out of Raw" (`CLAUDE.md` §1) is stronger
and more specific than the group notice's generic "archive it," and takes precedence for this
KB's own files. All three are registered as `skipped` in `Outputs/kb-registers.md`'s Processed
items table (not source material for the Wiki) rather than relocated.

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-10 | Policy v1.3 adopted (property codes, email-attachment transcription) | `Outputs/change-log-2026-09-10-v1.3-and-kosmosoft-quote.md` |
| 2026-09-09 | Policy v1.2 adopted; `FC-CR-0001` resolved (Accepted); no back-catalogue left to migrate | `Outputs/change-log-2026-09-09-v1.2-adopted.md` |
| 2026-09-09 | Rest of the local `FCD` back-catalogue: raised as `FC-CR-0001`, not migrated | `Outputs/change-log-2026-09-09-back-catalogue-change-request-raised.md` |
| 2026-09-09 | Rest of the MSEM case registered (`FC0000002`-`FC0000009`) | `Outputs/change-log-2026-09-09-msem-case-documents-registered.md` |
| 2026-09-09 | First real document registered (`FC0000001`, the MSEM claim form) | `Outputs/change-log-2026-09-09-first-group-register-document.md` |
| 2026-09-09 | Write access confirmed by a scripted add-then-delete test; open questions updated | `Outputs/change-log-2026-09-09-group-document-numbering-write-access-confirmed.md` |
| 2026-09-09 | Created; policy v1.1 adopted | `Outputs/change-log-2026-09-09-group-document-numbering-adopted.md` |
