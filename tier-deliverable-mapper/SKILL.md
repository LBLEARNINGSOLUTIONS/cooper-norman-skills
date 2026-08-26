---
name: tier-deliverable-mapper
description: Recommends the right service tier (Gold / Silver / Bronze) and maps the full deliverable set for an advisory or M&A engagement from the classification, goals, and scope signals. Use when an engagement is being scoped, when a partner asks "what tier is this" or "what are we actually delivering," before the Engagement Letter Generator runs, or whenever scope creep makes the deliverable list fuzzy mid-engagement.
---

# Tier & Deliverable Mapper

**Stage:** 5 · The Branch
**Source:** Daniel Hopkins §2.1(d) — primary (already self-built a version — start from his work, don't rebuild)
**Version:** v0.1 SCAFFOLD — mapping structure functional; the tier tracker and catalog content pending collection from Hopkins.

## What it does

Scopes the engagement against CN's tiered service catalog: recommends Gold/Silver/Bronze, lists the exact deliverables that tier includes for this engagement type, and flags what the client's situation needs that the tier doesn't cover (the honest upsell/downsell conversation).

## Inputs

- Classifier output and diagnostic notes (complexity signals: entity count, transaction ambition, timeline)
- The tier definitions and 10-phase service catalog `[COLLECT: the existing tier tracker — Hopkins has built this; ingest his artifact as the source of truth rather than re-deriving it]`
- Client budget signals and the partner's read on relationship depth

## Process

1. Score engagement complexity `[EXTRACT: Hopkins' scoping factors — what actually pushes an engagement up a tier in practice]`.
2. Recommend tier with reasoning; show the adjacent tiers and exactly what changes between them (clients buy the delta, not the label).
3. Map deliverables: per catalog phase, what this engagement gets, sequenced against the engagement timeline.
4. Flag mismatches both directions: needs the tier doesn't cover (scope conversation now, not in month three) and tier contents this client won't use (the "no yellow-brick-road" check — Dan's explicit concern that the tracker is prescriptive; the skill must support tailoring, not enforce the menu).

## Output

A scoping memo: recommended tier · deliverable map with sequence · deltas vs. adjacent tiers · mismatch flags — feeds directly into the Engagement Letter Generator.

## Guardrails

- The tier is a recommendation with reasoning; the partner sets the price and the promise.
- Deliverable list must be complete-or-flagged: an engagement letter built from a partial map is a dispute waiting for month six.
- Tension between standardization (the tracker) and tailoring (Dan's view) is resolved per-engagement by the partner — the skill presents both honestly.

## Extraction session agenda — Daniel Hopkins (45 min — also the pattern-review session for what he's already built, §2.6)

1. Walk his self-built version: what it does, what he wants it to do, what to keep verbatim.
2. Collect the tier tracker and service catalog artifacts.
3. Tier judgment: three recent engagements — why each landed in its tier; the borderline call he'd make differently now.
4. How he handles the standardization-vs-tailoring tension with Dan in real scoping conversations.
