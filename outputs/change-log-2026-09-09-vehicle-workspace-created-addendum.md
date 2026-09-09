# Change log - 2026-09-09 - Vehicle workspace: Wiki, CLAUDE.md v4, and a folder mix-up (addendum)

This is an addendum to `Outputs/change-log-2026-09-09-vehicle-workspace-created.md`, which
another, concurrent session wrote retrospectively from `Raw/Vehicles/INDEX.md`'s own account.
That entry is accurate as far as it goes (the Raw workspace, vehicle #1 confirmed as the Ford
Transit HT22BWP, Haydock Finance ruled out, Tower Leasing and vehicles #2/#3 still open) but
predates - and doesn't know about - the rest of the same underlying session's work, because two
sessions were editing this knowledge base concurrently. This entry fills in what it doesn't
cover, and records a process error worth keeping visible.

## What this adds

**Wiki.** Created the `Wiki/Assets/` category (not previously among this KB's eight named
categories) and its first article, `Wiki/Assets/vehicles.md` (`draft`). The reasoning for a new
category rather than filing under `Finance/` is in
`Wiki/Decisions/2026-09-09-assets-category-and-vehicles-workspace.md`, also created this
session. `Wiki/index.md` was rebuilt to list both.

**`CLAUDE.md` replaced by v4.** While working, the live `CLAUDE.md` was found to have been
edited out-of-band on 2026-09-06 (an operational-update banner, a struck-through line in §5, a
qualification in §7) without archive-then-recreate. `Wiki/Processes/email-to-tasks.md` was read
in full and the edit found to be genuine, sourced work, not reverted. `CLAUDE.md` v4 preserves
that content, adds the Assets/Vehicles workspace to §1, and adds a new §6d rule 5 stating that
archive-then-recreate applies to this file with no exception for a well-intentioned edit.

## A folder mix-up, and what it means for this file

While rebuilding `Outputs/kb-registers.md` earlier in this session, its live copy was archived
before checking what folder its own replacements were being written to. Two files -
`kb-registers.md` and a first draft of this entry, under the name
`change-log-2026-09-09-vehicle-workspace-created.md` - were created in
`Archive/` (folder id `1m2JY4DPZ9N8B3ZpgrXGzk6kZeDPFXErM`, which had been read from repeatedly
while chasing archived copies of `kb-registers.md`, and was wrongly assumed to be `Outputs/`
because every kb-registers.md file found by name so far happened to be an archived one sitting
there) instead of the real `Outputs/` folder (`1ckL5P1rde59_QQ_p9WtllVcDyT7fT9oD`). Both
misplaced files have been trashed. Nothing was lost: the `kb-registers.md` content that mattered
- the concurrent session's Mail Register and Fishbone Holdings dividend work, the court-notice
entry, and the retrospective vehicle-workspace entry - was already correctly filed in the real
`Outputs/` by the other session by the time this was caught, and this addendum now sits
alongside it in the right place.

**Lesson recorded rather than silently fixed:** a folder id is not "the Outputs folder" just
because every file found under a given name so far came from there. Confirming a destination
folder's own title and parent before writing to it - not just pattern-matching on what's already
in it - would have caught this before, not after, two files were misfiled.

## What was not done (unchanged from the entry this addends)

- The Smartsheet fleet register - deferred by the owner's own instruction.
- Vehicles #2 and #3 - not identified, not guessed.
- Tower Leasing - left open; two sources give different amounts and neither describes the
  leased asset.

## Files touched by this addendum

Drive: `Wiki/Assets/`, `Wiki/Assets/vehicles.md`,
`Wiki/Decisions/2026-09-09-assets-category-and-vehicles-workspace.md`, `Wiki/index.md`
(re-issued), `CLAUDE.md` (replaced by v4), this file. Two misfiled files trashed (see above).

Git mirror: `wiki/Assets/vehicles.md`, `wiki/Decisions/2026-09-09-assets-category-and-vehicles-workspace.md`,
`wiki/index.md`, `CLAUDE.md`, `raw/Vehicles/INDEX.md`, `outputs/change-log-2026-09-09-vehicle-workspace-created.md`
(this session's original, fuller draft of the entry the other session also wrote independently -
kept in the git mirror as this session's own record; the canonical Drive copy under that exact
name is the other session's retrospective entry, per Drive's "first writer keeps the plain name"
outcome here) committed to `claude/fishbone-construction-5uqgot`.
