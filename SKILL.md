---
name: content-gate
description: >-
  Use when drafting, editing, reviewing, or approving blog or guide articles for
  search or publish quality. Run the people-first / Google Search Central
  Content Gate before shipping. Prefer quality over page count. Do not use for
  keyword-volume, backlink, or ranking-manipulation tactics.
---

# Content Gate

Use Content Gate before drafting, rewriting, reviewing, or approving blog and
guide articles meant to rank or attract search traffic. The authority sources
are Google Search Central (helpful content, gen-AI content, spam policies,
Search Essentials). Prefer quality over page count.

This skill is generic: it applies to blogs and guides on any site. Do not
assume a product brand, vendor, or house style unless the project's own
guidelines file says so.

## 1. Load the project's own writing rules first

1. Look for a repo or workspace content-guidelines / editorial / SEO writing
   doc (often `CONTENT_GUIDELINES.md`, `guidelines.md`, or similar).
2. If one exists, **Read it and treat it as the hard gate** for that project.
   This skill is the shared procedure; that file owns project-specific facts,
   product boundaries, and checklist extras.
3. If none exists, continue with the Google-aligned checks below and note that
   the project has no locked local guidelines.

## 2. Decide Why before keywords

Answer in one sentence: who is helped, and what task can they finish after
reading?

- If the honest answer is mainly "rank for search" with little reader value →
  do not publish; rewrite or cancel.
- Titles and H1s may use the words people search with, but only **after** the
  article already helps a direct visitor.

## 3. People-first vs search-engine-first sniff test

Flag search-engine-first patterns (any several is a stop):

- Written mainly to attract search visits, not existing readers
- Many near-duplicate pages covering slight keyword variants
- Heavy automation / AI volume with little added value
- Mostly rewritten third-party text
- Padding for length; no preference for word count
- Sensational titles that overpromise
- Freshness theater (date bumps with no real update)

Prefer people-first signals: first-hand experience, clear site purpose, enough
depth to complete the job, something a reader would bookmark or share.

## 4. Who / How / Why self-check

| Lens | Check |
| --- | --- |
| **Who** | Clear attribution (person or accountable team); link to About / author when readers would ask who wrote it |
| **How** | Steps match real UI/product; evidence (screenshots, measured conditions); if AI heavily assisted drafting, disclose when readers would reasonably ask how it was made |
| **Why** | Exists to help people complete a task—not mainly to manipulate rankings |

Do **not** put "AI" as the author byline.

## 5. Spam / scaled-content hard stops (must all be No)

- Main purpose is ranking manipulation rather than helping users?
- Batch-producing many near-identical thin pages (AI, template, or human)?
- Scraping / synonymizing / low-quality translation with little added value?
- Keyword stuffing or doorway-style query pages?
- Date change without substantive update?

Any **Yes** → do not publish.

## 6. Pre-publish checklist (Yes / No)

**Helpfulness**

- [ ] A direct visitor (not only a searcher) would find it useful
- [ ] Reader can complete a concrete goal after reading
- [ ] First-hand traces exist (real steps, limits, data, or screenshots)
- [ ] Clear extra value beyond restating docs or competitors
- [ ] Title is accurate, not hype
- [ ] You would share or bookmark it

**Trust**

- [ ] Attribution / ownership is clear
- [ ] Trust surfaces reachable (About, Support, Privacy, Contact as relevant)
- [ ] Key facts verified by a human who knows the product or topic
- [ ] No easily checkable exaggerations or stale claims
- [ ] AI-assisted drafts were deeply edited so they are not hollow shells

**Craft & localization**

- [ ] Written for the target language’s readers first—not line-by-line translation
- [ ] Plain, specific, actionable verbs; each paragraph earns its place
- [ ] No empty marketing fluff ("revolutionary", "ultimate", "one-click solves everything")
- [ ] No mechanical keyword repetition in adjacent sentences or headings
- [ ] Product/topic boundaries stated honestly (what it does not do)

**Pass rule:** Section 5 all No; Section 6 mostly Yes. Known gaps need a fix
plan before Conditional pass. Same template across brands/vendors must pass the
"remove the brand name—does it still look like a reskin?" test; if yes, merge
or cut.

## 7. When launching or reviewing agent-written copy

1. Point the writer at this skill **and** the project guidelines file.
2. Require the Section 5–6 checklist in the PR / review notes.
3. Run any project SEO/content audit script if one exists (for example a site
   SEO audit npm/script); fix failures before merge.
4. Review language naturalness and honesty separately from technical SEO
   (titles alone do not pass the gate).

Use `assets/templates/gate_report.md` as the output shape for the verdict.

## 8. Verdict

Record one of:

- `pass`: Section 5 all No; Section 6 mostly Yes; no unresolved hard-gate
  guideline failures.
- `conditional`: publishable only after a named fix plan for known gaps.
- `fail`: any Section 5 Yes, or the article is mainly search-engine-first.

Do not invent metrics, traffic forecasts, keyword volumes, or competitor
scores to justify a pass.

## 9. What this skill is not

- Not a keyword-volume / backlink playbook
- Not permission to invent metrics, competitor prices, or unverified
  head-to-head scores
- Not a substitute for the project’s own locked guidelines when those exist
- Not black-hat SEO, ranking manipulation, or scaled thin-content advice
