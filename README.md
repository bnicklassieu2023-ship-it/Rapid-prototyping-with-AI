# Rapid-prototyping-with-AI
Group project

An AI assistant that shows US undergraduates only the jobs and internships they actually fit, verified and explained, with no employer-paid placement.

## What changed after the graded feedback, 7 October 2026

The previous submission scored 5.68 out of 8. Every criterion the professor marked Revise or Rework is answered below, with the file that answers it. Nothing here is a plan to fix something later.

| Criterion | What the feedback said | What we did |
|---|---|---|
| **Venture chain**, 0.36/0.4 | Trust and intended use are mixed together. Choose one and carry it through the test and decision rule | Chose **trust**. The word "use" is gone from the assumption, the sprint goal, the metric and the decision rule. One claim runs end to end: [venture-skeleton-v0.1.md](evidence-log/venture-skeleton-v0.1.md) v0.2 |
| **Riskiest Assumption**, 0.62/0.8 | Choose either trust or intended use, then explain why that one matters most | [assumptions.md](evidence-log/assumptions.md) v0.3. Four reasons for trust over intended use, including that intended use is downstream and that our whole ERRC grid is a trust strategy |
| **Experiment fit**, 0.8/1.6 | You designed a runnable test but have not run it. Make the metric measure one thing | One metric, the **fit rate**, with a threshold fixed before anyone saw the prototype: [experiment-card.md](evidence-log/experiment-card.md) v0.2. And **two tests have now actually been run**, with results, in [evidence-log/test-runs/](evidence-log/test-runs/) |
| **Rough Test**, 0/0.8 | Add the actual rough prototype and a backup. The README lists files to add but they are not there | [prototype/index.html](prototype/index.html) is a working prototype with six real, verified openings and built in scoring. The PDF and PNG are the backup. The old "files to add" README is gone |
| **Traceability**, 0.4/0.4 | Records are consistent and show test access and checks completed | Kept, and extended: every test run names who ran it, on what date, and what the result was, including the results that went against us |
| **Explanation**, 3.5/4 | Test whether the idea already exists and what differentiates you. How do you handle privacy and data sharing? You do not need a build to start testing | [Test run 02](evidence-log/test-runs/run-02-does-this-already-exist.md) checks each incumbent against our two strategic moves. [privacy.md](evidence-log/privacy.md) takes a data position and separates what is built from what is only claimed. The prototype is hand picked with no algorithm behind it, which is the cheapest possible build |

### The three things our own tests found that work against us

A test that only confirms what you hoped is not a test. These are in the repository because they happened, not despite happening.

1. **Our AI failed the one check the product exists to make.** Asked to judge whether 12 job postings were still open, the model got 2 of the first 3 wrong. The "still open" check has been taken away from the model entirely. [Test run 01](evidence-log/test-runs/run-01-shortlist-feasibility.md)
2. **Our university price is contradicted, not just unproven.** We assumed about 18,000 dollars a year. Handshake charges universities about 8,000 for a system that replaces their whole careers stack. Funnel B's revenue line has to be rebuilt or defended. [Test run 02](evidence-log/test-runs/run-02-does-this-already-exist.md)
3. **Verification is a cost we never priced.** Twelve page checks produced five usable openings. It appears nowhere in either funnel.

### Still not done, stated plainly

The student trust test has **not** been run. 0 of 7. The prototype, the scoring sheet, the protocol and the threshold all exist; the students do not yet. Nothing in this repository treats the riskiest assumption as tested until that table has five rows. Same for the two careers office conversations, 0 of 2.


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
| `prototype/index.html` | **The working rough prototype v0.2**, six real verified openings, fit rate scored in the page |
| `prototype/` | The v0.1 PDF and PNG backups, and the scoring sheet |
| `evidence-log/test-runs/` | **Every test we have actually run**, with raw data, and the ones still owed |
| `evidence-log/privacy.md` | Our data and privacy position, built parts separated from claimed parts |

## What is still open

The critical test is unfinished: 7 filmed interviews, 2 careers-office conversations, and the second round of survey responses. Survey round 1 has been read and is in evidence-log/survey.md: n=4, too small to settle anything, and it already works against our push force. Nothing in the ERRC grid or either funnel is validated until those land. The constitution has five unanswered tech-stack questions.
