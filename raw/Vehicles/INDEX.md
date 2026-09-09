# Raw file index - Vehicles

Register of the company's owned or leased vehicles and where their documents live. Per
`CLAUDE.md` §1, one subfolder per vehicle, named `<Make> <Model> - <REG> (<how it's held>)`.
Drop insurance certificates, MOT/inspection records, service invoices, tax reminders and the
like into the matching subfolder as they arrive. Documents that already have a home elsewhere
(a finance agreement filed in the group Loans database's `Raw/`) are **linked, not copied** -
see the note on each vehicle below.

**Status: 1 of 3 vehicles identified.** The owner said on 2026-09-09 that the company owns or
leases three vehicles. Bank-data and Loans-database checks confirmed one; the other two are
awaited. See `Outputs/change-log-2026-09-09-vehicle-workspace-created.md` for how the first was
found and why two bank-data candidates were ruled in/out.

## Vehicles

| Folder | Registration | How held | Status |
|---|---|---|---|
| `Ford Transit - HT22BWP (MotoNovo HP)/` | HT22BWP | Hire purchase, MotoNovo Finance | Confirmed |
| *(vehicle 2 - not yet identified)* | ? | ? | Awaiting owner |
| *(vehicle 3 - not yet identified)* | ? | ? | Awaiting owner |

## Ford Transit - HT22BWP (MotoNovo HP)

Ford Transit 350 L2 Diesel RWD, VIN WF0AXXTTRANT79444. On hire purchase with MotoNovo Finance
Limited, agreement 23193713, signed 28/05/2025: £459.80/month, 48 months, first payment
28/06/2025, final payment due 28/05/2029. MotoNovo owns the vehicle until the final payment.

**The signed HP agreement and the group's financial tracking of it are not duplicated here.**
They are the group Loans database's material and stay there:
- `Facility — MotoNovo Finance — Hire Purchase` (Loans database Wiki) - full terms, balance,
  and the reading caveats on the scanned agreement (a side-by-side table that didn't extract
  cleanly - see that page's Notes & Caveats before quoting any figure from the source PDF
  directly).
- `Raw/Motonovo Finance.pdf` (Loans database `Raw/`) - the signed agreement itself.

This folder is for what belongs to the vehicle rather than the finance: insurance certificate,
MOT history, service records, mileage, driver assignment, tax/SORN status.

## Ruled out from the bank-data search

Two other bank-data lines looked vehicle-shaped and were checked against the Loans database
before being trusted, per `CLAUDE.md` §0 (check the sister knowledge bases before concluding
anything about a counterparty).

- **Haydock Finance** (£1,210.16/month HP) is **not a vehicle** - it is three used woodworking
  machines (Altendorf panel saw, Vitap edgebander line, Hebrock edgebander), agreement 22 Jan
  2026. Confirmed from the Loans database's `Facility — Haydock Finance — Hire Purchase` page.
  A bank-statement pattern match alone would have put this wrongly in a vehicle register.
- **Tower Leasing** (£373, one payment, August statement only) has **no facility write-up
  anywhere** in the group Loans database. It may be vehicle 2 or 3, or it may be an equipment
  lease unrelated to vehicles - not established either way. Worth asking about directly rather
  than guessing from one bank line.

## Open questions

- What and where are vehicles 2 and 3?
- Is Tower Leasing one of them?
- Once all three are identified: is a Smartsheet fleet register wanted now, or held until
  documents are gathered? (Owner said "later" on 2026-09-09 - not created yet.)

---

Compiled 2026-09-09. See `Outputs/change-log-2026-09-09-vehicle-workspace-created.md`.
