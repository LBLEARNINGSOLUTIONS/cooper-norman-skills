---
name: cim-teaser-builder
description: Builds the teaser and CIM (Confidential Information Memorandum) positioning materials for a sell-side engagement from the business's numbers and story. Use when a Seller engagement reaches go-to-market: drafting a blind teaser, assembling a CIM, or positioning a business for buyers. Trigger on "teaser," "CIM," "marketing the business," "buyer packet," or Conversation-stage work on any sell-side M&A engagement.
---

# CIM & Teaser Builder

**Stage:** 6 · The Conversation
**Source:** Dan Packard §2.1(a) — primary
**Version:** v0.1 SCAFFOLD — document structure functional; CN's positioning voice and buyer-psychology judgment pending extraction.

## What it does

Drafts the two go-to-market documents from material already in the war room: a blind teaser (one page, anonymized) and a CIM skeleton populated with the normalized financials, growth story, and positioning angles — so the partner edits instead of assembling.

## Inputs

- Five-Year Normalizer output and Valuation Range (numbers must be final before positioning starts)
- Classifier + diagnostic notes (the story: why sell, why now, what a buyer is really buying)
- Data Request items: customer contracts, employee census, facility/lease detail
- CN brand templates via Branded Report Generator

## Process

1. **Teaser:** industry, size band, headline financials, 3–4 investment highlights, anonymized to survive a small-market guessing game `[EXTRACT: Dan's anonymization standard for the Idaho market — what detail has burned confidentiality before]`.
2. **CIM:** build from CN's section structure `[EXTRACT: the CIM outline Dan uses — or the best past CIM as template]` — business overview, market, financial summary with add-back bridge, growth opportunities, transition/transferability story.
3. Position, don't inflate: every claim in the highlights ties to a number or documented fact in the war room.
4. Flag the weak spots a buyer will find (concentration, owner dependence) and draft the honest framing for each `[EXTRACT: how Dan pre-frames known weaknesses]`.

## Output

Teaser (one page, branded) + CIM draft with all sections populated or explicitly stubbed, plus an internal "exposure list" of the weaknesses a diligence process will surface and the prepared responses.

## Guardrails

- Nothing in the teaser or CIM may contradict the normalized financials — one inconsistent number kills credibility for the whole document.
- Confidentiality first: teaser drafts are reviewed against the anonymization standard before anything leaves the war room.
- Add-backs presented to buyers must be the documented ones only (Five-Year Normalizer's "proposed" column never ships).

## Extraction session agenda — Dan (45–60 min)

1. Pull the best teaser and CIM CN has produced: what makes them work; capture structure and voice.
2. Buyer psychology for CN's market: what the first-page read must accomplish; what kills interest instantly.
3. The anonymization line in a small market — stories of leaks or near-misses.
4. How he frames the three most common weaknesses (owner dependence, concentration, thin management).
