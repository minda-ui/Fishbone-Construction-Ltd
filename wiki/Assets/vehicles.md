---
title: Vehicles
category: Assets
status: draft
sensitive: false
created: 2026-09-09
updated: 2026-09-11
sources:
  - ../../Raw/Vehicles/INDEX.md
  - ../../raw/FCD0000025 - Vehicle - MOT test certificate and refusal notice (Ford Transit NJ17CYK).pdf
  - ../../raw/2026-09-10_handoff_group-to-construction_FC0000010-FC0000011.md
related:
  - ../Finance/debt-service.md
---

# Vehicles

The company owns or leases three vehicles (owner statement, 2026-09-09). One is confirmed and
documented; two are not yet identified. `draft` until all three are on record.

## Key facts

| Item | Value | Source |
|---|---|---|
| Vehicles, per owner | 3 | [^1] |
| Confirmed | 1 - Ford Transit, HT22BWP | [^2] |
| Held on hire purchase | MotoNovo Finance, 48 months, £459.80/mo | [^2] |
| Documents | `Raw/Vehicles/` on Drive, one subfolder per vehicle | - |
| Fleet register | Not yet built. Smartsheet, once all three vehicles and their documents are in | - |

## Details

### Ford Transit - HT22BWP

Ford Transit 350 L2 Diesel RWD, on hire purchase with MotoNovo Finance Limited since 28 May
2025 (agreement 23193713): £459.80 a month for 48 months, final payment due 28 May 2029.
MotoNovo owns the vehicle until the agreement completes.

Full terms, the balance, and the reading caveats on the source agreement (a page that didn't
extract cleanly from a scanned PDF) live in the group Loans database, which is authoritative on
lending per `CLAUDE.md` §1 - see `Facility — MotoNovo Finance — Hire Purchase`. This article
does not repeat the finance terms; it is the entry point for everything about the vehicle
itself once documents arrive: insurance, MOT history, service record, mileage, driver.

### Vehicles 2 and 3

Not yet fully identified. Two candidates were checked in the bank statements and one was ruled
out:

- **Haydock Finance** (£1,210.16/month HP) looked vehicle-shaped from the payment pattern alone
  but is **three woodworking machines**, confirmed against the Loans database. Not a vehicle.
- **Tower Leasing** (£373, appearing once, August 2026 only) has no facility record anywhere in
  the group Loans database. It may be a vehicle or may be unrelated equipment - unconfirmed.

**A second Ford Transit is now documented, but its registration is unresolved.** Two documents
arrived the same week (2026-09-10/11) naming what looks like the same vehicle under two
different plates:

- **MOT record, registration `NJ17CYK`** (`FCD0000025`, a scanned certificate uploaded directly
  to `Raw/`). Ford Transit, VIN `WFOZXXTTGZHU86918`. Test on 08.07.2026 at Advanced Wallsend
  Test Centre Ltd (3 Bewicke Road Industrial Estate, Wallsend - a bank payee already appearing
  in `Raw/Finance/`), mileage 185,741. **Initially refused** for three major defects - road
  wheel fixings missing on the nearside front, offside front and nearside rear - then
  represented and **passed the same day with defects**: registration-plate lamp inoperative
  (advisory), a non-excessive oil leak, and a corroded brake pipe. MOT expiry 07.07.2027.
- **DVLA vehicle tax reminder (V11), registration `NJ17 CWK`** (group Document Register
  `FC0000011`, handed to this KB via `Raw/2026-09-10_handoff_group-to-construction_FC0000010-
  FC0000011.md`, a §7a inter-KB receipt). Ford, Light Goods Vehicle, 1995cc. Tax expires 30
  September 2026; needs a valid MOT to re-tax. Addressed to Fishbone Drylining Ltd (the
  company's former name). Tax reference `1276 5121 6874 0040`.

The two registrations differ by one letter (`CYK` vs `CWK`) and neither source is this KB's own
transcription of the other - the MOT certificate is a direct scan, and the DVLA reminder's plate
was transcribed by the group's post-handling process before reaching this KB. **Not resolved
whether this is one vehicle read two different ways, or two distinct vehicles.** Not guessed.

Full detail: `Raw/Vehicles/INDEX.md`.

## Open questions

- **Is `NJ17CYK` (MOT) the same vehicle as `NJ17 CWK` (DVLA tax reminder), or two vehicles?**
  Check against the V5C registration certificate or the insurance schedule before treating
  either reading as correct. Whichever it resolves to, the vehicle needs re-taxing before
  30 September 2026 (it has a valid MOT to do so, expiry 07.07.2027).
- What and where is the (possible) third vehicle?
- Is the Tower Leasing payment one of them?
- Insurer and current keeper/finance arrangement for the second vehicle - not established from
  the MOT certificate or tax reminder alone (unlike vehicle 1, no hire-purchase facility for it
  has yet been found in the group Loans database).
- Whether the Haydock woodworking machines (correctly excluded from this vehicle article)
  deserve their own `Assets/` article as equipment rather than staying undocumented outside the
  Loans database.

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-11 | Second vehicle (Ford Transit) added from an MOT certificate and a DVLA tax reminder; registration discrepancy flagged, not resolved | `Outputs/change-log-2026-09-11-raw-check-vehicle-and-hse-handoff.md` |
| 2026-09-09 | Created; workspace set up, one of three vehicles confirmed | `Outputs/change-log-2026-09-09-vehicle-workspace-created.md` |

## Sources

[^1]: Owner statement, 2026-09-09 (conversational; not yet written up as a dated `Raw/` note - see Decisions article).
[^2]: `Facility — MotoNovo Finance — Hire Purchase`, group Loans database Wiki, last updated 04/09/2026.
