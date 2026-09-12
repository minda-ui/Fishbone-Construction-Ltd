---
title: Vehicles
category: Assets
status: draft
sensitive: false
created: 2026-09-09
updated: 2026-09-12
sources:
  - ../../Raw/Vehicles/INDEX.md
  - ../../raw/FCD0000025 - Vehicle - MOT test certificate and refusal notice (Ford Transit NJ17CYK).pdf
  - ../../raw/2026-09-10_handoff_group-to-construction_FC0000010-FC0000011.md
  - ../../raw/2026-09-12_owner-note_vehicle-fct00020-confirmed-company-van.md
  - ../../raw/2026-09-12_owner-note_two-vans-two-plates-confirmed.md
related:
  - ../Finance/debt-service.md
---

# Vehicles

The company owns or leases three vehicles (owner statement, 2026-09-09), and all three are now
identified by registration: Ford Transit `HT22BWP`, Ford Transit `NJ17CYK`, Ford Transit
`NJ17CWK`. `draft` until insurance, keeper and finance detail for the two Transits confirmed on
2026-09-12 are on record.

## Key facts

| Item | Value | Source |
|---|---|---|
| Vehicles, per owner | 3 | [^1] |
| Confirmed | 3 - Ford Transit HT22BWP; Ford Transit NJ17CYK; Ford Transit NJ17CWK | [^2] [^3] [^4] |
| Held on hire purchase | MotoNovo Finance, 48 months, £459.80/mo (HT22BWP only; no facility yet found for the other two) | [^2] |
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

### Ford Transit - NJ17CYK

**Confirmed as one of the two remaining company vans by the owner on 2026-09-12** (see
Confirmation history below). MOT record: `FCD0000025`, a scanned certificate uploaded directly
to `Raw/`. Ford Transit, VIN `WFOZXXTTGZHU86918`. Test on 08.07.2026 at Advanced Wallsend Test
Centre Ltd (3 Bewicke Road Industrial Estate, Wallsend - a bank payee already appearing in
`Raw/Finance/`), mileage 185,741. **Initially refused** for three major defects - road wheel
fixings missing on the nearside front, offside front and nearside rear - then represented and
**passed the same day with defects**: registration-plate lamp inoperative (advisory), a
non-excessive oil leak, and a corroded brake pipe. MOT expiry 07.07.2027. Tax status not
established - no DVLA reminder for this registration has arrived in `Raw/`.

### Ford Transit - NJ17CWK

