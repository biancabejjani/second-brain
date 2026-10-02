---
title: Kickoff notes pilot "Agentic AI in service", 21 August 2026
type: source
created: 2026-10-02
updated: 2026-10-02
sources: [raw/alpstein/2026-08-21-kickoff-notes-agentic-ai-pilot.md]
tags: [ai, service, pilot]
---

# Kickoff notes pilot "Agentic AI in service", 21 August 2026

**Raw file:** `raw/alpstein/2026-08-21-kickoff-notes-agentic-ai-pilot.md`
**Date:** 21 August 2026, 14:00–15:30
**Participants:** [[jonas-weber]] (project lead), [[priya-raman]] (technology), [[nadia-frei]] (Service Desk, team lead), [[lukas-amrein]] (software development), [[marco-steiner]] (guest, finance) · **Notes:** [[lukas-amrein]]

## Summary

The kickoff launched the pilot [[agentic-ai-in-service]]: a "service triage agent" reads tickets from [[alpmind]] and the email mailbox, classifies them, suggests answers from a knowledge base and forwards everything else to a human. Goal: response time under 10 minutes in the standard case (today: 3 hours on average). The pilot runs from September to November 2026 with an approved budget of CHF 180,000. A first draft defines what the agent may do; it may never promise a credit note – a lesson from the Bergland case ([[bergland-logistik-ag]]). Four open questions concern liability, quality measurement, data protection and fallback.

## Key points

- Ticket categories: fault, maintenance, question, complaint. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Response time today: **3 hours on average**; goal: **under 10 minutes** in the standard case (as of 21 August 2026). (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Pilot duration: **September to November 2026**. Budget: **CHF 180,000 (approved)** (as of 21 August 2026). (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- [[nadia-frei]]: "The agent may suggest, not promise." (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Architecture ([[priya-raman]]): one agent, no multi-agent solution in the pilot; knowledge base = service manuals + last 2,000 resolved tickets, prepared as a wiki; every action logged; second stage after the pilot: a checker agent. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])

## What the agent may do – first draft

| Action | Allowed? | Comment |
|---|---|---|
| Read and categorize ticket | yes | – |
| Suggest an answer from the knowledge base | yes | A human approves |
| Send an answer directly to customers | **no** (pilot phase) | to be decided after the pilot |
| Give price information | no | Price questions always go to Sales |
| Promise a credit note or compensation | **never** | Lesson from the Bergland case |
| Trigger a technician call-out | suggestion only | Dispatch decides |
| Close ticket | no | – |

(Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])

## People and organizations involved

[[jonas-weber]], [[priya-raman]], [[nadia-frei]], [[lukas-amrein]], [[marco-steiner]], [[alpstein-robotics-ag]].

## Open points

1. Who is responsible if the agent misclassifies a ticket and a downtime lasts longer as a result? ([[marco-steiner]])
2. How to measure quality, not just speed? Proposal [[nadia-frei]]: 10% sample reviewed by the team.
3. May customer data from tickets go into the language model? Data protection clarification by 15 September 2026.
4. Fallback to today's process must be possible at any time.

## Next steps

| What | Who | By |
|---|---|---|
| Finalize the rule set "What the agent may do" | [[jonas-weber]], [[nadia-frei]] | 5 September 2026 |
| Build the knowledge base | [[lukas-amrein]] | 19 September 2026 |
| Data protection clarification | [[priya-raman]] | 15 September 2026 |
| Quality measurement concept | [[nadia-frei]] | 12 September 2026 |
| Status report to the Executive Board | [[jonas-weber]] | 30 September 2026 |

(Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])

> [!warning] Contradiction – pilot start
> Strategy memo (5 May 2026): "Pilot from August 2026" (Source: [[2026-05-05-strategy-memo-service-first]]).
> Kickoff notes (21 August 2026): "Pilot duration: September to November 2026" (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]]).
> Not resolved.
