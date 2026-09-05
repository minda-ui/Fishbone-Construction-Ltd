---
title: FP 2401 - 131 Goathland Avenue
category: Projects
status: active
sensitive: false
created: 2026-09-05
updated: 2026-09-05
sources:
  - ../../Raw/FP 2401_131 Goathland Avenue/INDEX.md
related:
  - ../Suppliers/trade-suppliers.md
  - ../Suppliers/subcontractors.md
  - ../Processes/data-capture-and-accounting-systems.md
---

# FP 2401 - 131 Goathland Avenue

The only project with a documented cost file in this knowledge base. 99 supplier documents
covering 16 April to 24 August 2026 have been processed into the Smartsheet Classifier and the
FP 2401 Budget, and re-read on 2026-09-05 to identify each one's supplier.

## Key facts

| Item | Value | Source |
|---|---|---|
| Project code | FP 2401 | [^1] |
| Raw documents held | 99, in 8 supplier subfolders | [^1] |
| Document date range | 16 Apr 2026 to 24 Aug 2026 | [^1] |
| Suppliers | 15 | [^1] |
| Processed into Classifier and Budget | 2026-08-25, batch marked COMPLETE | [^2] |
| Classifier codes added | approximately 40 | [^2] |
| Budget sheet size | approximately 380 rows | [^2] |
| Smartsheet Budget | `FP 2401_Budget`, sheet id 8653045758035844 | [^3] |
| Smartsheet Classifier (all projects) | `Сlassifier` (Cyrillic С), sheet id 6344783272478596 | [^3] |

## Details

### Scope, as far as the invoices show it

There is no scope document, drawing, contract or programme in `Raw/`. What the project involves
has to be inferred from what was bought, which points to a full residential refurbishment:

- **Structure and shell** - steel (NT Steel), timber and CLS (Quay Timber, B&Q), partitioning
  (SP Partitions)
- **Drylining** - plasterboard, metal stud, MF ceiling, insulation, jointing compound (Galaxy
  Insulation, in seven deliveries through June and July)
- **Plumbing and heating** - a Baxi 30kW combi boiler with flue and Magnaclean, copper tube,
  solder-ring and push-fit fittings (JT Dove); bathroom sanitaryware, shower bath, wall-hung WC
  and basin frames (Victorian Plumbing)
- **Electrical** - consumer units (CEF, Consumer Unit World), MCBs (YESSS), cable, sockets and
  switches (Screwfix)
- **Finishes** - Dulux primer and vinyl matt (J P McDougall), stair nosings (Lilley Tile),
  architrave and trims (National Plastics), door furniture and hinges (IronmongeryDirect)

Two second-floor bathrooms or similar are implied by items bought in twos - two wall-hung WC
frames, two basin frames, two basins.

### Cost data

The invoices were processed into actual rates on 2026-08-25. The methodology is recorded in the
closed Change Log and in the session-starter document, and matters for anyone auditing the
figures:

- JT Dove invoices show ex-VAT prices directly, verified against printed Goods/VAT totals.
- Screwfix classic invoices print a **gross** unit price; the Net column was used.
- Screwfix order-history screenshots state values inclusive of VAT; ex-VAT was computed as
  gross / 1.2, and where a whole-order discount applied each line's share was estimated
  proportionally by list price and **flagged as estimated** in the Budget notes.
- Some B&Q mixed-basket receipts required the same proportional estimation.

Solder-ring and push-fit plumbing fittings are kept as **distinct Classifier codes** on the
owner's instruction (M16-009/M16-014 against M16-036/037). Apply that consistently.

### Housekeeping already done

- Two Screwfix orders carrying reference **FC2522** were confirmed as a different project and
  removed from this folder on 2026-08-25.
- One JT Dove invoice (fence posts) was removed as wrong project.
- One Screwfix order under reference **Fc2518**, on a second director's card, was confirmed as
  legitimate spend on this project.
- A fabricated Budget entry against M17-012 (13A 2-gang socket) was written in error on
  2026-08-25 and reverted to blank before the session ended. No bad data remains for that code.

### The file organisation

Until 2026-09-05 all 99 documents sat in one flat folder, 91 of them named only by their Dext
transaction id. They are now in eight supplier subfolders with
[`INDEX.md`](../../Raw/FP%202401_131%20Goathland%20Avenue/INDEX.md) recording each file's
supplier and document date. **Filenames were deliberately not changed** - the Dext id is the
link back to Dext and to the Budget and Classifier notes.

## Open questions

- **What and where is the project?** No client, contract, scope, programme or value is recorded
  anywhere in this knowledge base. "131 Goathland Avenue" is an address in the project name and
  nothing more.
- Is it complete? The last document is 24 August 2026.
- **Is it profitable?** The Budget sheet holds plan and actual rates, but no comparison has been
  drawn into this knowledge base, and the owner's own view recorded on 2026-09-04 was that
  negative margins are real and jobs are underpriced. This project is the one place where that
  could actually be tested against data.
- Who is the customer? If it is [Macdonald Joinery](../Customers/macdonald-joinery.md), the
  project's completion may be the explanation for the May payment collapse - but nothing links
  them.
- What are the FP project codes generally? FC2518, FC2522, FC2603, FC2604, FC2605, FC0204,
  FC0207, FC0210 and others appear on bank lines and invoices. No register of them exists here.

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-05 | Created; Raw folder reorganised into supplier subfolders | `Outputs/change-log-2026-09-05-kb-skeleton-and-raw-tidy.md` |

## Sources

[^1]: [`Raw/FP 2401_131 Goathland Avenue/INDEX.md`](../../Raw/FP%202401_131%20Goathland%20Avenue/INDEX.md), compiled 2026-09-05 by reading all 99 documents.
[^2]: `Wiki/Change Log` (closed), entries dated 2026-08-25.
[^3]: `Wiki/FP 2401 Goathland Avenue - Actuals Processing Instructions`, re-issued 2026-09-05.
