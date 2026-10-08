# Test run 03: the student trust test

**Status: NOT RUN. 0 of 7 students completed.**

This is the test the graded feedback said we had designed and never run, and it is still not run. What exists: the openings it uses are real and verified from [run 01](run-01-shortlist-feasibility.md), the metric is one number, the protocol below is written, and the threshold was fixed before anyone was shown anything. What is missing is two things only the team can make: the five cards, and the students.

| Field | Detail |
|---|---|
| Assumption under test | Students will judge an AI-built shortlist as accurate, meaning they recognise the openings we show them as genuinely fitting their profile |
| Why this assumption and not intended use | See [../assumptions.md](../assumptions.md), v0.3 |
| Metric | **Fit rate.** The share of openings shown to a student that the student marks "fits me". One number per student. Nothing else counts |
| Threshold, set 7 October 2026 before any student was shown a shortlist | **Pass: median fit rate of at least 70% across at least 5 students** |
| Material needed | **Five cards, one per verified opening from [run 01](run-01-shortlist-feasibility.md), handwritten or printed by the team. NOT YET MADE** |
| Scoring | One tally sheet per student, made at the same time as the cards. NOT YET MADE |
| Why cards and not software | The course is explicit that no build is needed to start testing, and `prototype/` stays empty until Session 16. A card carries the same claim as a screen and costs nothing to change between students |
| Owner | Linda |
| Target date | 15 October 2026 |
| Stop condition | Fewer than 5 students by 15 October: report the fit rates we have as individual cases, do not take a median of three people and call it a result |

## The one thing that is deliberately not measured

"Would you use this as a first filter?" is asked at the end of every session and written into user-feedback.md. **It does not count toward pass or fail.**

This is a change made because of the graded feedback. The previous experiment card had two success signals, 70% saying they would use it and most matches marked as fitting, and a decision rule that branched on both. That is two tests wearing one card, and it meant no result could cleanly pass or fail. The metric is now one number measuring one thing: accuracy, which is our trust assumption. What students say about using it is context for interpreting the number, not part of it.

## Protocol

Fifteen minutes per student. No screen sharing, no explaining, no selling.

1. **Before the cards.** Ask the four profile questions out loud and write the answers down: field, location preference, year of study, whether they need visa sponsorship. Do not describe the product yet.
2. **Hand over.** Lay the five cards face up in front of them, in the order the four answers produced. Say only: "These came up for you. For each one, tell me whether it fits you or not."
3. **Silence.** Do not justify a card. If they ask whether a card is a good match, say "what do you think?" and wait. The moment the operator defends a card, the result is worthless.
4. **Per card.** They mark each card "fits me" or "does not fit me". On a "does not fit me", ask for one line on why and write it on the card. Those lines are the most useful output of the whole test.
5. **After the cards.** Count the "fits me" marks and divide by five. Write that fit rate and every rejection reason onto the tally sheet.
6. **Two closing questions, recorded but not scored.** "Would you use this as a first filter?" and "What would stop you using it?"
7. **Consent.** Confirm the recording consent in [../recruitment.md](../recruitment.md) before filming.

## Decision rule, pre-committed

Set on 7 October 2026, before any student had been shown a shortlist. One metric, three branches.

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
