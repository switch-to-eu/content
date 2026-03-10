---
description: Research a service for switch-to.eu. Outputs a factual research document with evidence table to .research/ for your review before the rewrite pipeline runs.
argument-hint: <service-name> <optional-path-to-existing-page>
---

## Task

Research the service "$ARGUMENTS" for switch-to.eu.

## Steps

1. If a page path was provided, read it to understand what's already covered.
   If no path was given, use Glob to check if a page already exists for this service.

2. Create the `.research/` directory if it doesn't exist.

3. Use the **service-researcher** agent to produce a comprehensive research document.
   The researcher should save its output to `.research/[service-name].md`.

4. After the researcher finishes, print a summary:
   - How many sources were consulted
   - How many evidence items collected (with breakdown by confidence level)
   - Key facts found about privacy & data handling
   - Key facts found about company & ownership
   - Notable Reddit sentiment themes
   - Any gaps where information could not be found

5. Then tell me:
   "Research saved to `.research/[service-name].md`.

   Review it and edit anything that is wrong or missing. Pay special attention to:
   - The Evidence Table (are confidence levels accurate?)
   - Privacy & Data Handling (is anything missing?)
   - Community Sentiment (does it match your experience?)

   When ready, run `/rewrite-service [service-name] [page-path]`
   to continue the pipeline."

## Important

Do NOT proceed to rewriting. Stop after research. I need to review the research
document before the next stages run.
