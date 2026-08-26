---
name: valuation-payout-modeler
description: Builds the buyout, valuation, and payout scenarios that today get worked out by hand — payment structures, earnouts, seller notes, equity rollovers — with after-structure proceeds per scenario. Use when a structural option needs numbers behind it, when a partner asks "what would the owner actually walk away with," when modeling a buyout of a partner or shareholder, or in any deal conversation involving payment terms. Pairs with the Structural Options Generator in the Branch stage.
---

# Valuation & Payout Modeler

**Stage:** 5 · The Branch
**Source:** Dan Packard §2.1(a) — primary · Robert Drasso — contributing practitioner
**Version:** v0.1 SCAFFOLD — modeling mechanics functional; CN's deal-model conventions pending extraction.

## What it does

Takes a valuation range and a candidate structure and produces the scenario math: purchase price paths, payment schedules, earnout mechanics, seller financing terms, and — the number the owner actually cares about — estimated net proceeds over time per scenario.

## Inputs

- Valuation Range Developer output (or a partner-supplied range)
- Candidate structure(s) from the Structural Options Generator
- Deal variables: cash at close %, note terms, earnout triggers, rollover equity % `[EXTRACT: the ranges CN treats as market for their deal size band]`
- Known debt payoffs and transaction costs

## Process

1. Build a base model per structure: sources and uses, payment timeline, contingent components.
2. Run scenarios across the valuation range (low/mid/high) and key term variations `[EXTRACT: which variables Dan flexes in front of a client vs. holds fixed — the model Drasso builds by hand today is the template]`.
3. Compute gross → net bridge per scenario: price → debt payoff → transaction costs → tax estimate (flagged for §2.1(c) review, never concluded) → net proceeds by year.
4. Stress the contingent pieces: earnout paid at 0% / 50% / 100%; note default sensitivity.

## Output

A scenario workbook (xlsx) + one-page comparison: per scenario, headline price, cash at close, at-risk components, and estimated net proceeds timeline. Built to be shown to a client with a partner narrating.

## Guardrails

- Tax figures are placeholder estimates marked for tax-partner review — this skill never finalizes a tax number.
- Every scenario states its assumptions on the page it's printed on. No orphan numbers.
- The model shows at-risk dollars honestly (earnouts, notes) — no scenario presents contingent money as certain.

## Extraction session agenda — Robert Drasso primary, Dan validates (60 min)

1. Open the actual spreadsheet from a recent deal: capture structure, formulas, and the outputs the client saw.
2. What's market for CN's deal sizes: cash %, note terms, earnout norms `[capture as defaults]`.
3. The client conversation: which scenario views land, which confuse — and the one number Dan always ends on.
4. Where hand-built models have broken before (the error stories become validation checks).
