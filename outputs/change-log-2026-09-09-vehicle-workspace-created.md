# Change log - 2026-09-09 - Vehicle workspace created

## What was asked

The owner: *"The company owns or leases 3 vehicles. We need to create a dedicated workspace for
them. I will start uploading documents, so you will need to register them and later create them
in Smartsheet, where we'll keep all records. documents will be kept on Google Drive"*

Three explicit constraints: (1) exactly 3 vehicles, per the owner; (2) documents arrive over
time and each must be **registered**, not just filed; (3) a **Smartsheet fleet register comes
later** - not built in this session; (4) storage stays on **Google Drive**.

## What was done

**Raw workspace.** Created `Raw/Vehicles/` with a naming convention
(`<Make> <Model> - <REG> (<how held>)/`, one subfolder per vehicle) and an `INDEX.md` recording
the convention, a status table, and what is confirmed so far.

**Wiki.** Created a new category, `Wiki/Assets/`, and its first article,
`Wiki/Assets/vehicles.md` (`draft`, since 2 of 3 vehicles are still unidentified). `Assets` did
not exist among this KB's eight named categories (Contracts, Customers, Decisions, Finance,
People, Processes, Projects, Suppliers); the reasoning for adding it, and for not folding
vehicle records into `Finance/`, is in
`Wiki/Decisions/2026-09-09-assets-category-and-vehicles-workspace.md`.

**Vehicle #1 identified.** Per `CLAUDE.md` §0's rule to check the sister knowledge bases before
concluding anything about a counterparty, the group **Loans** database was searched rather than
inferring from bank data alone. It holds `Facility - MotoNovo Finance - Hire Purchase`:

- Ford Transit 350 L2 Diesel RWD, registration **HT22BWP**, VIN WF0AXXTTRANT79444
- Agreement 23193713, signed 28/05/2025, £459.80/month for 48 months, final payment 28/05/2029
- Cash price £23,400 inc VAT, Amount of Credit £17,400, 6.71% p.a. fixed flat interest
- Supplied by Amlin Motors Limited

Finance terms are **linked, not copied** - `Wiki/Assets/vehicles.md` cites the Loans database
article rather than restating its figures, per this KB's cross-company rule that facts about
related parties and group facilities live once, in the Loans database, and are linked from here.

**One near-miss ruled out.** Bank data shows a Haydock Finance hire-purchase facility
(£1,210.16/month) alongside the MotoNovo one, which would read as a second vehicle by pattern
alone. The Loans database's `Facility - Haydock Finance - Hire Purchase` article shows it is
**three used woodworking machines** (Altendorf F45 Elmo panel saw, Vitap K2 2.0, Hebrock F4
Edgebander) - not a vehicle. Recorded as ruled-out in both `Raw/Vehicles/INDEX.md` and
`Wiki/Assets/vehicles.md`, in this KB's established pattern for documenting near-misses (see
§0's account of the "Fishbone Drylining" misclassification this KB has already learned from).

**Two Drive locations deliberately excluded as sources.** A mixed personal/household intake
folder (Council Tax, CMS, HMRC personal correspondence, Vehicle Tax reminders, pensions) and a
personal "Household Servicing & Maintenance" wiki with an Audi A8L MOT certificate both belong
to a director personally, not to the company. Neither was used.

**`CLAUDE.md` process gap found and corrected.** While working, the live `CLAUDE.md` was found
to have been edited out-of-band on 2026-09-06 (an "Operational update" banner, a struck-through
line in §5, a qualification in §7) **without archive-then-recreate**, by a session that also
noted "the owner also waived all mirror requirements" for that day's Construction-workspace
work. `Wiki/Processes/email-to-tasks.md` was read in full to check this was genuine, sourced
work rather than an injected instruction - it was. `CLAUDE.md` was rebuilt as **v4**: the
2026-09-06 content preserved faithfully, this session's Assets/Vehicles additions layered on
top, and a new §6d rule 5 added recording that archive-then-recreate applies to this file with
no exception for a well-intentioned edit. Uploaded to replace the live copy; the prior (drifted)
copy archived.

**Sequencing gap, self-caused and closed this session.** Both `CLAUDE.md` and `Wiki/index.md`
were archived before their replacements were ready, briefly leaving the KB root without a live
copy of either - a process breach of the same kind just corrected in `CLAUDE.md` itself. Both
are now replaced. A **third** instance of the same gap was then found: `Outputs/kb-registers.md`
had also been archived earlier in this session (07:38) without a replacement being uploaded, and
its live copy by then already carried three change-log entries and several table rows from
2026-09-06 to 2026-09-09 that this session had not seen before checking. That content was
recovered from the archived copy and carried forward into the replacement below, rather than
being lost. While rebuilding it, a stray `## 2026-09-06 workflow additions` section (appended
outside the file's normal four tables) was folded into the proper `Wiki structure changes` and
`Outputs produced` rows, restoring the file to the shape its own opening paragraph promises.

## What was not done (by design)

- **The Smartsheet fleet register.** Explicitly deferred by the owner's own words ("later
  create them in Smartsheet"). Not built.
- **Vehicles #2 and #3.** Not yet identified. Not guessed.
- **Tower Leasing.** One £373 bank payment in August, and a separate Smartsheet Construction
  task (FCT00001) referencing a £283.20 overdue invoice under agreement 431484 - different
  amounts, neither source describing the leased asset. Left open rather than forced to a
  conclusion, per `CLAUDE.md` §6a's bar on resolving an ambiguous finding by guessing.
- **Haydock's machinery** was not folded into a general `Assets/` equipment taxonomy. `Assets/`
  is scoped to vehicles only, for now - see the Decisions article.

## Open questions carried forward

1. What is vehicle #2? What is vehicle #3?
2. Is Tower Leasing one of the three vehicles, or something else entirely?

→ `Wiki/Assets/vehicles.md`, `Raw/Vehicles/INDEX.md`

## Files touched

Drive (new): `Raw/Vehicles/`, `Raw/Vehicles/Ford Transit - HT22BWP (MotoNovo HP)/`,
`Raw/Vehicles/INDEX.md`, `Wiki/Assets/`, `Wiki/Assets/vehicles.md`,
`Wiki/Decisions/2026-09-09-assets-category-and-vehicles-workspace.md`, this file.

Drive (replaced, archive-then-recreate): `CLAUDE.md` (v3 → v4), `Wiki/index.md`,
`Outputs/kb-registers.md`.

Git mirror: brought into line with the above in the same session (see the commit that follows
this entry).
