# Change log - 2026-09-09 - MSEM court case: remaining documents registered in the group Document Register

## What was asked

Following the first real group-register registration (`FC0000001`, the MSEM claim form), the
owner explicitly asked: *"register FCD0000015–FCD0000023."* This overrides the deliberate scope
limit recorded in `Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md` and
`Wiki/Processes/group-document-numbering-and-filing.md` (only the claim form registered
initially) - the owner has now asked for the rest of that case's local documents to be
cross-registered too.

## What was done

**Scope.** Of `FCD0000015`-`FCD0000023` (9 local IDs), `FCD0000018` was already registered as
`FC0000001` in the prior session. The remaining 8 - `FCD0000015, 016, 017, 019, 020, 021, 022,
023` - were registered this session as `FC0000002` through `FC0000009`, in ascending local-ID
order.

**Dedup-on-entry.** Checked the group register's current state before minting anything: exactly
2 rows (`FA0000001`, `FC0000001`), no collision.

**Filed.** Two of the 8 documents (`FCD0000015`, `FCD0000016`) are physically in this KB's own
`Raw/` folder; the other 6 already live in Collaboration Space
(`Fishbone Construction / C Legal & Court Cases / MSEM UK Ltd Claim – BBC Cardiff/`). Consistent
with the `FC0000001` precedent and this KB's own Raw-immutability rule (`CLAUDE.md` §1) taking
precedence over the group policy's generic Collaboration Space filing convention, the two `Raw/`
files were **renamed in place**, not moved, and the six Collaboration Space files were renamed
in place too (all same Drive file ids, so no links break):

| Local ID | Group ID | Renamed to | Location |
|---|---|---|---|
| FCD0000015 | FC0000002 | `FC0000002 - Legal - Notice of Trial Date and Allocation (claim 019JE538).pdf` | `Raw/` (this KB) |
| FCD0000016 | FC0000003 | `FC0000003 - Legal - Claimant's N180 Directions Questionnaire (claim 019JE538).pdf` | `Raw/` (this KB) |
| FCD0000017 | FC0000004 | `FC0000004 - Legal - Chronology of Events (claim 019JE538).pdf` | Collaboration Space |
| FCD0000019 | FC0000005 | `FC0000005 - Legal - BBC C010 Timesheet, MSEM Invoice 554 backing (claim 019JE538).ods` | Collaboration Space |
| FCD0000020 | FC0000006 | `FC0000006 - Legal - Correspondence with MSEM UK Ltd, 6-27 March 2026 (claim 019JE538).docx` | Collaboration Space |
| FCD0000021 | FC0000007 | `FC0000007 - Legal - Court correspondence (claim 019JE538).pdf` | Collaboration Space |
| FCD0000022 | FC0000008 | `FC0000008 - Legal - N9B Defence and Counterclaim (claim 019JE538).pdf` | Collaboration Space |
| FCD0000023 | FC0000009 | `FC0000009 - Legal - Fishbone's N180 Directions Questionnaire, signed (claim 019JE538).pdf` | Collaboration Space |

**Registered.** Added rows `FC0000002`-`FC0000009` to the group Document Register, each with
`Entity = FC - Fishbone Construction Ltd`, `Status = Issued`, `Source key` = the Drive file id,
and a `Description` cross-referencing the local `FCD` number, `FC0000001`, and the other new
rows.

**Two deliberate omissions from the shared descriptions**, both flagged in the source data
during this session:
- `FC0000003` (from `FCD0000016`): the claimant's individual contact's home address, present in
  the local description, was **not** copied into the group register - personal-data
  minimisation, same practice as `FC0000001`.
- `FC0000007` (from `FCD0000021`): the underlying document contains a **live Money Claims Online
  security/access code**. This is a credential, not just personal data, and was **not** copied
  into a register shared across seven companies. Both omissions are noted explicitly on the
  group-register rows themselves and on the corresponding local rows, so a reader is told the
  detail exists and where it lives, not left to wonder why the field looks short.

**Cross-referenced back.** Updated all 8 local `FCD` rows' descriptions to note the new `FC`
number and the rename, mirroring the pattern already applied to `FCD0000018`. One correction
surfaced in the process: `FCD0000023`'s local description said the file was "found loose in
Minda's Downloads folder... copied... for consolidation" - live Drive metadata confirmed it is
now filed in Collaboration Space, so the local row's cross-reference notes the file is
**confirmed filed there**, not still pending.

**No new Wiki article.** Same reasoning as `FC0000001`: this case is tracked in
Tasks/Document Register only, kept out of the Wiki, consistent with this KB's established
handling of sensitive live litigation.

## What was not done

- **No content or response was filed with the court, and no contact was made** with MSEM, its
  contact, or the court. Registration and filing only.
- **The claimant's home address and the Money Claims Online security code were not copied
  anywhere new** - not into the group register, not into this change-log entry, not into any
  Wiki article. This entry names that they exist and where (the local `FCD0000016`/`FCD0000021`
  rows and their underlying documents), without repeating them.
- **The local `FCD`/`FCT` back-catalogue migration was not run.** Only this one case's remaining
  documents were registered, per the explicit instruction; the group's own back-catalogue
  migration (all other local `FCD` documents, and any other company's) remains untouched.

## Files touched

Smartsheet: group Document Register (sheet `7352854736144260`) - 8 rows added (`FC0000002`-
`FC0000009`); local Construction Document Register (sheet `258807861217156`) - 8 rows' `Description`
fields updated (`FCD0000015`, `016`, `017`, `019`, `020`, `021`, `022`, `023`).

Drive: 8 files renamed in place (same file ids throughout) - 2 in this KB's `Raw/`, 6 in
Collaboration Space's `MSEM UK Ltd Claim – BBC Cardiff` folder.

Drive/git mirror: `Wiki/Processes/group-document-numbering-and-filing.md` and
`Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md` updated (the prior
"deliberate limit" note now recorded as superseded by this instruction), `CLAUDE.md` (replaced
by v8), `Outputs/kb-registers.md` (re-issued), this file.
