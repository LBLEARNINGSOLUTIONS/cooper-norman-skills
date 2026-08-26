---
name: buyer-seller-database-matching
description: Tracks buyers and sellers across Cooper Norman's deal pipeline over time and surfaces likely matches between them. Use when a new Buyer or Seller classification lands, when a sell-side engagement goes to market and needs a buyer list, when a buy-side client needs acquisition targets, or when anyone asks "who do we know who might want this." The institutional memory that today lives in Dan's head — trigger it whenever a match question comes up.
---

# Buyer / Seller Database & Matching

**Stage:** 7 · Sticky Relationship
**Source:** Dan Packard §2.1(a) — primary
**Version:** v0.1 SCAFFOLD — data model functional; matching judgment and historical seed data pending extraction. **Depends on data-team coordination (§2.9) for pipeline data access.**

## What it does

Maintains a structured record of every buyer and seller the firm touches — classified engagements, inbound interest, deals that didn't close — and surfaces matches when a new mandate arrives. Converts Dan's mental rolodex into a firm asset that survives him.

## Data model (v0.1)

Per party: type (buyer/seller/both) · industry + NAICS · size band (revenue, EBITDA) · geography · posture source (engagement, inquiry, referral) · status (active mandate, watching, dormant, closed) · timeline · key constraints (financing, geography, management depth) · relationship owner · last touch · notes.

## Process

1. **Capture:** every Classifier output and every M&A conversation writes a party record — capture is a side effect of doing the work, not a data-entry task.
2. **Match:** on a new mandate, score the book: industry adjacency, size fit, geography, timing, financing reality `[EXTRACT: Dan's matching heuristics — what makes him pick up the phone; which "obvious" matches he skips and why]`.
3. **Surface:** ranked match list with the reason per match and the relationship owner who should make the call.
4. **Age:** dormant records resurface on triggers (industry transaction activity, timeline maturity `[EXTRACT: Dan's re-contact rhythm]`).

## Output

Match memos on demand (mandate → ranked candidates with reasoning) and a quarterly book review: active buyers, active sellers, aging mandates, matches worth a call.

## Guardrails

- **Confidentiality walls:** a party's record never exposes another client's engagement details in a match memo. Blind profiles until a partner authorizes contact.
- Match suggestions route to the relationship owner — the skill never initiates contact.
- Records carry provenance: where the intel came from and how stale it is.

## Extraction session agenda — Dan (45 min) + data team session (§2.9)

1. Dump the current rolodex: the buyers and sellers Dan is carrying in his head right now, into the data model. This seed data IS the asset.
2. Matching heuristics: walk three matches he's made — why those, and the near-matches he passed on.
3. Deals that died: which parties stay on the list anyway, and what would reactivate them.
4. With Hans/Kameron: where pipeline and practice-management data can seed and update records automatically.
