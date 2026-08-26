---
name: tax-return-data-extractor
description: Pulls years of tax returns into Cooper Norman's template in minutes instead of hours, structured and ready for staff to verify. Use whenever tax returns land in a war room — onboarding a new client, starting a valuation or advisory engagement that needs return data, or building multi-year comparisons. Trigger on any request to extract, summarize, or spread tax return data. PREPARATION ONLY — this skill extracts and organizes; it never interprets or advises.
---

# Tax Return Data Extractor

**Stage:** 2 · Foundation
**Source:** Scott Nielson §2.1(c) — primary · Monte Morris — contributing practitioner
**Version:** v0.1 SCAFFOLD — extraction mechanics functional; CN's template and verification workflow pending extraction.

## PARTNER GATE

**Preparation only.** This skill extracts and structures data. Every output is labeled "prepared for staff verification." It draws no conclusions, computes no positions, and gives no advice. Professional judgment stays exactly where it belongs.

## What it does

Converts stacks of returns (1040, 1120, 1120-S, 1065, state) into the firm's structured template: multi-year, line-referenced, cross-tied — the hours of manual spreading collapsed to minutes plus a verification pass.

## Inputs

- Return PDFs in the war room (any mix of years and entity types)
- CN's spreading template `[EXTRACT/COLLECT: the actual template Scott's team fills today — this defines the output format; get the file, then confirm field mapping with Monte]`

## Process

1. Identify each document: form type, tax year, entity, preparer.
2. Extract per CN's template mapping `[EXTRACT: which lines/schedules matter per form type — income detail, officer comp, depreciation, K-1 flows, balance sheet Sch L, M-1/M-2 items]`.
3. Cross-tie automatically: year-over-year continuity (retained earnings roll, depreciation schedules), federal-to-state consistency, K-1 flows to owner returns where both exist.
4. Flag, never fix: unreadable fields, missing schedules, cross-tie breaks — each flagged with page reference for the verifier.
5. Output the populated template + verification checklist (every extracted figure with source page link; every flag listed first).

## Output

CN-template workbook (xlsx), multi-year, with a verification cover sheet: extraction confidence per section, flags, and sign-off lines for staff verification. Feeds Five-Year Normalizer and Smell-Test once verified.

## Guardrails

- Nothing downstream consumes unverified extractions — the workbook carries UNVERIFIED status until staff sign-off.
- Ambiguity is flagged, not resolved: the skill never guesses a number.
- No tax positions, no observations about planning opportunities — items that look like opportunities route to Tax-Strategy Surfacer *after verification*, not from this skill.

## Extraction session agenda — Monte Morris primary (45 min) · Scott confirms template authority (15 min — protect this; without at least one real Scott touchpoint, §2.1(c) is Monte's methodology with Scott's name on it)

1. Get the actual spreading template and a completed example (sanitized).
2. Field-by-field mapping walkthrough for the common forms; which schedules staff always pull and which they skip.
3. The verification workflow today: who verifies, what they check first, the error patterns they catch.
4. Volume and shape: typical years-per-client, entity mixes, the messiest return package they've spread this year.
