# Test run 01: can we build a verified shortlist by hand at all?

**Status: RUN AND COMPLETE. Result recorded below, including the parts that go against us.**

| Field | Detail |
|---|---|
| Run on | 7 October 2026 |
| Run by | Claude (Cowork, claude-opus-5) as a desk run, instructed and reviewed by Linda |
| Type | Desk feasibility run. **Not** a user test. No student took part and none of this is user evidence |
| Question | Before we promise students a verified shortlist, can a human produce one at all, by hand, with no build? |
| Why it was run first | The graded feedback said we had designed a runnable test and never run one. This is the cheapest test in the project: no participants, no build, no scheduling. There was no good reason not to have run it already |
| Method | Search public sources for Summer 2027 openings matching one test profile, open every candidate, and check each against the four verification criteria our ERRC Raise row promises |
| Raw data | [raw/run-01-candidates.csv](raw/run-01-candidates.csv), 12 rows, every URL checkable |

## The test profile

Invented for the run, built from the Mass Applier persona. It is a profile, not a person, and is labelled as such.

> US undergraduate, junior year, business major, looking for a Summer 2027 internship in marketing or analytics, open to New York, Chicago or remote, authorised to work in the US without sponsorship.

## The four verification criteria

These are what our Raise row commits to. A candidate passes only if all four hold.

1. It is a real individual posting a student can apply to, not a landing page or a round-up article.
2. It is still open on the day of the check.
3. The student in the profile is eligible, by year of study and degree.
4. The posting states something about work authorisation or sponsorship.

## Result

**5 of 12 candidates passed all four criteria. Pass rate 42%.**

| # | Candidate | 1 Real posting | 2 Still open | 3 Eligible | 4 Work auth stated | Verdict |
|---|---|---|---|---|---|---|
| 1 | Endeavor, Digital Marketing Internship, Undergraduate, Summer 2027, New York | Yes | Yes, deadline 7 Oct 2026 23:59, closes today | Yes, any undergraduate year | Yes, explicit | **PASS** |
| 2 | Boeing, Summer 2027 Internship Program, Sales and Marketing | Yes | Yes, deadline 23 Oct 2026 | Yes, graduation Aug 2027 or later | Yes, explicit | **PASS** |
| 3 | Capital One, Analyst Early Internship Program, Summer 2027 | Yes | Yes, accepting | Yes, but sophomore standing only | Yes, explicit | **PASS** |
| 4 | Capital One, Business Analyst Intern, Summer 2027 | Yes | Yes, accepting | Yes, graduation by Aug 2028 | Yes, explicit | **PASS** |
| 5 | Allegion, Digital Marketing Intern, Summer 2027, Carmel IN | Yes | Yes, no deadline stated | Yes, bachelor's in progress | Yes, explicit | **PASS** |
| 6 | Constellation Brands, Undergraduate Marketing Intern, Summer 2027, Chicago | Yes | Yes, no deadline stated | Rising senior only | **No.** Mentions E-Verify, which is not a sponsorship statement | FAIL |
| 7 | Schwan's, Marketing Internship, via the Babson careers portal | Yes | Yes, expires 21 Oct 2026 | Yes | **No** | FAIL |
| 8 | Estee Lauder Companies, student internships page | **No**, landing page | Window "September to October 2026", no date | Not stated per role | **No** | FAIL |
| 9 | FedEx, marketing internships page | **No**, programme page | "Applications now open", no deadline | Not stated per role | **No** | FAIL |
| 10 | Interndock, "531+ live roles" Summer 2027 tracker | **No**, aggregator | Claims hourly updates, page dated 23 July 2026 | Not stated per role | **No** | FAIL |
| 11 | Morgan Stanley, 2027 Marketing Summer Analyst, via the IU Kelley portal | Surfaced by search as live | **No**, HTTP 410 Gone | Unknown | Unknown | FAIL |
| 12 | PepsiCo, 2027 Summer Intern, Marketing, Undergrad | Surfaced by search as live | **No**, HTTP 404 | Unknown | Unknown | FAIL |

## What this supports

- **The Raise row survives its first contact with reality.** Seven of twelve candidates that an ordinary student search surfaces are not things a student can act on: three are landing or aggregator pages rather than postings, two are dead, and two state nothing about work authorisation. The gap our Raise row claims to close is real and measurable, not a story we told ourselves.
- **Two of twelve search results were already dead.** Morgan Stanley returned HTTP 410 Gone and PepsiCo returned HTTP 404, both while still appearing in current search results. That is 17% of candidates where the student's click is wasted before they read a word. This is the cheapest part of our promise to keep and the one with the most visible payoff.
- **Work authorisation is the scarcest of the four.** Only the five large employers stated it. For an international student at a US university, that single field decides whether an application is worth sending at all, and it was missing or ambiguous more than half the time. Constellation Brands is the instructive case: it mentions E-Verify, which sounds like an authorisation statement and is not one. It tells a student nothing about whether sponsorship is available.
- **University careers portals are a closed door, twice.** Candidates 7 and 11 both sat behind a single university's portal, unreachable by a student anywhere else. That is an argument for the Funnel B partnership route and an argument against assuming we could simply index that content.

## What this works against us

- **Verification is expensive, and nothing in our plan has priced it.** Six searches and twelve page checks produced five usable openings. At that ratio a shortlist of five verified openings costs roughly twelve page checks. We have been writing about verification depth as a feature. It is a cost.
- **Most postings do not state a deadline at all.** Four of the five that passed gave no closing date. Our Raise row promises "still open", and the single most common honest answer is "no deadline stated". We cannot promise a student something the source does not contain.
- **The AI layer failed the staleness check.** When the model was asked to read each posting's status, it got two of the first three wrong. It called the Boeing posting closed when its deadline is 23 October, over two weeks away, and it called the Endeavor posting expired on a day it is still open. Both errors were caught only because a human compared the stated deadline against today's date.

  This is the most useful thing the run produced and it is uncomfortable: the single criterion our product exists to guarantee is the one the AI was worst at. The implication for the build is concrete. "Still open" must never be a model judgement. It must be the posting's own stated deadline, parsed as a date, compared against today, and shown to the student so they can check it themselves. Where no deadline exists, the card says "deadline not stated", never "open".

## What this does not show

- Nothing about whether students want this, trust it or would use it. No student was involved.
- Twelve candidates, one profile, one day. It shows the gap exists. It does not size it.
- Every one of the five that passed is a large employer with a professional recruiting function. We did not test small employers, which is where the less contested openings usually are, and the pass rate there is probably worse.

## Decisions taken from this run

| Decision | Reason |
|---|---|
| Keep verification depth as the ERRC Raise row | 7 of 12 failed it. The gap is real and measurable |
| Change the "still open" promise to "deadline shown, never inferred", and show "deadline not stated" where there is none | The AI misread status on 2 of 3 postings, and 4 of 5 passing postings stated no deadline at all |
| Add a dead-link check as the first and cheapest verification step | 2 of 12 were already dead. It costs one HTTP request |
| Price verification into the plan before the next revision of either funnel | 12 checks for 5 openings is a cost that appears nowhere in market-research.md |
| Treat an E-Verify mention as "not stated" for work authorisation | It reads like an answer and is not one |
| Use the five verified openings as the real cards in the rough prototype | The student trust test needs real openings, not invented ones |

## Next

Test run 03, the student trust test, uses the openings found here. Protocol in [run-03-student-trust-test.md](run-03-student-trust-test.md).
