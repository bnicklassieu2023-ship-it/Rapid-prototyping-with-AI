# Rapid-prototyping-with-AI
Group project

An AI assistant that shows US undergraduates only the jobs and internships they actually fit, verified and explained, with no employer-paid placement.

## How to read this repository

This repository follows the three layers of truth from Session 12.

| Layer | Folder | Question it answers |
|---|---|---|
| Evidence | `evidence-log/` | What do we know, and what supports it? |
| Constitution, v0.1 | `specs/` | What do we build, why, with what, and in what order? |
| Feature specification | `specs/YYYY-MM-DD-<feature>/` | Not started. Session 13 |
| Agent rules | `AGENTS.md`, `agents/persona-agent.md` | How agents work here, and the Persona Agent kept for rehearsal only |

**Start here:** [specs/mission.md](specs/mission.md), then [evidence-log/venture-skeleton-v0.1.md](evidence-log/venture-skeleton-v0.1.md).

## Market scope

The market is the **United States**, decided on 1 October 2026. Europe was dropped. The reasoning, with an evidence label on every line, is in [evidence-log/market-research.md](evidence-log/market-research.md), section 0. Two funnels: without university partnerships (about 1,800 students in year one) and with partnerships (about 36,000 active students by year three).

## File index

| File | What it holds |
|---|---|
| `specs/mission.md` | Purpose, promise, non-goals, open questions, every claim labelled |
| `specs/tech-stack.md` | Layers, the AI role, dependencies. Carries open TBDs on purpose |
| `specs/roadmap.md` | Step 1 is the thinnest end-to-end test of the riskiest assumption |
| `evidence-log/opportunity.md`, `opportunity-v02.md` | Original opportunity, then the US market review |
| `evidence-log/jtbd.md` | Current Job to Be Done with evidence status per element |
| `evidence-log/personas/` | 3 selected personas and 6 drafts, US context |
| `evidence-log/user-feedback.md` | Real-user evidence. Renamed from interview-evidence.md on 6 October 2026 |
| `evidence-log/persona-agent-rehearsal.md` | Synthetic Persona session: what it challenged, and why none of it counts as validation |
| `evidence-log/survey.md` | The live survey, its link and decision rules fixed in advance |
| `evidence-log/recruitment.md` | Who we test with, channels, consent, declared sample bias |
| `evidence-log/market-research.md` | Fermi estimate, claim table, alternatives map, both funnels, stress test |
| `evidence-log/ERRC.md` | The Blue Ocean grid, confirmed 6 October 2026, with the rehearsal pressure test |
| `evidence-log/spike-shift-monitor.md` | Technical spike on whether the shift monitor can be built with free data |
| `evidence-log/careers-office-outreach.md` | Script and decision rules for testing the partnership assumption |
| `evidence-log/experiment-card.md` | The test, thresholds, and the decision table with owners and stop conditions |
| `evidence-log/press-release.md` | Working Backwards opener |
| `evidence-log/assumptions.md`, `goals.md`, `ai-usage-log.md` | Assumption map, goals, AI use with student decisions |
| `downloads/` | The 8 course helper prompts plus SKILL.md and AGENTS.md |
| `prototype/` | Prototype v0 and its backup |

## What is still open

The critical test is unfinished: 7 filmed interviews, survey results and 2 careers-office conversations. Nothing in the ERRC grid or either funnel is validated until those land. The constitution has five unanswered tech-stack questions.
