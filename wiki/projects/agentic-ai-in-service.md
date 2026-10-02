---
title: Agentic AI in service
type: project
created: 2026-10-02
updated: 2026-10-02
sources: [raw/alpstein/2026-05-05-strategy-memo-service-first.md, raw/alpstein/2026-08-21-kickoff-notes-agentic-ai-pilot.md]
tags: [project, ai, service]
---

# Agentic AI in service

**Status (as of 21 August 2026):** Approved and started – kickoff on 21 August 2026; pilot September to November 2026; budget CHF 180,000 approved. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])

## Description

An AI agent ("service triage agent") reads incoming service tickets from [[alpmind]] and the email mailbox, classifies them (fault, maintenance, question, complaint), resolves standard cases with an answer from the knowledge base (pilot: suggestion only, a human approves) and forwards everything else to a human. Initiative 3 of the [[service-first-strategy]]. (Source: [[2026-05-05-strategy-memo-service-first]]) (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])

> [!warning] Contradiction – may the agent resolve cases directly?
> Strategy memo (5 May 2026): the agent should "resolve standard cases directly" (Source: [[2026-05-05-strategy-memo-service-first]]).
> Kickoff rules, first draft (21 August 2026): suggest an answer – **a human approves**; sending an answer directly to customers – **no** in the pilot phase (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]]).
> Not resolved.

## Goal and figures

- Response time in the standard case: under 10 minutes (goal); today 3 hours on average (as of 21 August 2026). (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Budget: CHF 180,000 – requested 5 May 2026 (Source: [[2026-05-05-strategy-memo-service-first]]), approved as of 21 August 2026 (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]]).

> [!warning] Contradiction – pilot start
> Strategy memo (5 May 2026): "Pilot from August 2026" (Source: [[2026-05-05-strategy-memo-service-first]]).
> Kickoff notes (21 August 2026): "Pilot duration: September to November 2026" (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]]).
> Not resolved.

## People

- Project lead: [[jonas-weber]]; technology: [[priya-raman]]. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Team: [[nadia-frei]] (Service Desk), [[lukas-amrein]] (software development); [[marco-steiner]] as guest (finance). (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])

## Rules – what the agent may do (first draft, 21 August 2026)

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

## Architecture

- One agent, no multi-agent solution in the pilot. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Knowledge base: service manuals and the last 2,000 resolved tickets, prepared as a wiki. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Every action of the agent is logged; the log is part of the evaluation. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- After the pilot: a checker agent that checks suggestions against the rules before a human sees them. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])

## Risks

- Liability: if the agent makes a wrong commitment in service, Alpstein is liable – clear rules needed. (Source: [[2026-05-05-strategy-memo-service-first]])

## Next steps

- 5 Sep 2026: finalize rule set – [[jonas-weber]], [[nadia-frei]]
- 12 Sep 2026: quality measurement concept – [[nadia-frei]]
- 15 Sep 2026: data protection clarification – [[priya-raman]]
- 19 Sep 2026: build knowledge base – [[lukas-amrein]]
- 30 Sep 2026: status report to the Executive Board – [[jonas-weber]]

(Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])

## Open points

- Responsibility if a misclassified ticket prolongs a downtime. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Quality measurement beyond speed (proposal: 10% sample). (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- May customer data from tickets go into the language model? (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Fallback to today's process must be possible at any time. (Source: [[2026-08-21-kickoff-notes-agentic-ai-pilot]])
- Whether the next steps (due September 2026) were completed is not in the wiki.

## Related

- [[2026-05-05-strategy-memo-service-first]] · [[2026-08-21-kickoff-notes-agentic-ai-pilot]] · [[alpcare]] · [[bergland-logistik-ag]]
