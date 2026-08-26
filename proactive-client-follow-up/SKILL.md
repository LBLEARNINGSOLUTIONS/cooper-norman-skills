---
name: proactive-client-follow-up
description: Watches for clients who have gone quiet and drafts the follow-up before they slip. Use on a recurring cadence across active war rooms, when a partner asks "who haven't we talked to," when an engagement stalls waiting on client documents, or when a deliverable went out and nothing came back. Turns advisory from an accident into a deliberate trigger — fire it weekly per partner book.
---

# Proactive Client Follow-Up

**Stage:** 1 · Trigger
**Source:** Eric Story §2.1(b) — primary
**Version:** v0.1 SCAFFOLD — mechanics functional; cadence rules and voice pending extraction.

## What it does

Attacks the audit's first pain — *advisory is almost never the front door; opportunities surface by accident* — by making silence a signal. Scans war rooms for staleness and drafts the specific, contextual follow-up a good partner would send, not a generic check-in.

## Inputs

- War-room timelines and open-loop lists across the partner's book
- Staleness thresholds `[EXTRACT: Eric's rhythm — how long is too quiet for an active engagement vs. a recurring tax client vs. a dormant advisory prospect]`
- Trigger events worth a touch: filing deadlines, industry news, benchmark updates, life events noted in the profile `[EXTRACT: which triggers CN considers appropriate vs. salesy]`

## Process

1. Sweep war rooms; flag: engagements stalled on client action, deliverables unacknowledged, relationships past their touch rhythm, open loops aging past threshold.
2. For each flag, pull the context: last conversation, what's pending, the client's stated goal.
3. Draft the follow-up in the partner's voice `[EXTRACT: voice samples per partner — Eric first]` — referencing the specific open thread, never "just checking in."
4. Queue drafts for partner review with a one-line "why now" per client. Partner sends; the skill never sends.

## Output

A weekly follow-up queue per partner: client · why now · draft message · related open loops. Plus a monthly "going cold" report for the book.

## Guardrails

- Drafts only — a partner sends every message. No automated client contact, ever.
- One follow-up per client per cycle; the skill consolidates threads rather than nagging.
- Tone: useful, specific, no manufactured urgency. If there's no real reason to reach out, the honest output is "no touch needed."

## Extraction session agenda — Eric (30 min)

1. His actual follow-up rhythm today: what triggers him to reach out, and what falls through.
2. Cadence by client type — active advisory vs. annual tax vs. dormant prospect.
3. Three real follow-up emails he's proud of (voice calibration).
4. The line between attentive and annoying for CN's client base.
