---
name: client-war-room-memory
description: Opens and maintains a living second brain for each client — the war room — holding every document, conversation, decision, and open item from intake forward. Use at intake for every new client, whenever documents or meeting notes arrive, whenever anyone asks "what do we know about this client," and as the memory layer every other skill reads from and writes to. If a client project exists, this skill governs how it stays organized; if one doesn't, this skill creates it.
---

# Client War-Room Memory

**Stage:** 1 · Trigger — foundation for everything downstream
**Source:** Eric Story §2.1(b) — primary
**Version:** v0.5 DEEP DRAFT — process skill; near-final. Extraction session confirms conventions, doesn't create them.

## What it does

Fixes the audit's critical pain: *no centralized client profile, no institutional memory — context lives in OneNote (sometimes deleted), Plaud, email, and the partner's head.* Every client gets one project (the war room) with a standard structure, and this skill keeps it current so any partner can open it and be sharp in five minutes.

## War room standard structure

```
/00-profile        Client Profile (living doc — see below)
/01-financials     Statements, returns, QuickBooks exports, normalized workbooks
/02-meetings       Notes + Plaud transcripts, one file per meeting, dated
/03-analysis       Smell-tests, benchmarks, classifications, valuations
/04-deliverables   Everything sent to the client, as sent
/05-correspondence Key email threads, decisions made in writing
/06-open-loops     Managed by Open-Loop Tracker
```

## The Client Profile (the skill's core artifact)

A single living document, updated on every material event:

- **Snapshot:** entity, ownership, industry/NAICS, size, service lines engaged, relationship owner, key contacts
- **The goal:** what the owner actually wants, in their words, dated — and how it has shifted
- **Posture:** current Buyer/Seller classification and date, if run
- **Timeline:** dated log of material events — engagements opened, decisions made, deliverables sent
- **Relationships:** who at CN knows them, cross-service-line touchpoints (tax, wealth, A&A)
- **Watch items:** sensitivities, family dynamics, what not to bring up cold

## Process

1. **Intake:** on any new client or engagement, create the war room, populate the profile from intake materials, run the Data Request Checklist.
2. **Ingest:** new document → filed to the structure, profile timeline updated in one line. New meeting → notes to /02, decisions and next steps routed to Next-Step Assigner, open items to Open-Loop Tracker.
3. **Answer:** "what do we know" questions get answered from the profile + timeline first, with pointers into source files — never from memory of a memory.
4. **Maintain:** anything filed loose gets refiled; duplicate or stale profile facts get corrected with a dated note, not silently overwritten.

## Output

The war room itself, and on request: a client one-pager (profile snapshot) for any partner walking into a meeting cold — which is also the input Meeting Re-Context builds from.

## Guardrails

- One war room per client. Fragmenting context across chats/projects recreates the disease this cures.
- The profile records **who said what, when** — attribution matters when goals shift.
- Nothing deleted: superseded facts are struck through with a date, preserving the history OneNote used to lose.
- Client data stays in the war room; cross-client questions route through Cross-Service-Line Integrator with its confidentiality rules.

## Extraction session agenda — Eric (30 min, confirmation not creation)

1. Confirm/adjust the folder structure against how Engagement Manager, ShareFile, and Go File Room are actually used — what stays in those systems vs. lives in the war room.
2. The profile fields Eric would add or cut; what he wishes he'd known walking into his last five client meetings.
3. Plaud recordings: ingestion path and consent/retention rules.
4. Naming conventions and who owns war-room hygiene per client.
