# Wiki Maintenance Guidelines

> **Mirror of:** [Wiki/Wiki Maintenance Guidelines](https://docs.google.com/document/d/1mXih5Syp9WkcWuKU68pm6WXoSF8hhjOGJaSx9qoO6Ww/edit) (Google Drive)
> Drive is the working copy. See [README](../README.md) before editing here.

**Last updated:** 2026-08-25

## 1. Purpose of the Wiki

The Wiki folder holds reference documentation about the Classifier database and the
processes around it — not the data itself (that lives in Smartsheet). Keep articles
short, current, and link-rich rather than long and duplicative.

## 2. Folder structure

```
Fishbone Construction ltd/
  Raw/       — unprocessed source material dropped in for review
               (quotes, supplier lists, scraped rates, new item lists)
  Wiki/      — this documentation set
  Outputs/   — finished deliverables generated from the database
               (reports, exports, comparisons)
```

## 3. Article conventions

- One topic per article. If an article grows past ~1 page, split it.
- Title articles descriptively and consistently (e.g. "Database Structure", "Processing
  Workflow") — avoid version numbers in titles; use the "Last updated" line instead.
- Start every article with a one-line "Last updated: YYYY-MM-DD" so staleness is obvious
  at a glance.
- Write in plain English. Assume the reader is a colleague, not a specialist.

## 4. Linking between articles

- Link to other Wiki articles by pasting their Google Drive share link inline, e.g. "see
  Database Structure [link]" rather than just naming the article — a bare name isn't
  clickable and goes stale silently.
- When an article references a specific Smartsheet section, row range, or column, link
  the row/section if possible (Smartsheet permalinks) rather than describing it purely in
  prose.
- Maintain a short "See also" list at the bottom of each article pointing to directly
  related articles.
- If you rename or move an article, update inbound links from other articles in the same
  session — don't leave dangling links for the next session to discover.

## 5. Linking to sources

- Every rate or fact pulled from outside the Classifier (supplier site, quote, catalogue)
  should be traceable back to its source.
- For individual priced items, the source link belongs in the Classifier's own "Link to
  supplier" column — not duplicated into the Wiki.
- For broader claims or decisions documented in the Wiki (e.g. "we standardised on X
  supplier because Y"), cite the source inline with a link and a date accessed, e.g.
  "(source: [url], accessed 2026-08-25)".
- Never restate scraped supplier text at length — link to it and summarise in your own
  words (keeps the Wiki lightweight and avoids stale/incorrect copies of pricing).

## 6. When to update vs. create a new article

- Update in place for: corrections, refinements, expanded coverage of the same topic.
- Create a new article for: a genuinely new topic, or when an existing article has become
  two topics glued together.
- Never leave two articles covering the same ground — merge or redirect (a one-line
  "moved to X" stub is fine short-term).

## 7. Responsibility for keeping this current

Whoever processes new Raw items or changes the Classifier structure is responsible for
updating the relevant Wiki article in the same session, and for adding an entry to the
Change Log. Documentation debt compounds fast in a database-backed wiki — don't defer it.

---

**See also:** [Database Structure](database-structure.md) · [Processing Workflow](processing-workflow.md) · [Change Log](change-log.md)
