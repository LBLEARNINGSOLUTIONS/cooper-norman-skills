---
name: five-year-normalizer
description: Pulls five years of client financials, normalizes them, and builds the side-by-side growth view used in every Cooper Norman valuation and advisory read. Use whenever multi-year financials arrive in the war room, a partner asks for normalized EBITDA, add-backs, trend or growth analysis, or before running the Financial Smell-Test, Industry Benchmark Analyzer, Buyer/Seller Classifier, or any valuation skill. If five years of statements exist and no normalized view does, run this.
---

# Five-Year Normalizer

**Stage:** 2 · Foundation
**Source:** Dan Packard §2.1(a) — primary · Robert Drasso — contributing practitioner
**Version:** v0.1 SCAFFOLD — mechanics functional; CN's normalization judgment rules pending extraction.

## What it does

Converts five years of raw statements into the normalized, side-by-side view partners actually read: revenue, gross margin, normalized EBITDA, owner-adjusted earnings, and growth rates — with every adjustment documented and tied back to source.

## Inputs

- 5 years of P&L and balance sheets (statements, QuickBooks export, or tax returns via Tax Return Data Extractor)
- Owner compensation detail, related-party items, one-time events noted in the war room

## Process

1. Ingest and map each year to a common chart of accounts `[EXTRACT: CN's standard mapping template — the one Drasso uses on buy/sell engagements]`.
2. Identify normalization candidates: owner comp vs. market, rent vs. market on related-party leases, personal expenses, one-time legal/settlement items, discretionary spend. `[EXTRACT: CN's add-back categories and the evidence standard for each — what counts as documented vs. asserted]`
3. Apply adjustments per year; produce raw → adjusted bridge for every year so nothing is a black box.
4. Build the five-year side-by-side with CAGR, margin trend, and working-capital trend.
5. Flag anomalies for the Smell-Test (year-over-year swings > `[EXTRACT: CN's threshold]`, margin inversions, negative working capital turns).

## Output

A workbook (xlsx) + one-page summary: five-year side-by-side, adjustment schedule with documentation status per add-back, growth view, and an anomalies list routed to Diagnostic Discovery. Every number traces to a source cell or document.

## Guardrails

- **No undocumented add-backs.** An adjustment without support goes in a "proposed — needs support" column, never into normalized EBITDA silently.
- Ties to source: totals must reconcile to the underlying statements; discrepancies are flagged, not plugged.
- Staff verify before partners rely — output states "prepared for verification" until a human initials it.

## Extraction session agenda — Robert Drasso primary, Dan validates (60 min)

1. Walk one completed normalization from a real deal: every add-back taken, every one declined, and why.
2. The add-back fights: which adjustments buyers routinely challenge, and how CN documents to survive that.
3. Owner comp normalization: what market benchmark CN uses and when they deviate.
4. The threshold judgment: how big does an anomaly need to be before it changes the story?