**Confirmed as the other remaining company van by the owner on 2026-09-12.** DVLA vehicle tax
reminder (V11): group Document Register `FC0000011`, handed to this KB via
`Raw/2026-09-10_handoff_group-to-construction_FC0000010-FC0000011.md`, a §7a inter-KB receipt;
tracked locally as `FCT00020`. Ford, Light Goods Vehicle, 1995cc. **Tax expires 30 September
2026**; needs a valid MOT to re-tax - none is on file for this specific registration in `Raw/`
(the MOT above is for `NJ17CYK`, a different vehicle). Addressed to Fishbone Drylining Ltd (the
company's former name). Tax reference `1276 5121 6874 0040`. The DVLA letter printed the
registration with a space (`NJ17 CWK`); the owner's own statement (below) did not use one -
not treated as a substantive difference.

### Confirmation history for NJ17CYK and NJ17CWK

The two registrations differ by one letter (`CYK` vs `CWK`) and arrived on two unconnected
documents (a direct MOT scan and a DVLA reminder transcribed by the group's post-handling
process), so this KB could not tell from the documents alone whether they named one vehicle or
two - flagged as an open question rather than guessed. The owner resolved it in two steps on
2026-09-12:

1. First (`Raw/2026-09-12_owner-note_vehicle-fct00020-confirmed-company-van.md`): "This is one
   of our company vans. No issues with registration plate number" - referring to `FCT00020`.
   Read at the time as confirming one genuine vehicle with an unresolved plate spelling.
2. Later the same day (`Raw/2026-09-12_owner-note_two-vans-two-plates-confirmed.md`): "We have
   two vans which reg plate have letter difference. NJ17CWK and NJ17CYK" - **superseding
   reading 1**. Both registrations are correct; each names a distinct company van. This also
   fully accounts for the three vehicles the owner named on 2026-09-09.

Insurer, keeper and finance arrangement for both vehicles remain unconfirmed - no hire-purchase
facility for either has been found in the group Loans database, unlike `HT22BWP`.

Full detail: `Raw/Vehicles/INDEX.md`.

### Vehicles previously considered for "vehicle 3" (superseded)

Before the owner's 2026-09-12 clarification, `NJ17CWK` and `NJ17CYK` were suspected to be one
vehicle, leaving a third vehicle unidentified. Two payment-pattern candidates were checked
against the bank statements at that time and are kept here for the record, now that identity is
no longer in question:

- **Haydock Finance** (£1,210.16/month HP) looked vehicle-shaped from the payment pattern alone
  but is **three woodworking machines**, confirmed against the Loans database. Not a vehicle;
  not one of the company's three.
- **Tower Leasing** (£373, appearing once, August 2026 only) has no facility record anywhere in
  the group Loans database and is not one of the three named vehicles. What it paid for is
  still unexplained - kept as a separate open question below, unconnected to vehicle identity.

## Open questions

~~**Is `NJ17CYK` (MOT) the same vehicle as `NJ17 CWK` (DVLA tax reminder), or two vehicles?**
Check against the V5C registration certificate or the insurance schedule before treating either
reading as correct.~~ ~~**Answered 2026-09-12: it's one vehicle, a genuine company van** - the
owner confirmed there's no registration issue. Kept visible per `CLAUDE.md` §6d rule 2. Still
open: which of the two transcribed plates is spelled correctly.~~ **Corrected 2026-09-12, later
the same day: these are two vehicles, not one** - the owner clarified: "We have two vans which
reg plate have letter difference. NJ17CWK and NJ17CYK"
(`Raw/2026-09-12_owner-note_two-vans-two-plates-confirmed.md`). Both plates are correct; each
names a distinct company van. The earlier same-day "one vehicle" answer above is superseded,
not deleted, per `CLAUDE.md` §6d rule 2. All three of the owner's stated vehicles are now
identified: `HT22BWP`, `NJ17CYK`, `NJ17CWK`.
- **`NJ17CWK` needs re-taxing before 30 September 2026** - it has no MOT on file in `Raw/` yet
  (only `NJ17CYK` does, expiry 07.07.2027); confirm `NJ17CWK` has a valid MOT before DVLA will
  accept tax renewal.
- Insurer and current keeper/finance arrangement for `NJ17CYK` and `NJ17CWK` - not established
  from the MOT certificate or tax reminder alone (unlike `HT22BWP`, no hire-purchase facility
  for either has yet been found in the group Loans database).
- **What was the Tower Leasing payment (£373, August 2026 only) for**, if not a vehicle? No
  longer relevant to vehicle identity (all three are named), but still unexplained.
- Whether the Haydock woodworking machines (correctly excluded from this vehicle article)
  deserve their own `Assets/` article as equipment rather than staying undocumented outside the
  Loans database.

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-12 | Corrected: `NJ17CYK` and `NJ17CWK` are two vehicles, not one - all three of the owner's vehicles now identified | `Outputs/change-log-2026-09-12-vehicle-confirmed-company-van-addendum.md` |
| 2026-09-12 | Second vehicle confirmed as a genuine company van by the owner; registration-discrepancy question narrowed (one vehicle, exact plate spelling still open) - **superseded the same day, see row above** | `Outputs/change-log-2026-09-12-vehicle-confirmed-company-van.md` |
| 2026-09-11 | Second vehicle (Ford Transit) added from an MOT certificate and a DVLA tax reminder; registration discrepancy flagged, not resolved | `Outputs/change-log-2026-09-11-raw-check-vehicle-and-hse-handoff.md` |
| 2026-09-09 | Created; workspace set up, one of three vehicles confirmed | `Outputs/change-log-2026-09-09-vehicle-workspace-created.md` |

## Sources

[^1]: Owner statement, 2026-09-09 (conversational; not yet written up as a dated `Raw/` note - see Decisions article).
[^2]: `Facility — MotoNovo Finance — Hire Purchase`, group Loans database Wiki, last updated 04/09/2026.
[^3]: Owner statement, 2026-09-12 - `Raw/2026-09-12_owner-note_vehicle-fct00020-confirmed-company-van.md`.
[^4]: Owner statement, 2026-09-12 - `Raw/2026-09-12_owner-note_two-vans-two-plates-confirmed.md`.
