# Change log - 2026-09-12 - Addendum: two vans, two plates, both correct

## What was asked

Later the same day as the entry this addends
(`Outputs/change-log-2026-09-12-vehicle-confirmed-company-van.md`), the owner said, unprompted:

> "We have two vans which reg plate have letter difference. NJ17CWK and NJ17CYK"

## What this corrects

That earlier entry recorded the owner's statement on `FCT00020` ("This is one of our company
vans. No issues with registration plate number") as settling that `NJ17CYK` (MOT certificate)
and `NJ17 CWK` (DVLA tax reminder) are **one vehicle**, with only the exact plate spelling left
open. **That reading was wrong.** The owner's follow-up makes clear these are **two vehicles**,
one for each registration - not one vehicle with an uncertain spelling.

Per `CLAUDE.md` §4 ("if something in a past entry turns out to be wrong, write a new entry that
references it - never go back and change the old one") and §6d rule 2 (retract in place, never
delete a claim that was believed), the earlier entry is left untouched; this entry is the
correction on record.

## What was done

- Wrote up the owner's statement as `Raw/2026-09-12_owner-note_two-vans-two-plates-confirmed.md`.
- **Rewrote `Wiki/Assets/vehicles.md`**: split the single "second van" section into two
  distinct vehicle sections (`NJ17CYK`, `NJ17CWK`), added a "Confirmation history" section
  showing both of the owner's statements and which superseded which, corrected the Key facts
  table to 3 of 3 vehicles confirmed, and corrected the Open questions section in place (the
  earlier "one vehicle, spelling open" answer is struck through and marked superseded, not
  deleted).
- Updated `FCT00020` (Smartsheet Tasks): retitled to reflect that `NJ17CWK` is a confirmed,
  separate vehicle from `NJ17CYK`; Notes appended.
- Updated `FCD0000025` (Construction Document Register): Description corrected to state that
  its MOT is for `NJ17CYK` specifically, a vehicle distinct from `NJ17CWK`.

## What was not done

- **Still no DVLA contact, taxing or SORN action for `NJ17CWK`** (tax due 30 September 2026).
  Per `CLAUDE.md` §6a this remains an owner decision, and `NJ17CWK` still has no MOT of its own
  on file in `Raw/` (the MOT on file is for `NJ17CYK`).
- **No new task opened for `NJ17CYK`'s tax status.** Nothing in `Raw/` currently raises it as
  an item needing action; not invented.
- **The HSE invoice (`FC0000010`/`FCT00008`) is untouched** - unrelated to this correction.
- **`CLAUDE.md` was not replaced.** Not a structural change (§6c).

## Files touched

Smartsheet: Tasks (sheet `5235584035587972`) - `FCT00020` updated. Construction Document
Register (sheet `258807861217156`) - `FCD0000025` description updated.

Drive: `Raw/2026-09-12_owner-note_two-vans-two-plates-confirmed.md` created.

Drive/git mirror: `Wiki/Assets/vehicles.md` updated, `Outputs/kb-registers.md` re-issued, this
file.
