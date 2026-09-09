# Change log - 2026-09-09 - Group Document Register: write access confirmed

## What was asked

Following adoption of the Fishbone Group's document-numbering policy (v1.1), which left write
access to the group Document Register as an open question, the owner asked: *"confirm write
access to the group Document Register."*

## What was done

Read access had already been confirmed at adoption time. To confirm write access without
registering a fake business document into a shared, cross-company register, a scripted
add-then-delete test was run directly against the Smartsheet:

1. `get_columns` on sheet `7352854736144260` to get exact column IDs.
2. `add_rows`: one row, clearly non-conforming to the real ID pattern so it could never be
   confused with a genuine document even if cleanup failed - `Document No. = TEST-ACCESS-CHECK`,
   `Entity (owner) = FC - Fishbone Construction Ltd`, `Direction = Internal`,
   `Status = Void`, and a `Description` stating plainly that it was an access test to be deleted
   immediately. **Succeeded** - row id `7595678077945732`.
3. `delete_rows` on that row id. **Succeeded.**
4. `get_sheet_summary` again to confirm the sheet was back to exactly its prior state.

**Result: both read and write access confirmed for this KB's connection.** Along the way, the
register was found to no longer be empty - Amfa Furniture Ltd had already added its own first
real row (`FA0000001`, a Companies House change-of-name certificate), explicitly noted on that
row as "First registration on the group Document Register (proof-of-concept end-to-end run)."
The test above added its row after that one and removed only its own, leaving Amfa's row
untouched.

## What was not done

- **No real document was registered.** The test used a placeholder explicitly marked `Void` and
  deleted within the same operation, not a real qualifying document. The next actual qualifying
  document is still this KB's first real end-to-end use of the register (see the Decisions
  article's open question).

## Files touched

Drive/git mirror: `Wiki/Processes/group-document-numbering-and-filing.md` and
`Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md` (both updated in place -
the "not yet tested" caveats replaced with the confirmation above), `CLAUDE.md` (replaced by
v6, one word changed in §1's live-data-sources table), `Outputs/kb-registers.md` (re-issued),
this file.

External (Smartsheet, not Drive): sheet `7352854736144260` ("Fishbone Group - Documents"
workspace) - one row added and deleted; net change to the sheet is none.
