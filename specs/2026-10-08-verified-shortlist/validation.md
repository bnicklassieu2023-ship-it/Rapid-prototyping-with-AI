# Validation: the verified shortlist

What counts as this feature working, fixed in advance. Written 8 October 2026.

## The one metric

**Fit rate.** The share of the five openings shown to a student that the student marks "fits me". One number per student. Nothing else counts toward pass or fail.

**Pass:** median fit rate of at least 70% across at least five students.

Set on 7 October 2026, before any student had been shown a shortlist. Full card in [experiment-card.md](../../evidence-log/experiment-card.md) v0.2.

### Why one metric and not two

The graded feedback said: make the metric measure one thing. The previous card had two success signals, 70% saying they would use it and most matches marked as fitting, with a decision rule that branched on both. That is two tests wearing one card, and it meant no result could cleanly fail, because any outcome could be read as a partial pass on one of them. "Would you use this as a first filter?" is still asked at the end of every session and still written down. It is context for reading the number. It is not part of it.

## Decision rule, pre-committed

| Median fit rate | Decision |
|---|---|
| 70% or above | Phase B of [plan.md](plan.md) starts. Accuracy holds when a human does the matching, so a system can be built to do it |
| 50% to 69% | The concept survives, the matching rule does not. Rewrite the matching criteria from the rejection reasons and re-run the same paper test before anything is built |
| Below 50% | Stop and rethink the venture. Do not build. If a human hand-picking from verified openings cannot reach half, an automated version will not |

## Stop conditions

| Condition | What we do, not what we hope |
|---|---|
| Fewer than 5 students by 15 October 2026 | Report the individual fit rates as cases. Do not take a median of three people and call it a result |
| Fewer than 20 survey responses across both forms by 13 October 2026 | Report it as a weak sample. **This has already fired for round 1, n=4**, and every figure in [survey.md](../../evidence-log/survey.md) is written as a count out of 4 rather than a percentage because of it |
| Zero careers offices willing to talk | Funnel B is unvalidated, and the free-to-student channel in the press release is a claim rather than a plan |

## What we expect, written down before the test

So that we cannot claim afterwards that we knew.

- We expect a fit rate between 50 and 70%, that is, a near miss rather than a clean pass, because the matching is being done by hand against four answers.
- We expect the rejection reasons to be more useful than the number.
- We expect at least one student to reject an opening for a reason none of our four questions could have caught, and that reason to become a fifth question.

## What is already validated, and by what

| Claim | Status | Evidence |
|---|---|---|
| A verified shortlist of five can be assembled by hand | **OBSERVED.** 12 candidates checked, 5 passed all four criteria | [run 01](../../evidence-log/test-runs/run-01-shortlist-feasibility.md) |
| Model judgement of "still open" is unreliable | **OBSERVED.** Wrong on 2 of the 3 postings it read | run 01 |
| Live postings include dead links | **OBSERVED.** 2 of 12, HTTP 410 and HTTP 404 | run 01 |
| Accuracy is the first trust condition students name | **REPORTED, n=4.** The only option all four chose | [survey.md](../../evidence-log/survey.md) round 1 |
| Students would use this free through their university | **REPORTED, n=4.** 4 of 4 | survey.md round 1 |
| The university price is about 18,000 dollars a year | **CONTRADICTED.** Handshake charges about 8,000 | [run 02](../../evidence-log/test-runs/run-02-does-this-already-exist.md) |
| Employers cannot buy placement is a real differentiator | **SUPPORTED from outside.** Handshake is rolling out paid employer promotion in student feeds, beta, about 30 employers | run 02 |
| Students apply at high volume and are not hired | **CHALLENGED.** 2 of 4 sent five or fewer; 2 of 4 already hired through a platform | survey.md round 1 |
| Students will judge our shortlist as accurate | **UNTESTED.** 0 of 7 | run 03 |

## What would make this feature not worth building

Stated now, while it costs nothing to admit.

If the interviews show that students neither apply at high volume nor struggle to tell which openings are real, then the problem we are solving is not a problem they have, and the correct outcome is a different venture rather than a better shortlist. The push force is the weakest link in the chain, not the matching.
