# Change log - 2026-09-11 - Raw/Finance checked; new RT_ export found, reconciled, registered pending

## What was asked

The owner asked: *"check /Raw/Finance folder for new bank transactions."*

## What was found

One new file since the six monthly HSBC statements already processed (which run 22 Feb to
21 Aug 2026): **`Raw/Finance/RT_20260911_04212819.csv`**, uploaded 2026-09-11.

It is **different in kind** from the prior six files, not just a new month:
- **Naming.** `RT_20260911_04212819.csv` - an `RT_` (Recent Transactions) prefix with the
  export date, not the prior `YYYYMMDD_04212819.csv` pattern keyed to the statement's closing
  date.
- **Columns.** `Date,Type,Description,Amount,Balance` - one signed `Amount` column and a
  `Balance` printed on every row - instead of the prior `Date,Type,Description,Paid Out,Paid
  In,Balance` with `Balance` printed only intermittently.
- **Coverage.** 217 transactions, newest-first, spanning **12 Aug to 11 Sep 2026** - a rolling
  window, not a closed statement cycle.

## Reconciliation

Per `CLAUDE.md` §3d, no figure from this file is quoted without reconciling first:

1. **Internal arithmetic.** Checked every adjacent pair of rows: `balance[i] == balance[i+1] +
   amount[i]`, walking oldest to newest. **0 mismatches across all 217 transactions.**
2. **Continuity with the last processed statement.** The prior file
   (`Raw/Finance/20260821_04212819.csv`) closes on 21 Aug 2026 at **£5,867.23** (last row:
   Screwfix Dir Ltd, -£29.28). The new file's 21 Aug 2026 row for the same transaction
   (description, amount and date all match) closes at the **same £5,867.23**. The two files
   agree exactly where they overlap.

Rows dated 12-21 Aug 2026 in the new file duplicate `20260821_04212819.csv`, already `done`.
**Rows dated 22 Aug-11 Sep 2026 are new** - 21 days not yet reflected anywhere in this
knowledge base.

## Why this was not reconciled into the Wiki

Two reasons, both explained in `Outputs/kb-registers.md`'s new Processed items row:

1. **It's a partial period.** `CLAUDE.md` §1 says the next expected file is the full 22 Aug to
   21 Sep cycle; this file stops on 11 Sep, ten days short of that close. The KB's practice has
   been to fold a full month into the Finance/Customer/Supplier Wiki articles at once, not a
   partial window - writing up a partial reconciliation risks a figure that changes again in
   ten days without a "Changes" trail explaining why.
2. **The shape is different** from the categorisation and Classifier-adjacent workflow already
   built around the six-column monthly format. Folding a differently-shaped export into that
   workflow untested, without checking whether more `RT_` files are coming or whether a proper
   `20260921_04212819.csv` close will still arrive, risks inventing a process the owner didn't
   ask for.

**Registered `pending`** in `Outputs/kb-registers.md`'s Processed items table rather than
`done` or `partial` - nothing has been written into the Wiki from it yet.

## Notable transactions in the new territory (22 Aug - 11 Sep), not yet written up

- **Kosmosoft payment corroborated.** A debit dated 10 Sep 2026: `22910 RBD10096F7N5Y58G
  Kosmosoft Srl 0000001.13891400 /TMS/ 2026-09-10 07:28:59 GMT /MID/ 1.164685`, **-£878.03**.
  The reference carries the offer number (`22910`) and an FX rate (`1.13891400`); £878.03 ×
  1.13891400 ≈ €1,000.00 almost exactly. This independently corroborates the owner's statement
  the day before that the SmartCABINET purchase (`Wiki/Suppliers/kosmosoft-smartcabinet.md`)
  cost €1,000 - worth noting on that article as bank-transaction evidence, not done in this
  session since it wasn't asked for here.
- **Macdonald Joinery continuing to pay, and increasing.** Four credits in the new window: 21
  Aug £1,360; 28 Aug £2,920; 4 Sep £3,000; 11 Sep £6,144 - the last one the largest single
  Macdonald credit since the May 2026 fall documented in
  `Wiki/Customers/macdonald-joinery.md`. Four data points across three weeks don't establish a
  new trend on their own, and this session draws no conclusion from them - flagged for whoever
  next reconciles this period into the Wiki.
- **LendingCrowd DD (9 Sep, -£2,388.26)** matches the already-documented "£2,388 a month,
  unvarying" pattern in `Wiki/Finance/debt-service.md` - checked against that article before
  treating it as anything new. Not a new lender.
- Continued `HOLDINGS loan` and `Fishbone Drylining FLEXIPAY` inbound credits, consistent with
  the already-documented related-party funding pattern - no new counterparty observed.

None of the above was written into any Wiki article this session; they are flagged here so the
next processing pass (whenever the full 22 Aug-21 Sep statement arrives, or if the owner asks
for this partial window to be processed now) doesn't have to re-derive them.

## What was not done

- **No Wiki Finance, Customer or Supplier article was updated.** The new transactions are
  listed above but not categorised or written into any article.
- **No Smartsheet Classifier/Budget writes.** Not applicable to bank data, and none attempted.
- **No conclusion drawn about Macdonald Joinery's trend** from four transactions.
- **`CLAUDE.md` was not replaced.** Its §1 note ("next file expected: 22 Aug to 21 Sep") still
  holds; this file doesn't satisfy that yet.

## Files touched

Drive: `Raw/Finance/RT_20260911_04212819.csv` read only; not moved or renamed.

Drive/git mirror: `Outputs/kb-registers.md` re-issued, this file.
