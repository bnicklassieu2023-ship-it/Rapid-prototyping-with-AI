# Experiment Card

> **Read v0.2 at the bottom of this page first.** Everything between here and the "v0.2" heading is kept on purpose as the version history the course asks for, and it is **superseded**. In particular the riskiest assumption immediately below still reads "trust **and** use", which is the exact wording the graded feedback told us to split. It is left visible so the change is traceable rather than silently rewritten. The current card is [v0.2](#v02-7-october-2026-one-metric).

## Riskiest assumption, v0.1, SUPERSEDED
Users will trust and use AI-generated opportunity recommendations as a first step in their decision process.

## Hypothesis, v0.1, SUPERSEDED
If we show students a simple prototype that asks for their preferences and returns a shortlist with clear explanations, then most of them will say they would use it to narrow down options.

## Smallest falsifiable experiment, v0.1, SUPERSEDED
Show 5-8 target users a rough prototype.

The prototype should:
1. Ask for preferences (career goal, location, budget, field, deadlines, remote/on-site preference).
2. Return 3-5 recommended opportunities.
3. Explain why each recommendation matches.

Then ask users:
- Would you use this as a first filter? Why or why not?
- Which part do you trust the least?
- Would you prefer this over searching manually at the start?

## Success signal
At least 70% of test users say they would use the tool as a first filter for finding relevant opportunities.

## Failure signal
Fewer than 70% say they would use it, or users say they do not trust the recommendations enough to rely on them.

## Decision rule
If at least 70% of users respond positively, continue developing the recommendation concept.
If not, narrow the scope or redesign the trust/explanation mechanism before building more.

## v0.1 (Session 8): revision

**Why revised:** interview 01 (user-feedback.md) linked trust to never seeing an unsuitable job, so the test now also measures match accuracy.

**Riskiest assumption:** unchanged.

**Hypothesis v0.1:** If we show students a shortlist where every job or internship fits their stated profile and interests, then most of them will use it as a first filter.

**Smallest falsifiable experiment:** the same rough prototype with 5 to 8 students aged 19 to 24. Each student enters preferences, receives 3 to 5 recommendations and marks each one as "fits me" or "does not fit me".

**Added question:** "How many unsuitable jobs would it take before you stopped trusting it?"

**Success signal:** at least 70% say they would use it as a first filter (unchanged), and most recommendations are marked "fits me".

**Failure signal:** fewer than 70% would use it, or students reject recommendations as unsuitable and say this breaks their trust.

**Decision rule (pre-committed):**
- If both success signals hold, continue developing the recommendation concept.
- If first-filter use is high but many matches are rejected, improve matching accuracy before building more.
- If students trust accurate matches but still ask for reasons, add the explanation layer.
- Otherwise, narrow the scope or redesign the trust mechanism.

## Decision and next move (Group Project I)

**Status: proposed on 6 October 2026. Dates and owners to be confirmed at the next team meeting.**

| Test | Threshold that decides it | Owner | Date | Stop condition |
|---|---|---|---|---|
| Survey, live since 1 October | 50 responses, read against the rules in survey.md | Linda | Close 13 October 2026 | Under 20 responses by 13 October: report it as a weak sample instead of presenting percentages from a handful of people |
| 7 filmed student interviews | 7 completed and coded into user-feedback.md, including the five questions the Persona rehearsal generated | Linda | 15 October 2026 | Fewer than 5 by that date: present what we have and name the gap on the slide |
| 2 careers-office conversations | At least 1 agrees to a pilot | [team member] | 17 October 2026 | Both decline to add anything alongside Handshake: drop Funnel B from the presentation and say the channel assumption failed |
| Shift-monitor spike | Complete, see spike-shift-monitor.md | Done | Completed 6 October 2026 | Not applicable |

**The decision we are heading to:** does the evidence support continuing with the verified shortlist as Step 1 of the roadmap?

- **Continue** if the survey supports accuracy over explanation and at least 5 interviews show high application volume with poor results.
- **Narrow** if students want fewer bad matches but do not care about verification depth: keep the Reduce row, soften the Raise row, and take verification cost out of the plan.
- **Stop or pivot the channel** if both careers offices decline: the product may survive, but the university route, and therefore the business model, does not.

Set before any results arrived, in line with the course rule that the decision rule comes before the test.

## v0.2 (7 October 2026): one metric

**This is the current experiment card. Everything above it is the audit trail, not what we now run.**

### Why revised

The graded feedback: "You have designed a runnable test, but you have not run it. Make the metric measure either trust or intended use, not both." One half is closed and one is not, and saying otherwise would repeat the mistake the feedback caught. The metric is now one number measuring one thing. The test is still **not** runnable in practice: the artefact it needs, a set of hand made cards carrying the five openings verified in [test run 01](test-runs/run-01-shortlist-feasibility.md), has not been made. What has changed is that the openings on those cards will be real and checkable instead of invented.

### Riskiest assumption

> Students will judge an AI-built shortlist as accurate, meaning they recognise the openings we show them as genuinely fitting their profile.

Trust. Not intended use. The reasoning for choosing trust is in [assumptions.md](assumptions.md), v0.3.

### Hypothesis

If we show a student six openings chosen for the profile they gave us, each one verified as real and each carrying one line on why it is there, then the student will mark at least seven in ten of them as fitting.

### The experiment

Five real, verified Summer 2027 openings, found and checked by hand in [test run 01](test-runs/run-01-shortlist-feasibility.md), written by the team onto one card each. **The cards have not been made yet.** The student answers four questions out loud, is handed the five cards, and marks each "fits me" or "does not fit me", giving one line of reasoning for every rejection. Fifteen minutes. Seven students. Protocol in [test run 03](test-runs/run-03-student-trust-test.md).

### The metric

> **Fit rate: the share of the openings shown to a student that the student marks "fits me".**

One number per student. The result is the **median fit rate across students**. Nothing else counts toward pass or fail.

### Threshold, pre-committed 7 October 2026 before any student was shown a shortlist

| | |
|---|---|
| **Pass** | Median fit rate of at least 70%, across at least 5 students |
| **Fail** | Median fit rate below 70% |

### Decision rule, one metric, three branches

| Median fit rate | Decision |
|---|---|
| 70% or above | Accuracy holds at the manual stage. Continue to Step 2 of the roadmap |
| 50% to 69% | The concept survives, the matching rule does not. Rewrite the matching criteria from the rejection reasons and re-run this same test before building anything |
| Below 50% | Stop and rethink the venture. If a human hand picking from verified openings cannot reach half, an automated version will not, and the verified shortlist promise fails at its foundation |

### What is deliberately not measured

"Would you use this as a first filter?" and "What would stop you using it?" are asked at the end of every session and written into [user-feedback.md](user-feedback.md). **Neither enters the pass or fail.**

This is the single most important change in v0.2. The previous card had two success signals, 70% saying they would use it and most matches marked as fitting, and a decision rule that branched on both at once. A test with two metrics cannot be failed cleanly, because any result can be read as a partial pass on one of them. Now it can.

### What we expect, written down before the test

We expect a median fit rate between 50 and 69%, and we expect the Capital One Analyst Early Internship card to be the most rejected, because its sophomore only requirement is a hard eligibility gate our matching never looked at. If that card drives the rejections, the lesson is about eligibility fields. If rejections spread evenly across all six, the lesson is that the whole matching approach is too coarse. Writing this down first is what makes the result falsifiable instead of reinterpretable afterwards.

### Status

| | |
|---|---|
| Designed | Yes |
| Runnable | **Not yet.** The metric, threshold and protocol are in the repository and the openings are verified. The cards have not been made, so this test is fully specified rather than runnable today |
| **Run** | **Not yet. 0 of 7 students.** Owner Linda, target 15 October 2026 |

Two other tests on this venture have now been run and are written up with their results, including the results that went against us: [test run 01](test-runs/run-01-shortlist-feasibility.md) and [test run 02](test-runs/run-02-does-this-already-exist.md).
