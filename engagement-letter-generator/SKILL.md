---
name: engagement-letter-generator
description: Drafts the tier-based engagement letter from Cooper Norman's letter library, ready for partner review. Use immediately after the Tier & Deliverable Mapper sets scope, when a partner says "send them the engagement letter," when scope changes mid-engagement and the letter needs an amendment, or when renewal season requires updated letters. Every advisory engagement should start with this skill's output, reviewed and signed.
---

# Engagement Letter Generator

**Stage:** 5 · The Branch
**Source:** Daniel Hopkins §2.1(d) — primary (engagement-letter library referenced in the workflow map)
**Version:** v0.1 SCAFFOLD — assembly functional; letter library and clause rules pending collection.

## What it does

Assembles the engagement letter for the scoped tier: correct template, correct clauses, deliverables straight from the Mapper's output, fees per the tier structure — a review-ready draft in minutes, with every deviation from standard flagged for the partner.

## Inputs

- Tier & Deliverable Mapper output (tier, deliverable list, timeline)
- CN letter library `[COLLECT: the actual templates by engagement type — advisory, valuation, M&A, tax, forensic; plus the AI-use language Eric said the firm now requires in engagement letters]`
- Client entity details from the Client Profile
- Clause rules `[EXTRACT: which clauses flex by engagement type and which never change — limitation of liability, dispute resolution, withdrawal, records]`

## Process

1. Select template by engagement type and tier.
2. Populate: parties, scope narrative from the deliverable map (specific, not boilerplate — the deliverable list IS the scope), fees `[EXTRACT: how tier pricing is expressed — fixed, range, hourly hybrid]`, timeline, responsibilities both directions (client document obligations from the Data Request Checklist).
3. Include the firm's standard protective clauses unmodified; flag any requested deviation in a redline note for the partner — the skill never negotiates clauses silently.
4. Include CN's AI-use disclosure language (Eric's stated requirement from the audit review).
5. Output draft + a one-page cover summary for the partner: scope, fee, deviations from standard, and what the client must provide.

## Output

Review-ready letter (docx) + partner cover summary, filed to the war room; on signature, scope and deliverables auto-log to the Client Profile and Open-Loop Tracker (client document obligations become tracked loops).

## Guardrails

- **Drafts only. No letter leaves without partner review and signature authority.**
- Scope language must match the Mapper's deliverable list exactly — daylight between the letter and the map is how scope disputes start.
- Deviations from the standard library are flagged, never silent.
- Fee figures come from the partner or the tier structure — the skill never invents a price.

## Extraction session agenda — Hopkins (30 min + artifact handoff)

1. Collect the letter library; identify the most-used template per engagement type.
2. The clause map: what's sacred, what flexes, who approves a deviation.
3. Fee expression by tier; how mid-engagement scope amendments are papered today.
4. The AI-use language the firm settled on (or draft it with Eric if it doesn't exist yet — flag to Lyden either way).
