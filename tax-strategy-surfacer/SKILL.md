---
name: tax-strategy-surfacer
description: Surfaces the structuring and planning considerations worth a tax partner's attention from a client's facts — entity structure, transactions in motion, return data, life events. Use during Diagnostic Discovery, when a structural option needs its tax dimension flagged, when returns are verified and planning season approaches, or when anyone asks "any tax angles here?" SURFACES, NEVER CONCLUDES — output is a partner attention list, not advice.
---

# Tax-Strategy Surfacer

**Stage:** 3 · Diagnostic Discovery
**Source:** Scott Nielson §2.1(c) — primary · Monte Morris — contributing practitioner
**Version:** v0.1 SCAFFOLD — surfacing framework functional; CN's consideration catalog pending extraction.

## PARTNER GATE

**Surfaces, never concludes.** Output is a list of considerations for a tax partner's judgment, each phrased as a question with the facts that raised it. The skill never quantifies a benefit, recommends a strategy, or communicates tax matters to a client. The partner's judgment makes every call.

## What it does

Reads the war room the way a tax partner skims a new file — entity choices, comp patterns, depreciation posture, state footprint, transactions coming — and lists what deserves partner attention this year, with the why attached.

## Inputs

- Verified return data (Tax Return Data Extractor output post-verification)
- War-room context: posture, structural options in play, life events, stated goals
- Consideration catalog `[EXTRACT: Scott's checklist — the things he looks for by client type; the v0.1 categories below are generic and must be replaced/ranked by his actual practice]`

## Process

1. Scan facts against the catalog. v0.1 generic categories: entity structure fit · owner comp reasonableness (S-corp) · accounting method opportunities · depreciation/179/bonus posture · state nexus and footprint changes · retirement plan capacity · succession/gifting signals · transaction-driven items (structure of a pending sale, QSBS-type questions, installment treatment) · credits likely missed `[EXTRACT: which of these Scott actually hunts, what he'd add, and his priority order]`.
2. For each hit: the fact pattern seen · why it may matter · the question for the partner · deadline sensitivity if any.
3. Rank by `[EXTRACT: Scott's triage — dollars at stake? deadline? client relationship moment?]`.
4. Route to the tax relationship owner; log to the Client Profile that the surface ran (not its contents — see guardrails).

## Output

A partner attention memo: ranked considerations, each with facts, question, and timing flag. Explicitly headed: *"Considerations for professional review — not advice, not conclusions."*

## Guardrails

- No numbers on benefits. "May warrant review of X" — never "would save $Y."
- Nothing from this skill reaches a client in any form until a partner has made it their own.
- Regulatory-change items come from Regulatory Change Checker with citations; this skill doesn't freelance on law.

## Extraction session agenda — Scott Nielson (45 min minimum, direct — this session is the difference between Scott's methodology and Monte's with Scott's name on it) + Monte follow-up

1. Scott's skim: new client file on the table — what does he look at, in what order, and what makes him stop?
2. The catalog: his actual hunt list by client type (operating business, real estate, farm/ranch, professional practice).
3. Triage: what makes a consideration urgent vs. annual-review material.
4. The considerations most often missed by less experienced staff — the ones this skill exists to stop missing.
