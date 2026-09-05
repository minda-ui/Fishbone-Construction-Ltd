---
title: Trade suppliers
category: Suppliers
status: active
sensitive: false
created: 2026-09-05
updated: 2026-09-05
sources:
  - ../../Raw/FP 2401_131 Goathland Avenue/INDEX.md
  - ../../Raw/Finance/20260321_04212819.csv
  - ../../Raw/Finance/20260821_04212819.csv
related:
  - ../Suppliers/subcontractors.md
  - ../Projects/fp-2401-goathland-avenue.md
  - ../Finance/funding-circle-flexipay.md
---

# Trade suppliers

Materials and merchant accounts. **£59,381 over the six months to 21 August 2026**, across
fifteen identified suppliers. Small relative to subcontract labour, but it is where the
company's project cost data comes from: every rate in the Smartsheet Classifier traces back to
one of these invoices.

## Key facts

| Item | Value | Source |
|---|---|---|
| Materials and supplies, six months to 21 Aug 2026 | £59,381 | [^1] |
| Suppliers identified from the Goathland invoice batch | 15 | [^2] |
| Largest by document count | Screwfix and Plumbfix, 68 of 99 documents | [^2] |
| Largest by bank spend | Screwfix, £10,305 over six months | [^1] |
| Accounts still in the former company name | at least 3 | [^2] |

## Details

### The supplier base

Fifteen suppliers were identified by reading all 99 documents in the FP 2401 Goathland Avenue
invoice batch on 2026-09-05. The full file-level index is
[`Raw/FP 2401_131 Goathland Avenue/INDEX.md`](../../Raw/FP%202401_131%20Goathland%20Avenue/INDEX.md).

| Supplier | Documents | What they supply |
|---|---:|---|
| Screwfix / Plumbfix | 68 | General consumables, plumbing and electrical fittings, tools |
| B&Q Trade Point (North Shields) | 7 | Ad-hoc timber, fixings, sundries; till receipts |
| Galaxy Insulation and Dry Lining | 7 | Plasterboard, insulation, metal stud, jointing compound. Account FIS003 |
| Victorian Plumbing | 3 | Bathroom sanitaryware and frames |
| Consumer Unit World | 2 | Consumer units and distribution gear |
| JT Dove | 2 | Boilers, copper tube, plumbing and heating |
| YESSS Electrical (Tyne Tunnel) | 2 | MCBs and consumer-unit components |
| CEF (City Electrical Factors) | 1 | Consumer unit. Account 18577770 |
| IronmongeryDirect | 1 | Door furniture, hinges, seals |
| J P McDougall (Dulux Decorator Centre) | 1 | Paint and primer. Account 3618466 |
| Lilley Tile and Stone | 1 | Stair nosings |
| National Plastics | 1 | Trims, architrave, angle |
| NT Steel Services | 1 | Steel |
| Quay Timber | 1 | Timber |
| SP Partitions | 1 | Partitioning |

The bank statements also show spend with **James Latham** (£6,053), **Interfit** (£3,389),
**Unilin Flooring** (£2,906), **Loxone** (£2,609), **MKM Building Supplies**, **Wolseley**,
**ITS** and **R&J Machinery** that does not appear in the Goathland batch - so the supplier base
is wider than that one project's invoice file.

### Concentration is in document count, not value

Screwfix accounts for 69% of the documents but only 17% of six-month materials spend. It is
many small purchases; the larger single-invoice suppliers (JT Dove's £1,788 boiler package,
Galaxy's board and insulation deliveries, James Latham's timber) carry more value per document.
That matters for processing effort: most of the reading time goes on the smallest spend.

### Accounts still in the former company name

Screwfix, Consumer Unit World and IronmongeryDirect all still bill **Fishbone Drylining Ltd**
or "FISHBONE DRY LINING", the name the company traded under before 31 October 2024. One
Consumer Unit World order was sent to `minda@fishbonedrylining.co.uk`.

This is the same trap that caused a misreading of the bank statements on 2026-09-04, where
drawdowns on the company's own facility were counted as income from a sister company - see
[Funding Circle FlexiPay](../Finance/funding-circle-flexipay.md). Documents in the old name are
this company's own.

Updating these accounts would remove a recurring source of confusion, and is also the correct
position for VAT purposes on invoices addressed to a name the company no longer uses.

### Reading these documents

Recorded in `CLAUDE.md` §3d, repeated here because it bears on any future invoice batch:

- **Screwfix classic invoices print a gross "Unit Price".** Use the Net column.
- **Screwfix "Order History" screenshot PDFs have no text layer.** Extraction returns only
  `Account Details _ Screwfix Website`. Over 40 of the 68 Screwfix files are of this kind and
  must be rasterised and read visually.
- **Photographed till receipts OCR well**, including the VAT analysis block, but the date
  sometimes does not survive.

## Open questions

- Are any of these accounts on credit terms, and is anything overdue? The statements show
  payments but no supplier statements are held.
- Should the trade accounts still in the former name be updated?
- The QuickBooks A/P aging totals £57,034 against £52,222 in the balance sheet, a difference of
  £4,812 - see [Data capture and accounting systems](../Processes/data-capture-and-accounting-systems.md).
  How much of A/P is trade supply as against subcontract labour is not broken out anywhere.
- Sebastian Pabis appears in QuickBooks A/P at £50,506 - larger than six months of total
  materials spend. What is that balance for?

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-05 | Created from the bank data and the Goathland invoice index | `Outputs/change-log-2026-09-05-wiki-from-bank-data.md` |

## Sources

[^1]: All six statement CSVs in [`Raw/Finance/`](../../Raw/Finance/), categorised and reconciled 2026-09-05.
[^2]: [`Raw/FP 2401_131 Goathland Avenue/INDEX.md`](../../Raw/FP%202401_131%20Goathland%20Avenue/INDEX.md), compiled 2026-09-05 by reading all 99 documents.
