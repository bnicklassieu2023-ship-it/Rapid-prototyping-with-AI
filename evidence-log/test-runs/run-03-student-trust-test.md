# Test run 03: the student trust test

**Status: NOT RUN. Everything needed to run it exists. 0 of 7 students completed.**

This is the test the graded feedback said we had designed and never run. The prototype now exists, the openings in it are real and verified, the scoring sheet is in the repository and the threshold was set before any student saw it. What is missing is students, and only the team can supply those.

| Field | Detail |
|---|---|
| Assumption under test | Students will judge an AI-built shortlist as accurate, meaning they recognise the openings we show them as genuinely fitting their profile |
| Why this assumption and not intended use | See [../assumptions.md](../assumptions.md), v0.3 |
| Metric | **Fit rate.** The share of openings shown to a student that the student marks "fits me". One number per student. Nothing else counts |
| Threshold, set 7 October 2026 before any student saw the prototype | **Pass: median fit rate of at least 70% across at least 5 students** |
| Prototype | [../../prototype/index.html](../../prototype/index.html), v0.2 |
| Scoring sheet | [../../prototype/scoring-sheet.csv](../../prototype/scoring-sheet.csv) |
| Owner | Linda |
| Target date | 15 October 2026 |
| Stop condition | Fewer than 5 students by 15 October: report the fit rates we have as individual cases, do not take a median of three people and call it a result |

## The one thing that is deliberately not measured

"Would you use this as a first filter?" is asked at the end of every session and written into user-feedback.md. **It does not count toward pass or fail.**

This is a change made because of the graded feedback. The previous experiment card had two success signals, 70% saying they would use it and most matches marked as fitting, and a decision rule that branched on both. That is two tests wearing one card, and it meant no result could cleanly pass or fail. The metric is now one number measuring one thing: accuracy, which is our trust assumption. What students say about using it is context for interpreting the number, not part of it.

## Protocol

Fifteen minutes per student. No screen sharing, no explaining, no selling.

1. **Before the prototype.** Ask the four profile questions out loud and write the answers down: field, location preference, year of study, whether they need visa sponsorship. Do not describe the product yet.
2. **Hand over.** Open the prototype, enter their four answers, hand them the laptop. Say only: "These came up for you. For each one, tell me whether it fits you or not."
3. **Silence.** Do not justify a card. If they ask whether a card is a good match, say "what do you think?" and wait. The moment the operator defends a card, the result is worthless.
4. **Per card.** They press "fits me" or "does not fit me". If they press "does not fit me", ask for one line on why and type it in. Those lines are the most useful output of the whole test.
5. **After the cards.** The prototype shows the fit rate. Copy the result block into the scoring sheet.
6. **Two closing questions, recorded but not scored.** "Would you use this as a first filter?" and "What would stop you using it?"
7. **Consent.** Confirm the recording consent in [../recruitment.md](../recruitment.md) before filming.

## Decision rule, pre-committed

Set on 7 October 2026, before any student had seen the prototype. One metric, three branches.

| Median fit rate | Decision | Why |
|---|---|---|
| 70% or above | Continue to Step 2 of the roadmap | Accuracy holds at the manual stage. If a human can do it, a system can be built to do it |
| 50% to 69% | The concept survives, the matching rule does not. Rewrite the matching criteria from the rejection reasons and re-run this same test before anything is built | A near miss means we are matching on the wrong fields, not that students reject the idea |
| Below 50% | Stop and rethink the venture. Do not build | If a human hand-picking from verified openings cannot reach half, an automated version will not, and the verified shortlist promise fails at its foundation |

## What we expect, written down before the test

Writing the expectation down first makes the result falsifiable rather than reinterpretable afterwards.

We expect a median fit rate between 50 and 70%, and we expect the Capital One card to be the most rejected one, because its sophomore-only requirement is a hard eligibility gate that our matching never looked at. If that card is rejected most often, the lesson is about eligibility fields, not about trust. If instead the rejections spread evenly across cards, the lesson is that the whole matching approach is too coarse.

## Results

| Student | Date | Cards shown | Marked "fits me" | Fit rate | Most common rejection reason | Would use as first filter (not scored) |
|---|---|---|---|---|---|---|
| | | | | | | |

**Median fit rate: not yet calculated. n = 0.**

Nothing in this repository treats this assumption as tested until this table has at least five rows.
