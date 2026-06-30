# Data Processing Roadmap

*Artist Mutual Aid Directory — how resource data is sourced, processed, and displayed, and how that process has changed.*

---

## Purpose

This statement documents the directory's data strategy: how resource information is acquired, cleaned, verified, and published, why that process changed from its original 2021 design, and the direction it's moving in as new tools and partnerships become available. It exists so the process is documented and repeatable, rather than living only in one person's working memory.

---

## Original Approach (2021)

The project's original design, developed during the 2021 Kaggle/Google BIPOC Data Fellowship, assumed resource data would come primarily from **bulk public datasets** — structured exports from sources like the National Endowment for the Arts (NEA/arts.gov), national mutual aid directories, and general web search for downloadable structured data (CSV, spreadsheet, and similar file types). The planned pipeline was: locate bulk sources → download → clean with Python/Pandas → publish to the directory.

## What Changed

By the time active development resumed in 2026, several conditions had shifted in ways that made the original bulk-sourcing model substantially less viable:

- **Dataset discoverability has decreased.** General web search no longer surfaces downloadable structured data (CSV, spreadsheet exports, etc.) as reliably as it once did. Search behaviors that previously worked well for locating this kind of file are significantly less effective now.
- **Some originally identified sources are no longer available or no longer reliable.** Specific sources flagged in 2021 (including NEA/arts.gov exports and MutualAidHub) were re-evaluated in 2026 and found to be inconsistent, lacking a clean export mechanism, or otherwise not suited to bulk integration in their current state.
- **Link rot and source attrition.** A meaningful share of resource links collected during the 2020–2021 period are now broken, redirected, or point to organizations that have since changed scope, merged, or ceased operating.
- **Terminology sensitivity has affected source availability.** The term "mutual aid" carries specific associations for some audiences that go beyond its general dictionary meaning. In some cases, this has made organizations and platforms more cautious about publicly using that framing or openly sharing structured data under it, which has, in turn, reduced the pool of readily available bulk data using that terminology. This directory uses "mutual aid" descriptively, in its general sense of community members supporting one another, and does not take a position on the term's broader associations.

## Current Approach (2026 onward)

Given the above, the directory has moved to a **manual curation model** as the primary method, rather than a fallback:

1. **Acquisition** — resources are now identified individually, through direct research, community submissions (via the site's Submit a Resource flow), and targeted review of known organizations' own websites, rather than broad bulk-dataset search.
2. **Staging** — any externally sourced spreadsheet or list goes through an offline first-pass cleanup, then a structured staging process (see internal data vetting documentation) before any entry is considered for inclusion. Entries that originate from a secondary or nested source (a spreadsheet found via a link inside another spreadsheet) receive additional scrutiny.
3. **Verification** — each resource is checked individually: the link is confirmed live, the organization's current scope is confirmed to match the description, and the entry is checked against existing directory entries to avoid duplication.
4. **Publication** — only verified entries are added to the live directory's resource data.

## Toward Automation

Manual acquisition and manual verification remain necessary for now — there is no reliable automated substitute for confirming an organization is still active and accurately described. However, parts of the *processing* pipeline (once a source is acquired) are already automatable and are being built out incrementally:

- Column standardization and basic formatting cleanup (WIP/testing — filename to be `clean_and_dedupe.py`)
- Duplicate detection by normalized link (in place)
- Category-keyword pre-mapping to reduce manual categorization effort (in place, human-reviewed)
- Planned: automated periodic link-health checking for already-published entries, to catch link rot after the fact rather than only at intake
- Planned: structured intake from any sources that do offer a stable API or consistent export format (211.org is the most likely candidate, contingent on API access)

As trusted, consistently-formatted sources are identified over time — whether through direct partnerships, community submissions reaching sufficient volume, or stable APIs — the acquisition step itself may become more automatable. Until then, the directory's accuracy depends on the manual verification process described above, by design.

---

*This is a living document and will be revised as the data pipeline evolves.*
