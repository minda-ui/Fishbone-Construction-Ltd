# Change log - 2026-09-11 - Raw/ checked: vehicle MOT, and a group hand-off (HSE invoice, DVLA tax reminder)

## What was asked

The owner asked: *"check /Raw folder for new document."*

## What was found

Three new items since the last full `/Raw` check, beyond the Kosmosoft price-confirmation note
already processed earlier today:

1. **`Xerox Scan 20260911 145603.pdf`**, uploaded directly to `Raw/` (not via email), 2026-09-11.
   A two-part MOT record for a Ford Transit.
2. **`2026-09-10_handoff_group-to-construction_FC0000010-FC0000011.md`**, delivered by the
   Fishbone Group at 16:24 on 2026-09-10 - a §7a inter-KB hand-off of two documents the group
   received as paper post and already registered in its own Document Register.
3. **`2026-09-10_group-process_incoming-paper-mail-handling.md`**, delivered by the group at
   15:43 on 2026-09-10 - a notice explaining the new centralised paper-post procedure that
   produced item 2. Informational, not a business document.

Items 2 and 3 arrived during the previous session (which was scoped to `/Raw/Finance` only) and
had not yet been picked up - this full `/Raw` check is what found them.

## The MOT certificate: a safety defect found and cleared

Registered locally as **`FCD0000025`** (renamed in place to
`FCD0000025 - Vehicle - MOT test certificate and refusal notice (Ford Transit NJ17CYK).pdf`).

A Ford Transit (VIN `WFOZXXTTGZHU86918`, registration **`NJ17CYK`**) was tested on 08.07.2026 at
Advanced Wallsend Test Centre Ltd - a payee already appearing in `Raw/Finance/`. Two outcomes
from the same test date and mileage (185,741 miles):

- **Refused** first, for three **major** defects: road wheel fixings missing on the nearside
  front, offside front, and nearside rear.
- **Passed with defects** the same day, once represented, with only minor/advisory items left:
  registration-plate lamp inoperative, a non-excessive oil leak, a corroded brake pipe.

Read together, this is a vehicle that failed on a serious safety fault (wheels not properly
secured) and was fixed the same day. MOT now valid to 07.07.2027.

## The group hand-off: FC0000010 and FC0000011

Per the group's §7a rule, both IDs were **reused, not re-numbered** locally:

- **FC0000010** - an HSE Fee for Intervention invoice, £1,428.80 (7.6 hrs @ £188/hr), invoice
  date 3 Sep 2026, **due 3 Oct 2026**. Issued via Shared Services Connected Ltd, re a
  Notification of Contravention and material breaches arising from an incident on 10 July 2025
  at The Burlington, 124 New Street, Birmingham. This is the **same investigation** already
  tracked as `FCT00008`/`FCD0000008` (DWF Law LLP acts for Fishbone on it, per `FCT00015`) -
  updated that task with the invoice detail and moved its Due Date to 3 Oct 2026, rather than
  creating a duplicate task.
- **FC0000011** - a DVLA V11 vehicle tax reminder, registration **`NJ17 CWK`**, Ford, Light
  Goods Vehicle, 1995cc, **tax expires 30 Sep 2026**, needs a valid MOT to re-tax. Addressed to
  Fishbone Drylining Ltd (the former company name). No existing task covered this - opened
  **`FCT00020`**.

## The registration discrepancy

`NJ17CYK` (MOT certificate, a direct scan) and `NJ17 CWK` (DVLA reminder, transcribed by the
group's post-handling process before reaching this KB) differ by one letter. Both are Fords.
Neither is this KB's own transcription of the other, so there's no way to tell from these two
documents alone whether it's the same vehicle read two different ways, or two distinct
vehicles. **Not guessed** - flagged as the lead open question on `Wiki/Assets/vehicles.md` and
noted on `FCT00020`, with a suggestion to check the V5C or insurance schedule. Whichever
registration is correct, the vehicle needs re-taxing before 30 September 2026 and has a valid
MOT to do so.

## What was done

- Registered `FCD0000025` in the local Construction Document Register (Smartsheet, sheet
  `258807861217156`); renamed the Drive file to match.
- Updated `FCT00008` (Smartsheet Tasks, sheet `5235584035587972`) with the FC0000010 invoice
  detail and moved its Due Date to 3 Oct 2026.
- Opened `FCT00020` for the FC0000011 DVLA tax reminder, due 30 Sep 2026.
- Updated `Wiki/Assets/vehicles.md`: added the second-vehicle findings, the registration
  discrepancy as the top open question, and cross-references to `FCD0000025`, `FC0000011` and
  `FCT00020`.
- Registered all three new `Raw/` items in `Outputs/kb-registers.md`'s Processed items table.

## What was not done

- **No payment made or authorised** for the HSE invoice (£1,428.80, due 3 Oct 2026). Per
  `CLAUDE.md` §6a this is an owner decision; DWF Law LLP (the instructed solicitor on this
  matter) may also want to be consulted, and the invoice's own 21-day query window is worth
  noting to the owner.
- **No DVLA contact, taxing or SORN action** for the vehicle tax reminder (due 30 Sep 2026).
  Same governance reason, and the registration discrepancy should be resolved first regardless.
- **The registration discrepancy was not resolved by guessing.** Neither `NJ17CYK` nor
  `NJ17 CWK` was picked as "the real one."
- **`Raw/2026-09-10_group-process_incoming-paper-mail-handling.md` was not written up as a Wiki
  article** - it's a process notice, handled the same way earlier group policy notices were
  (registered `skipped`, understood and applied, not separately documented in the Wiki beyond
  this change log).
- **No group-register writes.** Both FC0000010 and FC0000011 were already registered by the
  group before this KB saw them; nothing new was added to the shared register.
- **`CLAUDE.md` was not replaced.** Nothing in its live-data-sources table changed; this is
  Raw-item processing under the existing rules, not a structural change (§6c).

## Files touched

Smartsheet: Construction Document Register (sheet `258807861217156`) - one row added
(`FCD0000025`). Tasks (sheet `5235584035587972`) - `FCT00008` updated, `FCT00020` added.

Drive: `Xerox Scan 20260911 145603.pdf` renamed to
`FCD0000025 - Vehicle - MOT test certificate and refusal notice (Ford Transit NJ17CYK).pdf`
(same file id, not moved). The two group notices read, not moved or altered.

Drive/git mirror: `Wiki/Assets/vehicles.md` updated, `Outputs/kb-registers.md` re-issued, this
file.
