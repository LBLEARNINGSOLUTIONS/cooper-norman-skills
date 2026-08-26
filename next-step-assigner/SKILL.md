---
name: next-step-assigner
description: Captures the decisions made in a meeting and assigns dated next steps with owners. Use immediately after every client or internal meeting — from notes, a Plaud transcript, or a partner's verbal recap — whenever someone says "capture the action items," or when a meeting ends without clear ownership. Every meeting in an advisory engagement should end with this skill having run.
---

# Next-Step Assigner

**Stage:** 6 · The Conversation
**Source:** Eric Story §2.1(b) — primary
**Version:** v0.5 DEEP DRAFT — process skill; near-final. Extraction confirms conventions.

## What it does

Ends the pattern where decisions live in a partner's head or a OneNote page that gets deleted. Takes meeting output and produces the decision log and action list — every step with an owner, a date, and the client-visible vs. internal distinction — filed to the war room and fed to the Open-Loop Tracker.

## Inputs

- Meeting notes, Plaud/Gemini transcript, or partner dictation
- War-room context: the engagement, existing open loops, prior commitments

## Process

1. Extract three things, kept strictly separate:
   - **Decisions made** — what was agreed, by whom, exactly as stated
   - **Next steps** — action · owner · due date · CN-side or client-side
   - **Parking lot** — raised but unresolved → routed to Open-Loop Tracker
2. Infer owners and dates only when explicit ("Scott will send by Friday" → assigned); ambiguous items go to a "needs owner" list for the partner — the skill never invents a commitment.
3. Cross-check against existing open loops: mark any that this meeting closed, and surface prior commitments that went unmentioned.
4. File to war room /02-meetings; update the Client Profile timeline in one line; push steps to the Open-Loop Tracker.
5. Draft the client-facing recap email (decisions + their action items + ours) for partner review.

## Output

Meeting record (decisions · steps · parking lot), updated open-loop list, and a ready-to-send recap draft in the partner's voice.

## Guardrails

- **Decisions are quoted, not paraphrased**, when stakes are material — a misremembered decision is worse than none.
- Client-side action items appear in the recap draft; internal notes never do. The skill enforces the boundary.
- No step exists without an owner or a "needs owner" flag. Unowned steps are how things slip.
- The recap draft is sent by the partner, never automatically.

## Extraction session agenda — Eric (20 min, can share a session with War-Room Memory)

1. His current post-meeting routine and where it breaks under load.
2. Recap email voice: two real examples.
3. Due-date defaults when a meeting sets none (one week? next meeting?).
4. Which meetings warrant this treatment vs. a one-line log entry.
