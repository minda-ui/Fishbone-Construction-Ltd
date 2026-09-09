# Change log - 2026-09-09 - Group policy v1.2 adopted; FC-CR-0001 resolved (Accepted)

## What was asked

The owner asked: *"check /Raw folder."*

## What was found

Listing `Raw/` turned up a new arrival since this session's earlier work: `Raw/2026-09-09_group-
policy_document-numbering-and-filing-v1.2.md`, delivered by the Fishbone Group knowledge base
at 21:46 that day. It is the group's response to `FC-CR-0001` (the change request this KB
raised earlier the same day about the 14 task/email rows in the local `FCD` register). Nothing
else in `Raw/` (Email, Finance, FP 2401 Goathland Avenue, Vehicles subfolders) had changed
against what `Outputs/kb-registers.md`'s Processed items table already records.

Cross-checked the group's Document System - Change Requests sheet (Smartsheet, sheet
`8918834172004228`): the group had already updated the `FC-CR-0001` row itself - `Status =
Accepted`, `Reviewed (date) = 2026-09-09`, and a `Resolution / new version` field spelling out
the answer.

## What the resolution says

Two clarifications, both accepted into policy **v1.2**:

1. **Tasks are not documents (§6).** A task, to-do or action item - including an automation's
   own action list - gets no Document Register row and no document ID, whatever channel it
   arrived through. A document is registered only once a thread yields a verified business
   record (an actual stored file, or an email that is itself the record). This confirms the
   earlier decision not to migrate `FCD0000001`-`FCD0000014`.
2. **Each KB may migrate its own back-catalogue now (§11).** No need to wait for a group-run
   migration; migrate whenever ready, deduping on entry against the group register by `Source
   key` and by title + date + counterparty, and retire the local sheet once its live entries are
   migrated.

## What was done

**Adopted v1.2** into `Wiki/Processes/group-document-numbering-and-filing.md`: title and
front matter bumped to v1.2, the new §6 (tasks are not documents) and the updated Transition
section (§11, per-KB self-migration) written up, the `FC-CR-0001` section rewritten to record
the resolution, open questions cleared, and both policy files (`v1.1` and `v1.2`) listed under
Sources - both stay in `Raw/`, neither moved or deleted, per this KB's own Raw-immutability
rule outranking the group notice's generic "archive this file."

**Updated `Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md`** to match:
the back-catalogue section now records both the Change Request and its same-day resolution, and
the open question is closed.

**Worked out the net effect for this KB specifically:** with point (1) in force, there is
nothing left to migrate. The local Construction Document Register's back-catalogue outside the
MSEM case is exactly `FCD0000001`-`FCD0000014`, and all 14 are excluded as tasks under the new
rule - so point (2)'s permission to self-migrate has nothing to act on here. All 23 local `FCD`
rows are now accounted for: 9 as group documents (`FC0000001`-`FC0000009`), 14 correctly
excluded as tasks.

## What was not done

- **No further registration.** No new `FC` rows were added; the 14 local rows were not touched.
- **`FC-CR-0001`'s row was not edited by this KB** - the group had already updated it (Status,
  Resolution, Reviewed date) before this check; nothing needed correcting.
- **The rest of `Raw/` was checked but not reprocessed.** Its other subfolders (Email, Finance,
  FP 2401 Goathland Avenue, Vehicles) matched the existing Processed items table exactly; no new
  Detect-step work was triggered.

## Files touched

Smartsheet: none written to. Read only: group Document System - Change Requests sheet (sheet
`8918834172004228`), confirming the group's own update to `FC-CR-0001`.

Drive: `Raw/2026-09-09_group-policy_document-numbering-and-filing-v1.2.md` read; not moved, not
registered (policy notice, not a business document, per its own instructions and this KB's
Raw-immutability rule).

Drive/git mirror: `Wiki/Processes/group-document-numbering-and-filing.md` and
`Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md` updated (v1.2 adopted,
`FC-CR-0001` resolution recorded), `CLAUDE.md` (replaced by v9), `Outputs/kb-registers.md`
(re-issued), this file.
