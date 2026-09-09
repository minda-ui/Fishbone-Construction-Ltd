---
title: Group document numbering and filing (policy v1.1)
category: Processes
status: active
sensitive: false
created: 2026-09-09
updated: 2026-09-09
sources:
  - ../../raw/2026-09-09_group-policy_document-numbering-and-filing-v1.1.md
related:
  - ../../CLAUDE.md
  - ../Decisions/2026-09-09-group-document-numbering-policy-adopted.md
  - ../Processes/email-to-tasks.md
---

# Group document numbering and filing (policy v1.1)

Adopted 2026-09-09. The Fishbone Group knowledge base issued a locked, versioned policy to
every group KB (Fishbone Properties, Fishbone Commercial Properties, Fishbone Holdings, Fishbone
Construction, Fishbone Waste, Amfa Furniture, Fishbone SSAS): register every business document
across the group **once**, number it consistently, and file it with the project or company it
belongs to. This article summarises it for this KB; the canonical text is
`Wiki/Process-Document-Numbering-and-Filing.md` (v1.1) in the Fishbone Group database, delivered
here as `Raw/2026-09-09_group-policy_document-numbering-and-filing-v1.1.md`. **Do not edit or
fork these rules locally** - raise anything that doesn't fit as a row on the group's Change
Requests sheet (below); only the group edits the policy.

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

The rules are locked and versioned (currently v1.1). If a document doesn't fit, a rule is
ambiguous, or there's an improvement to suggest, **do not fork the rules** - raise a row on the
group's **Document System - Change Requests** sheet, same workspace:
[sheet](https://app.smartsheet.eu/sheets/hrx6rP255gm8qVVQgX47GjQmqHGWRf576Vmm5hF1) (sheet id
`8918834172004228`). The group reviews the queue and, if a change is warranted, issues a new
policy version and notifies every KB to adopt it.

## Transition: what changes now, what doesn't

- **New qualifying business documents** from now on are registered in the **group** register
  (`FC`-prefixed) and filed in Collaboration Space per the rules above, not added to the local
  `FCD` sheet.
- **The existing local Construction Document Register (`FCD`) and Tasks sheet (`FCT`) keep
  working as they are.** The policy's own transition text says the local register "keeps
  working for now" and that its back-catalogue will be migrated into the group register as a
  follow-on the group runs, with dedup-on-entry throughout so nothing is lost or
  double-numbered. **This KB does not run that migration itself.**
- The `FCT` Tasks sheet is a task-tracking mechanism, not a document register, and is unaffected
  by this policy either way.

## Open questions

- No timeline has been given for when the group will migrate the local `FCD` back-catalogue.
- Whether every existing `FCD` entry should be cross-registered in the group register retroactively,
  or only left for the group's own migration, is not yet decided; not done without an instruction.

## Sources

The policy text as delivered: `Raw/2026-09-09_group-policy_document-numbering-and-filing-v1.1.md`.
Per its own instructions ("do not register it on the Document Register and do not assign it a
document ID - it is a policy notice, not a business document... archive this file per your
normal workflow"), it has been read and adopted here. It has **not** been physically moved or
deleted from `Raw/`: this KB's own rule that "nothing is deleted or moved out of Raw" (`CLAUDE.md`
§1) is stronger and more specific than the group notice's generic "archive it," and takes
precedence for this KB's own files. It is registered as `skipped` in
`Outputs/kb-registers.md`'s Processed items table (not source material for the Wiki) rather than
relocated.

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-09 | Write access confirmed by a scripted add-then-delete test; open questions updated | `Outputs/change-log-2026-09-09-group-document-numbering-write-access-confirmed.md` |
| 2026-09-09 | Created; policy v1.1 adopted | `Outputs/change-log-2026-09-09-group-document-numbering-adopted.md` |
