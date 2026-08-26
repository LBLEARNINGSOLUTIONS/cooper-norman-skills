---
name: buyer-seller-classifier
description: Classifies a business owner as a Buyer or Seller posture from their diagnostic answers, behavior, and financials, returning the classification with full reasoning. Use whenever an advisory engagement reaches the point of deciding direction — the owner asks "should I grow or get out," a partner asks which gameplan applies, diagnostic answers are in hand, or anyone mentions buyer/seller classification, exit readiness, succession posture, or the $5M question. This is the pivot of every Cooper Norman advisory engagement; when in doubt about direction, run it.
---

# Buyer / Seller Classifier

**Stage:** 4 · The Pivot — the critical break in the advisory spine
**Source:** Dan Packard §2.1(a) — primary · Robert Drasso — contributing practitioner
**Version:** v0.1 SCAFFOLD — extraction pending. **This is the one skill on the map that cannot be built second-hand.** Dan is the source; Eric and Robert feed live engagement context, but the classification logic must come from Dan's sessions.

## What it does

Reads the owner's situation — diagnostic answers, behavioral signals, and the normalized financial picture — and returns a Buyer (Innovation) or Seller (Invigilation) posture with the reasoning a partner can defend to the client. Diagnosis is by **behavior, not mood**: what the owner has been doing, not what they said they want this week.

## Inputs

- Diagnostic Discovery outputs: Financial Smell-Test flags, benchmark position, owner-goal notes ([EXTRACT: Dan's 40 questions — full list and which answers carry classification weight])
- The $5M coin-flip response ([EXTRACT: exact framing Dan uses, and how each response pattern maps to posture])
- The 10 behavioral indicators ([EXTRACT: the full list from Dan's "Buyer or a Seller" deck, with how many must be present and which are disqualifying])
- Five-Year Normalizer output (trajectory matters to posture)

## Process

1. Score the behavioral indicators against evidence in the war room — meetings, financials, decisions actually made. `[EXTRACT: indicator definitions, evidence standards, weighting]`
2. Apply the $5M test response. `[EXTRACT: interpretation rules, including the ambivalent-answer case]`
3. Run the prepared-vs-unprepared sub-read. `[EXTRACT: what separates a prepared seller from an unprepared one, and how that changes the recommendation — this sub-read is in the deck but the decision rules are Dan's]`
4. Return: posture, confidence, the specific evidence behind each indicator scored, contra-indicators honestly stated, and the recommended gameplan entry point (Innovation 0–6 or Invigilation 0–6 items from the workflow map).

## Output

A one-page classification memo: **Posture · Evidence · Contra-evidence · Prepared/Unprepared read · Recommended gameplan and first three moves.** Written so a partner who is not Dan can walk the client through the reasoning.

## Guardrails

- Never classify on thin evidence — below the evidence threshold `[EXTRACT: Dan's minimum]`, the output is "insufficient signal" plus the specific questions to ask next, not a guess.
- The classification is a partner conversation aid. The partner makes the call with the client; the skill shows its work so the partner can disagree.
- Ambivalence is a finding, not a failure — flag owners who present as both, with the tie-break logic `[EXTRACT]`.

## Extraction session agenda — Dan Packard (2–3 sessions, talking through live and past engagements; he never opens Claude)

1. Walk through the "Buyer or a Seller" deck slide by slide — capture the 10 indicators verbatim and what evidence satisfies each.
2. The $5M question: exact wording, why $5M, and the read on each answer type — including the owner who hesitates.
3. Prepared vs. unprepared: what tips the read, and how the gameplan changes for each quadrant.
4. Two live engagements (with Robert): classify them together out loud; record the reasoning path, not just the answer.
5. The misclassification stories — engagements where the first read was wrong and what signal was missed. These become the skill's contra-indicator checks.
6. The 40 questions: which five actually decide the classification in practice.
