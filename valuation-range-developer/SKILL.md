---
name: valuation-range-developer
description: Develops a defensible valuation range from comparables and multiples using Cooper Norman's valuation process. Use when normalized financials exist and anyone needs a value indication — pre-sale planning, buyout pricing, gift/estate context, or feeding the Payout Modeler. Trigger on "what's it worth," "valuation range," "multiple," "comps," or any Branch-stage conversation that needs a number band. Produces a range for advisory use, not a formal valuation report.
---

# Valuation Range Developer

**Stage:** 5 · The Branch
**Source:** Dan Packard §2.1(a) — primary · Robert Drasso — contributing practitioner
**Version:** v0.1 SCAFFOLD — method structure functional; CN's multiple selection and adjustment judgment pending extraction.

## What it does

Builds the range CN partners use to anchor deal conversations: normalized earnings base × selected multiples, cross-checked against comparables, with the discount/premium reasoning stated — defensible because every step shows its work.

## Inputs

- Five-Year Normalizer output (normalized EBITDA / SDE, trend)
- Industry Benchmark position (performance vs. peers moves the multiple)
- Comparable data: BVR/DealStats pulls in the war room `[EXTRACT: CN's comp sources and access path]`
- Company-specific risk factors: concentration, owner dependence, transferability

## Process

1. Select the earnings base `[EXTRACT: when CN uses SDE vs. EBITDA vs. weighted average of years — the decision rule]`.
2. Pull comp multiples for industry and size band; note dispersion, not just median.
3. Adjust within the comp range for company factors `[EXTRACT: CN's adjustment framework — how much does customer concentration move the multiple? owner dependence? the prepared/unprepared read from the Classifier?]`.
4. Cross-check: implied value vs. balance sheet reality (asset floor), vs. financeability (could a buyer actually fund this at market debt terms?), vs. revenue multiple sanity check.
5. State the range with the reasoning chain: base × low/high multiple, adjustments applied, cross-checks passed or flagged.

## Output

A valuation range memo: earnings base derivation · comp set with sources · multiple selection reasoning · adjustments · range · cross-checks · "what would move this number" list. Explicitly labeled **advisory range, not a formal valuation opinion**.

## Guardrails

- This is a calculation of value for advisory conversations. If the context is litigation, estate/gift filing, or anything requiring a signed opinion, stop and route to the formal valuation engagement path.
- Comps without provenance don't count. Source and date on every multiple.
- The range honestly reflects dispersion — a false-precision single number is a bug, not a feature.

## Extraction session agenda — Dan + Drasso (60 min)

1. Rebuild the range from a recent engagement: base chosen, comps pulled, adjustments made — capture each judgment.
2. The multiple-adjustment framework: rank the factors that move CN's multiples most, with rough magnitudes.
3. Where advisory ranges have differed from later formal valuations or actual sale prices — and why.
4. The defensibility standard: what does Dan need behind a number before he'll say it to a client's face?
