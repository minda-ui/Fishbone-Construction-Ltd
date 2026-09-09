---
title: Group document-numbering policy adopted
category: Decisions
status: active
sensitive: false
created: 2026-09-09
updated: 2026-09-09
sources:
  - ../../outputs/change-log-2026-09-09-group-document-numbering-adopted.md
related:
  - ../index.md
  - ../Processes/group-document-numbering-and-filing.md
---

# Group document-numbering policy adopted

The Fishbone Group knowledge base delivered a locked, versioned policy (v1.1) to every group KB,
found while checking `Raw/` for new documents, then adopted into this KB on the owner's
instruction. Full rules: `Wiki/Processes/group-document-numbering-and-filing.md`. This article
records the decisions made in adopting it, not the rules themselves.

## Why a new register rather than folding into the existing local one

The existing Construction Smartsheet workspace already has a `Document Register` (`FCD`-numbered)
and `Tasks` sheet (`FCT`-numbered), built 2026-09-06 for the info-mailbox intake pipeline. The
group's new register uses a **different prefix** (`FC`, no `D`) and a **different sheet**
entirely, in a new "Fishbone Group - Documents" workspace shared with six other companies. These
are not reconcilable by simply renaming a column - they are two different systems with
different owners (this KB's own Construction workspace vs. the group's cross-company one).

**Decision: keep both, don't merge them locally.** The policy's own transition text says the
local register "keeps working for now" and that migrating its back-catalogue into the group
register is a follow-on the *group* runs - not something to attempt unilaterally here, since it
would mean re-numbering documents other sessions and the owner already reference by their `FCD`
numbers (e.g. the MSEM court case's `FCD0000015`-`FCD0000023`). Doing that without being asked
would be exactly the kind of "invent a local variation" the policy explicitly rules out.

## What was and wasn't done

- **Adopted:** the rules, into a new `Wiki/Processes/` article (per `CLAUDE.md` §6d rule 4 -
  detailed rule sets belong in the Wiki, not in `CLAUDE.md` itself), with a short pointer added
  to `CLAUDE.md` §1's live-data-sources table.
- **Confirmed:** read access to the group Document Register sheet (0 rows, as expected for a
  brand-new sheet at the time), and **write access**, via a scripted add-then-delete test row
  (`TEST-ACCESS-CHECK`, `Entity = FC`, `Status = Void`) added and immediately removed, leaving
  the sheet exactly as found. By then Amfa Furniture Ltd had already added its own first real
  row (`FA0000001`) as an end-to-end proof of concept; the test did not disturb it.
- **Not done:** registering anything real in the new group register yet. No qualifying document
  has come up since adoption to register for real - the access test used a clearly-marked,
  deleted placeholder rather than a real document.
- **Not done:** migrating the local `FCD`/`FCT` back-catalogue. Explicitly the group's own
  follow-on, per the policy text.
- **Not done:** moving or deleting the policy notice file from `Raw/`. It asks receiving KBs to
  "archive this file"; this KB's own, more specific rule that nothing is deleted or moved out of
  `Raw/` (`CLAUDE.md` §1) takes precedence for this KB's own files. It stays in place, logged as
  `skipped` (not source material) in `Outputs/kb-registers.md`.

## Open question

The access test used a placeholder row, not a real document. The next genuinely qualifying
document (a lease, loan document, board letter, etc. per the Processes article's list) is still
the first real use of the register end-to-end - registering it, filing the file in
Collaboration Space, and getting the row's `File link`/`Location` right.

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-09 | Write access confirmed | `Outputs/change-log-2026-09-09-group-document-numbering-write-access-confirmed.md` |
| 2026-09-09 | Created | `Outputs/change-log-2026-09-09-group-document-numbering-adopted.md` |
