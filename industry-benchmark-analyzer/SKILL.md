---
name: industry-benchmark-analyzer
description: Compares a client company against its industry on a percentage basis and flags where it over- or under-performs, using IBISWorld, BVR, and D&B data. Use whenever normalized financials exist and a partner asks "how do they stack up," during Diagnostic Discovery, before a valuation, in benchmarking or KPI conversations, or when a buyer gameplan needs KPI discipline targets. Run after the Five-Year Normalizer on every advisory engagement.
---

# Industry Benchmark Analyzer

**Stage:** 3 · Diagnostic Discovery
**Source:** Dan Packard §2.1(a) — primary · Robert Drasso — contributing practitioner
**Version:** v0.1 SCAFFOLD — comparison mechanics functional; CN's metric selection and interpretation rules pending extraction.

## What it does

Places the client against industry peers the way CN's benchmarking process does today — common-sized comparison against IBISWorld / BVR / D&B references — and turns the gaps into diagnostic questions, not just a table.

## Inputs

- Five-Year Normalizer output (normalized, common-sized statements)
- Industry classification (NAICS) and size band
- Benchmark source data in the war room (IBISWorld/BVR/D&B pulls) `[EXTRACT: which source CN treats as primary per metric, and licensing/access path via the data team]`

## Process

1. Common-size the client (percent of revenue; per-employee where headcount known).
2. Match against industry percentiles for: gross margin, EBITDA margin, labor cost %, occupancy, revenue per employee, working capital days `[EXTRACT: CN's standard metric set — the ones partners actually quote to clients]`.
3. Flag over/under-performance beyond `[EXTRACT: CN's materiality band]`, with direction of trend from the five-year view — a below-median metric improving fast reads differently than one deteriorating.
4. Translate each material gap into the diagnostic question a partner would ask `[EXTRACT: Dan/Eric's gap-to-question patterns — e.g., high labor % → the staffing vs. pricing question]`.

## Output

Benchmark table (client vs. industry percentile per metric, 5-year client trend arrow) + a "where you stand" narrative in plain client language + the diagnostic question list feeding the Smell-Test conversation.

## Guardrails

- State the benchmark source, year, and size band on every table — a benchmark without provenance is an argument waiting to be lost.
- Industry misclassification is the silent killer: confirm NAICS with the partner before the client sees anything.
- Percentile position is context, not verdict — the narrative must say what the number means for this client's goal, or say that it doesn't.

## Extraction session agenda — Dan + Drasso (45 min)

1. Pull a real benchmarking deliverable: which metrics made the page, which were cut, and why.
2. The interpretation layer: for each core metric, what does "high" actually mean in a buy/sell context vs. an operations context?
3. Which industries CN benchmarks most — and where the published data is known to be wrong or thin.
4. How benchmark position feeds the Classifier (does chronic under-performance push toward Seller?).
