# Change log - 2026-09-09 - Rest of the local FCD back-catalogue: change request raised, not migrated

## What was asked

Following registration of the MSEM case's remaining documents (`FC0000002`-`FC0000009`), the
owner asked: *"migrate the rest of the local FCD back-catalogue too."*

## What was done

**Checked scope before doing anything.** The local Construction Document Register (Smartsheet,
sheet `258807861217156`) has 23 rows. 9 (`FCD0000015`-`FCD0000023`, matching `FC0000001`-
`FC0000009`) are already migrated. The remaining 14 are `FCD0000001`-`FCD0000014`.

**Read all 14 before migrating anything.** They are not documents in the sense the MSEM ones
were:
- Every `File link` is a Gmail message URL (`https://mail.google.com/mail/#all/...`) - no
  stored file, no Drive file id.
- Every `Description` says the underlying attachment or record is unfiled or unverified, e.g.
  "Attachments remain in Gmail and are not yet filed/validated" or "Underlying records not
  verified."
- Titles are action items, not document titles: "Reconcile Tower Leasing invoice 916284
  overdue notice," "Verify Forth England INV-1627 payment and filing," "Review SiteDocs
  renewal and notice deadline," "Decide Microsoft 365 renewal for two licences," "Coordinate
  Andrejus ArtiCAD training on 14 September," and similar for the rest.

This is the Construction info-mailbox intake pipeline's own tracking mechanism, closer in
nature to the local `FCT` Tasks sheet than to a registrable business document. Policy v1.1
explicitly excludes "routine automated notifications" and says to raise anything unclear
rather than guess.

**Decision: don't migrate them; raise it with the group instead**, per the policy's own
"do not fork the rules... raise a row on the group's Change Requests sheet" instruction. Added
`FC-CR-0001` to the group's Document System - Change Requests sheet (Smartsheet, sheet id
`8918834172004228`, "Fishbone Group - Documents" workspace, previously empty), asking:
1. Whether rows like these 14 - unfiled task/email pointers, not stored documents - qualify
   for the group Document Register at all.
2. Whether, separately, this KB is expected to run any part of the local back-catalogue
   migration itself, or should wait for a group-run pass (the policy's own transition text
   says migration is "the group's own follow-on").

**Not migrated: the 14 rows stay local-only (`FCD`-prefixed) for now**, pending a response on
`FC-CR-0001`.

## What was not done

- **None of `FCD0000001`-`FCD0000014` were registered in the group Document Register.** No
  files were renamed or moved for them; no local rows were changed.
- **No document was fabricated to fill the gap.** Where a row's own content said its evidence
  is unverified, that was taken at face value rather than treated as good enough to register.
- **No response to `FC-CR-0001` was assumed.** The Change Request sits at `New` status.

## Files touched

Smartsheet: group Document System - Change Requests sheet (sheet `8918834172004228`) - one row
added (`FC-CR-0001`); no change to the local Construction Document Register (sheet
`258807861217156`) or the group Document Register (sheet `7352854736144260`).

Drive/git mirror: `Wiki/Processes/group-document-numbering-and-filing.md` and
`Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md` updated (open questions
replaced with the Change Request outcome), `Outputs/kb-registers.md` (re-issued), this file.
