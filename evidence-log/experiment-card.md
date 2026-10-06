# Experiment Card

## Riskiest assumption
Users will trust and use AI-generated opportunity recommendations as a first step in their decision process.

## Hypothesis
If we show students a simple prototype that asks for their preferences and returns a shortlist with clear explanations, then most of them will say they would use it to narrow down options.

## Smallest falsifiable experiment
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
