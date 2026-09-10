# Change log - 2026-09-10 - Group policy v1.3 adopted; Kosmosoft SmartCABINET quote detected

## What was asked

The owner asked: *"check /Raw folder on google drive."*

## What was found

Two new arrivals in `Raw/` since the last check (2026-09-09):

1. **`2026-09-10_group-policy_document-numbering-and-filing-v1.3.md`**, delivered by the
   Fishbone Group knowledge base at 14:31. It resolves two *other* companies' change requests -
   `FM-CR-0001` (Fishbone Commercial Properties) and `FP-CR-0001` (Fishbone Properties), both
   Accepted 2026-09-10 - not anything this KB raised.
2. **`22910 FISHBONE.pdf`**, a scanned document ("Xerox Scan 20260910 082806.pdf") uploaded
   directly to `Raw/` (not via email), dated 10/09/2026. A software quote/contract (Offer/
   Contract Nr `22910`) from Kosmosoft Engineering S.r.l. (Bagnolo San Vito, Italy) for
   "SmartCABINET" - CRM/CAD/CAM/ERP software for cabinet making - addressed to **Fishbone
   Drylining Ltd**, the company's pre-October-2024 name.

The rest of `Raw/` (the two already-registered MSEM files kept locally, the Companies House
certificate, the v1.1/v1.2 policy notices, and the `Email`/`Finance`/`FP 2401 Goathland Avenue`/
`Vehicles` subfolders) matched `Outputs/kb-registers.md`'s existing Processed items table
exactly - nothing else new.

## Policy v1.3: what changed and what was adopted

Two clarifications, both accepted into policy **v1.3**:

1. **Property codes are 4-digit, self-assigned (§3/§7).** `<PREFIX>` + 2-digit acquisition year
   + 2-digit sequence (e.g. `FP1601`). Each company assigns its own and keeps its own property
   register; the group does not issue codes. **Not applicable to this KB** - Fishbone
   Construction Ltd owns no property (only vehicles, per `Wiki/Assets/vehicles.md`).
2. **Email-attachment source capture (§5).** Where the record is an email attachment whose
   bytes can't be captured into Drive, register with the Gmail thread id as `Source key` and a
   flagged plain-text transcription as the stored record; update later without renumbering if
   the binary is captured. **Directly relevant** - this KB's own info-mailbox pipeline
   (`Raw/Email/*.json`) has carried exactly this gap since 2026-09-06, with most captured
   messages noting "Attachments remain in Gmail and are not yet filed/validated."

Adopted into `Wiki/Processes/group-document-numbering-and-filing.md` (title, front matter and
body updated to v1.3) and `Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md`
(new section recording the v1.3 adoption). `CLAUDE.md` replaced by v10 (§1's live-data-sources
table corrected to v1.3).

**Not done:** applying the new email-attachment pattern retroactively to the existing backlog of
unfiled attachments in `Raw/Email/*.json`. That is separate, undecided work - the pattern is now
available to use, not applied.

## Kosmosoft SmartCABINET quote: registered pending, not processed

Read the document (OCR only - not re-read as a rasterised image). What's legible:
- Contract/Offer Nr `22910`, dated 10/09/2026, vendor Kosmosoft Engineering S.r.l. (Via Catania
  1, 46031 Bagnolo San Vito (MN), Italy).
- Product: "SmartCABINET", described as CRM/CAD/CAM/ERP software for cabinet manufacturing; one
  module clearly legible is "Cut optimization" (others present in the document but not cleanly
  OCR'd).
- Payment mode: 100% at confirmation. Offer validity: 30 days, then automatically cancelled.
  Payment by bank transfer to a named Credem account.
- Addressed to "Fishbone Drylining Ltd" - the company's name before the 31 October 2024 change
  to Fishbone Construction Ltd; a vendor still using the old name, not evidence of anything else.
- **Price is not stated with confidence.** The OCR shows "1.000,00" (Euro) on three separate
  lines - possibly three line items at €1,000 each, possibly an OCR duplication artefact of a
  single figure. Per `CLAUDE.md` §3d's reading-limits caution, this was not treated as a reliable
  total; re-reading the PDF as a rasterised image would be needed before quoting a firm price.
- No indication in the OCR text of whether this has been signed/accepted, or is still an open
  offer.

**Registered as `pending`** in `Outputs/kb-registers.md`'s Processed items table. **Not written
into the Wiki, and not registered in the group Document Register.** Two reasons: the pricing is
genuinely uncertain from OCR alone, and whether the company wants to proceed with this purchase
is the owner's decision, not something to assume by writing it up as settled. Per `CLAUDE.md`
§6a, automation may document but must never "commit the company to an obligation" - registering
this as an accepted business record before the owner has even seen the flagged uncertainty would
overstate what's actually known.

## What was not done

- **No group-register entry (`FC0000010` or similar) created** for the Kosmosoft document -
  deliberately deferred pending owner review of the price uncertainty.
- **No Wiki article written** for the Kosmosoft quote or for a Kosmosoft supplier record.
- **No re-read of the PDF as an image** to resolve the OCR uncertainty on price - flagged for a
  future session or the owner's own review, not done here.
- **No back-catalogue migration attempted** - v1.3 didn't reopen that question for this KB (see
  `Outputs/change-log-2026-09-09-v1.2-adopted.md`); nothing changed on that front.

## Files touched

Drive: two new `Raw/` files read (`2026-09-10_group-policy_document-numbering-and-filing-v1.3.md`,
`22910 FISHBONE.pdf`); neither moved, renamed or deleted.

Drive/git mirror: `Wiki/Processes/group-document-numbering-and-filing.md` and
`Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md` updated (v1.3 adopted),
`CLAUDE.md` (replaced by v10), `Outputs/kb-registers.md` (re-issued), this file.
