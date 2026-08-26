---
name: regulatory-change-checker
description: Flags tax-law and regulatory changes that affect a specific client and the questions worth revisiting because of them. Use at planning season kickoff, when major legislation or IRS guidance lands, when a client's fact pattern touches an area that changed, or on a recurring cadence across the tax book. SURFACES, NEVER CONCLUDES — output maps changes to affected clients as questions for partner review.
---

# Regulatory Change Checker

**Stage:** 3 · Diagnostic Discovery
**Source:** Scott Nielson §2.1(c) — primary · Monte Morris — contributing practitioner (named on the skill map for this skill)
**Version:** v0.1 SCAFFOLD — matching mechanics functional; monitoring scope and client-mapping rules pending extraction.

## PARTNER GATE

**Surfaces, never concludes.** The skill maps changes to client fact patterns and raises questions. It does not interpret new law beyond sourced summaries, does not advise, and nothing reaches a client without partner ownership.

## What it does

Turns "the law changed" into "these eleven clients are affected, here's the question for each." Watches the change landscape relevant to CN's book and cross-references war-room fact patterns so nothing expires or lands unnoticed.

## Inputs

- Change sources: federal legislation, IRS guidance and rev procs, Idaho and relevant state changes `[EXTRACT: CN's state footprint list; which research services the firm subscribes to (RIA/CCH/etc.) so citations use them]`
- War-room fact patterns across the tax book (entity types, industries, elections in place, transactions pending)
- Monitoring scope `[EXTRACT: Scott/Monte's beat — which areas they track closely vs. rely on service alerts for]`

## Process

1. Ingest a change (or run a periodic sweep) — capture: what changed, effective dates, sunset dates, cited source.
2. Match against the book: which clients' fact patterns touch the change `[EXTRACT: the matching rules — what client attributes the tax team indexes on today, even informally]`.
3. Per affected client: the revisit question ("Client uses X method — does the change to Y warrant revisiting?"), timing (act-by date), and the partner who owns the relationship.
4. Batch into the planning-season worklist or an immediate alert if deadline-driven.

## Output

Change briefs (what changed, source, who's affected, questions, deadlines) + per-partner worklists. Every legal statement carries its citation; no citation, no claim.

## Guardrails

- Sourced summaries only — the skill quotes and cites; interpretation is the partner's.
- Deadline flags err early: a premature reminder costs a minute, a missed election costs a client.
- Sunset tracking is explicit: provisions in current returns with expiration dates get standing entries.

## Extraction session agenda — Monte primary (45 min), Scott validates scope (15 min)

1. The current-events workflow today: how changes reach the team, and what slips past.
2. The client-attribute index: what would the team need tagged per client to make matching real (feeds §2.9 data-team work).
3. This year's live examples: two changes that mattered to the book — walk the ideal alert for each.
4. Cadence: weekly sweep? Monthly? Tied to IRS release rhythm?
