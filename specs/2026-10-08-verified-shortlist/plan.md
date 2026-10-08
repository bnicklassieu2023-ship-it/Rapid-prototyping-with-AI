# Plan: the verified shortlist

How Step 1 gets tested and then built, in that order. Written 8 October 2026.

## The order is deliberate

The course is explicit that no build is needed to start testing, and the repository structure keeps `prototype/` empty until Session 16. So the plan runs the test on paper first and builds only what the paper test survives. The reason is not tidiness. It is that a built screen is expensive to change between students, and a card costs nothing, so the paper round is where we can afford to be wrong.

## Phase A: the paper round, now, before any code

| Step | What | Owner | Status |
|---|---|---|---|
| A1 | Write the five verified openings from [run 01](../../evidence-log/test-runs/run-01-shortlist-feasibility.md) onto five cards, one per card, each carrying the posting source, the stated deadline or "deadline not stated", the quoted work authorisation line, and one line on why it is here | Team | **NOT DONE. This is the single blocking item** |
| A2 | Make one tally sheet per student: five rows, a fits/does not fit mark, a reason column, and a fit rate at the bottom | Team | NOT DONE |
| A3 | Run [test run 03](../../evidence-log/test-runs/run-03-student-trust-test.md) with 7 students, 15 minutes each, following the protocol exactly | Linda | 0 of 7 |
| A4 | Hold the 2 careers office conversations in [careers-office-outreach.md](../../evidence-log/careers-office-outreach.md) | Team | 0 of 2 |
| A5 | Merge survey round 2 from the parallel form, restate n, re-read every decision rule against the combined sample | Team | Waiting on the responses |

Phase A produces a number: the median fit rate across at least five students. The decision rule for that number was fixed on 7 October 2026 and is in [experiment-card.md](../../evidence-log/experiment-card.md) v0.2. Nothing in Phase B starts until that number exists.

## Phase B: the build, Session 16 at the earliest

Entered only on a median fit rate of 70% or above. On 50 to 69% the matching criteria are rewritten from the rejection reasons and Phase A is re-run. Below 50% the venture is rethought, not rebuilt.

| Step | What | Depends on |
|---|---|---|
| B1 | Four-question intake, one screen, no account | R1, R2, R3 |
| B2 | Dead-link check as the first operation on every candidate, before anything else touches it | R4. It is one HTTP request and it caught 2 of 12 |
| B3 | Deadline parsed from the posting text, never inferred, with "deadline not stated" as a first-class result | R5, R6 |
| B4 | Work authorisation line quoted verbatim, with E-Verify mapped to "not stated" | R7 |
| B5 | Five cards with the why line and the uncertainty line | R8, R10 |
| B6 | Hard constraint in the code path: no field, flag or parameter anywhere that an employer could pay to change | R9 |

## What the AI is allowed to do, and what it is not

This is the build rule the project runs on, and it came out of our own test, not out of principle.

**The AI may:** draft text, search for candidate postings, extract fields from a posting it has fetched, write the code, and write the explanation lines.

**The AI may not:** decide whether a posting is still open. In run 01 the model misread posting status on 2 of the 3 postings it was asked to read, including declaring a page live that returned HTTP 410. That judgement is taken away from the model entirely and replaced with a fetched status code and a parsed date. Any future build that gives it back has to argue against this paragraph.

**The AI may never:** stand in for a student. The three personas in [personas/](../../evidence-log/personas/) are a rehearsal device and are labelled as counting for nothing. No persona output appears in any result table in this repository.

## Risks that could stop this

| Risk | Current state | What we would do |
|---|---|---|
| Verification cost makes the unit economics impossible | 12 checks produced 5 openings, and this cost appears in neither funnel | Price it before the next funnel revision. If it does not close, the free-to-student model is the thing that breaks, not the product |
| The university price is wrong | Run 02 found Handshake charges universities about 8,000 dollars a year against the 18,000 we assumed | Funnel B gets rebuilt or defended. It cannot stay as written |
| Employers refuse AI-assisted applications | Raised unprompted by one survey respondent, n=1 | Cheap to check against real job descriptions. Not yet done |
| We are testing the wrong segment | Round 1: 2 of 4 sent five applications or fewer, 2 of 4 already hired through a platform. Only one of four resembles the student in interview 01 | The interviews ask where each student is in their search before anything else |
