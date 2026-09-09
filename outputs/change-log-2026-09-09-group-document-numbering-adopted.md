# Change log - 2026-09-09 - Group document-numbering policy adopted

## What was asked

Following an earlier check of `Raw/` for new documents (which surfaced a group policy notice,
among other things), the owner asked: *"adopt the group document-numbering policy into
CLAUDE.md."*

## What was done

**Read the policy.** `Raw/2026-09-09_group-policy_document-numbering-and-filing-v1.1.md` -
delivered by the Fishbone Group knowledge base, marked "for adoption, not for registration,"
locked and versioned at v1.1. It asks every group KB (Properties, Commercial Properties,
Holdings, Construction, Waste, Amfa Furniture, SSAS) to register every business document once,
in one cross-company Smartsheet Document Register, filed with the project it belongs to.

**Adopted the rules into the Wiki, not directly into `CLAUDE.md`.** Per `CLAUDE.md` §6d rule 4
("detailed rule sets live in the Wiki, not here"), the full rules went into a new article,
`Wiki/Processes/group-document-numbering-and-filing.md`: the one register (Smartsheet, sheet id
`7352854736144260`, workspace "Fishbone Group - Documents"), the `<PREFIX>` + 7-digit ID scheme
(this company's prefix is `FC`), the anti-duplication and dedup-on-entry rules, what does and
doesn't get registered, the Collaboration Space filing convention, the inter-KB hand-off
procedure (new in v1.1, §7a), and the group's Change Requests sheet for anything that doesn't
fit. `CLAUDE.md` itself got one new row in §1's live-data-sources table, pointing at that
article.

**Flagged, rather than silently resolved, a naming collision.** This company's existing
Construction Smartsheet workspace (built 2026-09-06 for the info-mailbox pipeline) already has
its own local numbering: `FCT` for Tasks, `FCD` for its own Document Register - already in
active use by the MSEM court case (`FCD0000015` through `FCD0000023`). The group's new register
uses a *different* prefix (`FC`, no `D`) in a *different* sheet. `Wiki/Decisions/2026-09-09-
group-document-numbering-policy-adopted.md` records the decision: keep both running in
parallel, do not attempt to merge or re-number the local `FCD`/`FCT` history locally - the
policy's own text says migrating the back-catalogue is a follow-on the *group* runs, and
re-numbering documents other sessions already reference (the court case, in particular) without
being asked would be exactly the kind of local variation the policy rules out.

**Checked access rather than assuming it.** Read access to the group Document Register was
confirmed (`get_sheet_summary` returned the sheet - empty, as expected for a brand-new
register). Write/Editor access was **not** tested, since nothing yet needs writing to it and the
policy's own adoption steps say the owner was still arranging those shares. Recorded as an open
question rather than assumed either way; the first genuinely new qualifying document is the
real test.

**Left the policy notice in `Raw/`.** It asks receiving KBs to "archive this file" once adopted.
This KB's own, more specific rule - "nothing is deleted or moved out of Raw" (`CLAUDE.md` §1) -
takes precedence for this KB's own files, so it was not moved or deleted. It is logged as
`skipped` in `Outputs/kb-registers.md` (not source material for the Wiki), which is this KB's
established way of registering non-source Raw items without physically touching them.

## What was not done (by design)

- **No document has been registered in the new group register yet.** Nothing qualifying has
  come up since adoption to test it with.
- **No migration of the local `FCD`/`FCT` back-catalogue.** Explicitly the group's own follow-on.
- **The policy notice file was not moved, archived, or deleted** from `Raw/` - see above.

## Files touched

Drive/git mirror: `Wiki/Processes/group-document-numbering-and-filing.md` (new),
`Wiki/Decisions/2026-09-09-group-document-numbering-policy-adopted.md` (new), `Wiki/index.md`
(re-issued to list both), `CLAUDE.md` (replaced by v5), this file, `Outputs/kb-registers.md`
(re-issued).
