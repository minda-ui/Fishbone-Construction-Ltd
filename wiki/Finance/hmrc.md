---
title: HMRC - PAYE, Time to Pay and VAT
category: Finance
status: active
sensitive: true
created: 2026-09-05
updated: 2026-09-05
sources:
  - ../../Raw/Finance/20260321_04212819.csv
  - ../../Raw/Finance/20260421_04212819.csv
  - ../../Raw/Finance/20260521_04212819.csv
  - ../../Raw/Finance/20260621_04212819.csv
  - ../../Raw/Finance/20260721_04212819.csv
  - ../../Raw/Finance/20260821_04212819.csv
related:
  - ../Finance/hsbc-current-account.md
  - ../Finance/funding-circle-flexipay.md
  - ../Finance/debt-service.md
---

# HMRC - PAYE, Time to Pay and VAT

**No payment to HMRC left the company's bank account between 22 April and 21 August 2026** -
four months. There is an explanation that makes that normal and an explanation that makes it
serious, and the bank statements cannot tell them apart. This needs checking against the HMRC
account, not inferring.

## Key facts

| Item | Value | Source |
|---|---|---|
| HMRC payments out, six months | £27,212 | [^1] |
| Last payment out | £12,562.03 on 22 April 2026 | [^2] |
| Months with no HMRC payment | 22 Apr to 21 Aug 2026 (four) | [^1] |
| VAT refunds in, six months | £19,024 | [^1] |
| Paid to HMRC via the FlexiPay-funded arrangement (per the group Loans database) | £54,258.57 | [^3] |

## Details

### What the statements show

| Date | Description | Amount |
|---|---|---:|
| 27 Feb 2026 | HMRC NDDS | £4,000.00 |
| 6 Mar 2026 | HMRC NDDS | £4,000.00 |
| 13 Mar 2026 | HMRC NDDS | £6,649.67 |
| 22 Apr 2026 | HMRC PAYE/NIC SPLY 475PS005711382612 | £12,562.03 |
| *then nothing to 21 Aug 2026* | | |

"NDDS" is HMRC's direct debit service, consistent with a Time to Pay arrangement being
collected. Those collections stop after 13 March; a single PAYE/NIC payment follows on 22
April; then silence.

### The two readings

**Benign.** The group Loans database records £54,258.57 paid directly to HMRC under a Time to
Pay arrangement funded by Funding Circle FlexiPay. That money moves lender to HMRC without
passing through this account, which is exactly why it would be invisible here. On this reading
the arrangement is current and the statements simply do not see it.

**Serious.** A Time to Pay arrangement that has defaulted also produces no payments on the bank
statement. The two look identical from here.

The benign reading is the more likely one and it is what the previous change-log entry
concluded. It is still an inference from an absence, and an absence is weak evidence. **Confirm
against the HMRC business tax account.** If the arrangement has in fact lapsed, PAYE and NIC
arrears rank as Crown debt and the position is materially worse than this knowledge base
currently records.

An earlier reading in this knowledge base, based on three months of statements only, concluded
that PAYE was going unpaid. That was wrong and was corrected on 2026-09-04. The correction is
not itself proof that the arrangement is current.

### The substance, if the benign reading holds

An interest-free HMRC arrangement has been converted into fee-bearing debt at an overall rate
of 8.53%. That is a worse position than owing HMRC directly. It is worth asking HMRC whether it
would extend Time to Pay against the current trading position instead - the answer costs
nothing to obtain.

### VAT

HMRC refunded £10,108.69 on 12 March 2026 and £8,915.43 on 12 June 2026 - £19,024 over six
months, and no VAT paid out at all. A construction company in a repayment position is normal
under the domestic reverse charge, where most sales are zero-rated to the customer while input
VAT on materials is recoverable.

That said, Companies House charged late-filing penalties of **£375 and £150 on 20 April 2026**,
which says filing deadlines are being missed somewhere. Whether VAT returns are current has not
been checked.

## Open questions

- **Is the Time to Pay arrangement current or in default?** The single most checkable item here.
- What periods does it cover, what is the outstanding balance, and when does it end?
- Are VAT returns filed and up to date?
- What were the two Companies House penalties for, and are the accounts now filed?
- Is CIS being operated and returned? The company pays subcontractors monthly - see
  [Subcontractors](../Suppliers/subcontractors.md) - and nothing in this knowledge base
  addresses CIS deductions or returns at all.

## Changes

| Date | Change | Change-log ref |
|---|---|---|
| 2026-09-05 | Created from the six statement CSVs | `Outputs/change-log-2026-09-05-wiki-from-bank-data.md` |

## Sources

[^1]: All six statement CSVs in [`Raw/Finance/`](../../Raw/Finance/), categorised and reconciled 2026-09-05.
[^2]: [`Raw/Finance/20260521_04212819.csv`](../../Raw/Finance/20260521_04212819.csv), line dated 22 Apr 2026.
[^3]: Group Loans database, Book 1, as recorded 2026-08-21. Separate Drive folder; not held in this knowledge base.
