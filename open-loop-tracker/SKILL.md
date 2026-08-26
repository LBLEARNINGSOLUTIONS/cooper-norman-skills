---
name: open-loop-tracker
description: Tracks every open decision, missing document, and unresolved risk across meetings and brings them back until closed, so nothing slips between sessions. Use continuously across every war room — fed by the Next-Step Assigner after meetings, checked by Meeting Re-Context before them, and swept on a weekly cadence per partner. Trigger on "what's outstanding," "what are we waiting on," or any status question about an engagement.
---

# Open-Loop Tracker

**Stage:** 7 · Sticky Relationship
**Source:** Daniel Hopkins §2.1(d) — primary
**Version:** v0.5 DEEP DRAFT — process skill; near-final. Extraction calibrates thresholds and escalation, doesn't create structure.

## What it does

The persistence layer for everything unresolved. Advisory relationships span months and service lines; this skill guarantees that a decision deferred in March resurfaces in June instead of dying in a notebook.

## Loop types and data model

Every loop: type · description · origin (meeting/date it opened) · owner (CN person or client) · due or review date · status · staleness · blocking (what it holds up).

- **Open decisions** — raised, discussed, not decided ("owner hasn't chosen between the ESOP and the third-party sale")
- **Missing documents** — requested, not received (auto-created from Data Request Checklist gaps)
- **Commitments** — promised by CN or by the client (from Next-Step Assigner)
- **Unresolved risks** — flagged in analysis, not yet addressed ("customer concentration raised in the smell-test, no mitigation discussed")
- **Deferred items** — consciously parked, with a wake-up date ("revisit gifting after year-end")

## Process

1. **Intake:** loops arrive from Next-Step Assigner, Data Request Checklist, analysis skills, or direct partner entry. Duplicates merge; every loop keeps its origin reference.
2. **Age:** staleness computes from due/review dates. Aging tiers: current → needs attention → overdue → critical `[EXTRACT: Hopkins' thresholds per loop type — a missing document goes stale faster than a deferred decision]`.
3. **Resurface:** loops appear in Meeting Re-Context sheets (always), weekly partner sweeps (aging items), and Proactive Client Follow-Up drafts (client-owned items).
4. **Close:** only with a resolution note — what happened, when, recorded on the Client Profile timeline. Loops never silently disappear; abandoned items are closed as "consciously dropped" with a reason.

## Output

Per-war-room loop list (always current), weekly per-partner sweep (aging + critical items across their book), and per-meeting loop extracts via Meeting Re-Context.

## Guardrails

- Every loop has an owner and a date. Ownerless loops are assigned to the relationship partner by default and flagged.
- Closure requires a reason — "handled" without a note is not closure.
- Client-owned loops generate follow-up drafts, never direct client contact.
- The tracker reports, it doesn't nag: one consolidated sweep per partner per week, not per-item pings.

## Extraction session agenda — Hopkins (20 min, calibration)

1. Staleness thresholds per loop type; what "critical" means in his book.
2. The weekly sweep format he'd actually read (and when — Monday morning? Friday close?).
3. Two engagements where something slipped: would this design have caught it? Adjust until yes.
