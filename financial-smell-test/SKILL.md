---
name: financial-smell-test
description: Scans a client's financials the way a senior partner would on day one, flagging what is unusual and the few items that matter most. Use the moment financials land in a war room, before any deep analysis, when a partner asks "anything jump out?", or at the start of Diagnostic Discovery on every engagement. Built from Eric Story's 12-step diagnostic — the financials-first read that opens every advisory conversation.
---

# Financial Smell-Test

**Stage:** 3 · Diagnostic Discovery
**Source:** Eric Story §2.1(b) — primary (the 12-step diagnostic)
**Version:** v0.1 SCAFFOLD — generic senior-partner checks functional; **the 12 steps themselves are the extraction target and the whole point.**

## What it does

The day-one read: not an audit, not a valuation — the experienced-eye pass that says "these three things are unusual, this one matters, ask about that loan." Output is a short flag list with the questions each flag raises, feeding the structured diagnostic conversation.

## Inputs

- Financials as they arrive (messy is expected — this runs before the Normalizer)
- Prior-year comparatives and tax returns if in the war room
- Industry context if known (full benchmarking comes later)

## Process

`[EXTRACT: Eric's 12 steps, in order, with what he looks at and what "unusual" means at each step. The v0.1 placeholder below is a generic senior-partner read — it must be replaced by Eric's actual sequence, which is the methodology being bought.]`

v0.1 placeholder sequence: 1 revenue trend vs. story · 2 gross margin stability · 3 owner comp and distributions pattern · 4 balance-sheet debt vs. P&L interest sanity · 5 working capital direction · 6 related-party items · 7 expense categories out of proportion · 8 cash vs. accrual artifacts · 9 concentration signals · 10 one-time items · 11 tax return vs. statement consistency · 12 what's *missing* that should be there.

Each flag gets: what was seen · why it's unusual · the question to ask · which downstream skill it feeds (Normalizer add-back, Benchmark check, Tax Surfacer, or Classifier signal).

## Output

A one-page day-one read: **top 3 items that matter most**, full flag list with questions, and a "clean enough to advise?" gate call — the workflow map's explicit Foundation gate (No → stay in cleanup).

## Guardrails

- Flags are questions, not accusations — phrased for a client conversation, not an audit finding.
- The skill states what it could NOT check (missing documents) so silence is never read as clean.
- Three items max in the headline. A 30-flag list is a data dump, not judgment `[EXTRACT: Eric's prioritization rule for what makes the top 3]`.

## Extraction session agenda — Eric (60 min — highest-priority §2.1(b) session)

1. The 12 steps, in his order, with a real (sanitized) financial package on the table — capture what his eye goes to first, second, third.
2. Per step: the threshold between "noted" and "matters."
3. The top-3 rule: how he picks what leads the client conversation.
4. Two war stories where the smell-test caught what the numbers hid — these become the skill's exemplars.
