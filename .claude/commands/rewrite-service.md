---
description: Run the rewrite pipeline (analyst → writer → SEO) on a service page using the reviewed research document. Run /research-service first.
argument-hint: <service-name> <path-to-page>
---

## Task

Run the full rewrite pipeline for "$ARGUMENTS" on switch-to.eu.

## Prerequisites

The research document should exist at `.research/[service-name].md`.
If it doesn't, stop and tell me to run `/research-service` first.

## Pipeline — run these agents in sequence

### Stage 1: Analysis & Fact-Check

Use the **content-analyst** agent.

Input: research document + existing page.
Output: `.research/[service-name].brief.md`

After the analyst finishes, summarize:
- Fact-check results (how many claims correct/wrong/outdated/unverified)
- What's being added
- What's being removed or corrected

### Stage 2: Writing

Use the **content-writer** agent.

Input: content brief + research document + existing page.
Output: updated page (saved in place) + `.research/[service-name].changelog.md`

After the writer finishes, summarize:
- Sections changed vs kept
- Word count before and after

### Stage 3: SEO Optimization

Use the **seo-optimizer** agent.

Input: updated page.
Output: page with SEO improvements (saved in place) + changes appended to changelog.

After the optimizer finishes, summarize:
- What SEO changes were made
- Primary keyword targeted

## After all stages complete

1. Show a final summary:
   - Research: [x] sources, [y] evidence items
   - Fact-check: [x] correct, [y] corrected, [z] unverified
   - Writing: [sections changed], [word count change]
   - SEO: [changes made]

2. Create a git commit:
   "content: update [service-name] — researched, fact-checked, rewritten, SEO optimized"

3. Tell me: "Pipeline complete. Review the page and trace any changes via:
   - `.research/[service-name].md` (research with evidence table)
   - `.research/[service-name].brief.md` (analyst brief with fact-check)
   - `.research/[service-name].changelog.md` (all changes made)"
