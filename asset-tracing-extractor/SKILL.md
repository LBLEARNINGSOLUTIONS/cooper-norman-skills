---
name: asset-tracing-extractor
description: Pulls transactions from bank, credit card, and loan statements into structured, reconciled schedules that tie to the ending balance — the foundation of forensic tracing work. Use on any forensic or litigation-support engagement involving statement analysis: divorce tracing, embezzlement investigation, commingling questions, estate disputes. Trigger whenever a folder of statements needs to become a reconciled transaction schedule.
---

# Asset Tracing Extractor

**Stage:** 2 · Foundation
**Source:** ⚠️ **TO DESIGNATE** — no named source. Week-one decision per the Skill Map: name a forensic source, or hold this and Damages Stress-Test for 2027 and build twenty-three.
**Version:** v0.1 SCAFFOLD — extraction/reconciliation mechanics functional; forensic methodology and evidentiary standards pending source designation.

## What it does

Converts raw statements into the working schedules forensic work is built on: every transaction captured, categorized, cross-account flows matched, and each account reconciled so the schedule provably ties to the ending balance — the tedious foundation collapsed to a verification pass.

## Inputs

- Statement PDFs: bank, credit card, loan, brokerage — complete runs for the tracing period, every account
- The tracing question (what the schedules must ultimately answer — separate vs. marital, diverted funds, source of deposits)
- CN's schedule format `[COLLECT: the working schedule template from past forensic engagements — source to provide]`

## Process

1. Inventory coverage: accounts × months; **gaps are finding #1** — a tracing schedule with missing months is an opposing counsel's opening argument.
2. Extract every transaction: date, description, amount, running balance, source page reference.
3. Reconcile per account per period: beginning balance + activity = ending balance, to the penny. Breaks are flagged with location, never plugged.
4. Match cross-account flows (transfers, payments between accounts in the set) `[EXTRACT: matching tolerance and timing-window rules the forensic team uses]`.
5. Categorize per the tracing question's schema `[EXTRACT: category frameworks by case type]` — uncertain items go to an "unclassified — review" bucket, never force-fitted.

## Output

Reconciled transaction workbook (per-account schedules + master), coverage map with gaps, cross-account flow schedule, reconciliation status per account, and an exceptions list — all page-referenced back to source. Labeled "prepared for professional review — not an opinion."

## Guardrails

- **Tie-out is absolute:** an unreconciled schedule ships as UNRECONCILED with the break documented — never silently approximated. This work gets deposed.
- Every figure carries its source-document page reference (evidentiary chain).
- Categorization judgment calls on contested items belong to the professional, not the skill.
- Chain of custody: source files are read-only; the workbook logs what was received, from whom, when.

## Extraction session agenda — pending source designation (candidates: ask Eric which partner/senior runs forensic engagements today; Jordan Graves reached out in June about advisory tooling — worth asking Eric if he's the forensic lane)

1. Collect two completed tracing workbooks (sanitized) — the format is the methodology.
2. Reconciliation and matching standards; how breaks are documented for testimony.
3. Category frameworks by case type (divorce, embezzlement, estate).
4. What opposing experts attack in CN's schedules — those attacks become the skill's self-checks.
