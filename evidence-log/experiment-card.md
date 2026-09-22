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

**Why revised:** interview 01 (interview-evidence.md) linked trust to never seeing an unsuitable job, so the test now also measures match accuracy.

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
