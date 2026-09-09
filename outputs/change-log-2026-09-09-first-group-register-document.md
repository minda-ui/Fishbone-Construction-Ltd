# Change log - 2026-09-09 - First real document registered in the group Document Register

## What was asked

Following confirmation of write access to the Fishbone Group's Document Register, the owner
asked: *"register the MSEM court claim as our first real document."*

## What was done

**Chose the document.** "The MSEM court claim" (County Court claim 019JE538, MSEM UK Ltd v
Fishbone Construction Ltd) is a case with many documents already tracked locally (`FCD0000007`,
`FCD0000015`-`FCD0000023` in the Construction Smartsheet workspace's own Document Register).
Per the group policy's `one owning entity → one row → one ID → one stored file` rule, a single
document had to represent it. The **Claim form** - MSEM's Money Claim Online form, the document
that actually started the case, dated 22 April 2026 - was chosen as the natural first/originating
document. It was already registered locally as `FCD0000018`.

**Dedup-on-entry.** Searched the group register by the file's Drive id and by "019JE538" before
minting anything. No match (the register held only Amfa Furniture Ltd's `FA0000001` at the
time).

**Filed.** The file already lived at
`Collaboration Space / Fishbone Construction / C Legal & Court Cases / MSEM UK Ltd Claim –
BBC Cardiff / Mikheil claim-form.pdf` - Collaboration Space filing was already in place, so no
move was needed. Renamed it in place (same Drive file id, so no links break) to
`FC0000001 - Legal - Claim form (claim 019JE538).pdf`, per the naming convention.

**Registered.** Added row `FC0000001` to the group Document Register: `Entity = FC - Fishbone
Construction Ltd`, `Direction = Incoming`, `Date = 2026-04-22`, `Category = Legal`, a
description covering the claim amount, the counterclaim, and the case's current procedural
state (Small Claims Track, evidence exchange 21 Oct 2026, hearing 19 Nov 2026), `Status =
Issued`, `Source key` = the Drive file id, and `File link`/`Location` pointing at the renamed
file in Collaboration Space. The description cross-references the local `FCD0000018` number and
the related tasks (`FCT00007`, `FCT00015`-`FCT00018`) and documents (`FCD0000015`-`FCD0000023`).

**Cross-referenced back.** Updated the local `FCD0000018` row's own description to note the new
group registration (`FC0000001`) and the file rename, so a reader starting from either register
finds the other.

**No new Wiki article.** Consistent with this KB's established pattern for this exact case
(sensitive legal correspondence, tracked in Tasks/Document Register only, kept out of the
Wiki), nothing new was written into `Wiki/`.

## What was not done

- **Nothing else from this case was registered in the group register.** Only the Claim form.
  The rest of the case's documents remain local-only (`FCD0000015`-`FCD0000023`) for now; the
  group policy's back-catalogue migration is explicitly the group's own follow-on, not this
  session's to run unilaterally.
- **No content or response was filed with the court, and no contact was made** with MSEM, its
  contact, or the court. This was a registration/filing action only.

## Files touched

Smartsheet: group Document Register (sheet `7352854736144260`) - one row added (`FC0000001`);
local Construction Document Register (sheet `258807861217156`) - one row's description updated
(`FCD0000018`).

Drive: the claim form file renamed in place (same file id): `1yJi66kcsZSR2jyXiKNyw5QXDcXQBnRBo`.

Drive/git mirror: `Wiki/Processes/group-document-numbering-and-filing.md` and
`Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md` updated (open question
about the first real registration now answered), `CLAUDE.md` (replaced by v7), this file,
`Outputs/kb-registers.md` (re-issued).
