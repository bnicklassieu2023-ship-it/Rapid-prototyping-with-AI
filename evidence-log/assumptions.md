# Assumptions

## MECE area 1: User problem
- Students feel overloaded by too many opportunity sources.
- Students want help narrowing options down.
- Students currently spend significant time comparing opportunities manually.

## MECE area 2: Product value
- Users will value personalized recommendations more than generic search results.
- Users will trust recommendations more if the AI explains the reason behind each match.
- Users will prefer a shortlist over a long list.

## MECE area 3: Adoption and behavior
- Users are willing to input their preferences and expectations.
- Users are willing to upload CV/profile information.
- Users would use an AI assistant before applying.

## Must-be-true assumptions
- Users have a real problem worth solving.
- Personalized matching is better than manual browsing.
- Users trust the recommendations enough to act on them.

## Evidence needed
- Interviews or usability feedback showing students care about the problem.
- Reactions to a rough prototype that generates recommendations.
- Evidence that explanation/transparency increases trust.

## Riskiest assumption
Users will trust and use AI-generated opportunity recommendations as a first step in their decision process.

## Why this is the riskiest
If users do not trust the recommendations, the whole product loses value before we even reach the application step.

## v0.1 (Session 8): reprioritisation

Evidence: user-feedback.md (1 real student), jtbd.md, personas/.

| Assumption | v0 | v0.1 status |
|---|---|---|
| Users will trust and use AI-generated opportunity recommendations as a first step in their decision process | Riskiest | Still the riskiest. Unchanged. Not yet tested with the prototype |
| Users will trust recommendations more if the AI explains the reason behind each match | Product value | CHALLENGED by interview 01: trust was linked to accuracy (no unsuitable jobs), not explanations |
| New: trust depends on showing no job that does not fit the student's profile or interests | Not listed | NEW, from interview 01 (n=1). Must be tested |
| Students currently spend significant time comparing opportunities manually | User problem | PARTLY SUPPORTED: hundreds of applications (interview 01) |
| Users are willing to upload CV/profile information | Adoption | Still UNKNOWN, not asked |

The riskiest assumption stays exactly as written. What changed is what we believe makes students trust the recommendations.

## v0.2 (Group Project I): market assumptions

Added 1 October 2026 with the move to the United States. These are assumptions, not findings.

| Assumption | Status | How we would test it |
|---|---|---|
| The United States is the right first market for us | Team decision, untested | Compare switching and channel evidence between US and European respondents |
| Spanish survey respondents behave closely enough to US students to inform US decisions | Team decision, explicitly declared as a proxy | Send the survey to US students and compare the two groups |
| 40% of US undergraduates look for a job or internship in a given year | ASSUME, used in both funnels | Survey Q3 and Q4 |
| 40% would try a new platform rather than stay with Handshake or LinkedIn | ASSUME, the tightest demand filter | Survey Q6, plus the prototype test |
| A US careers office will adopt a second tool alongside Handshake | No evidence at all. The whole partnership funnel rests on it | Two careers-office interviews |
| A university would pay about 18,000 dollars a year for a licence | ASSUME, no public pricing exists for the incumbent | Ask in the careers-office interviews |
| Students want to be told which entry-level roles are shrinking | ASSUME, our Create row | Survey Q10 |

## v0.3 (7 October 2026): one assumption, chosen

**This is the current position. Everything above it is the audit trail, not what we now hold.**

### Why this version exists

The graded feedback on the previous submission said the same thing three times in three different criteria:

> Venture chain: "The chain is mostly coherent, but trust and intended use are mixed together. Choose one and carry it consistently through the test and decision rule."
> Riskiest Assumption: "Choose either trust or intended use as the main assumption, then explain why that one matters most."
> Experiment fit: "Make the metric measure either trust or intended use, not both."

It was right. Our riskiest assumption was literally "users will **trust and use** AI-generated opportunity recommendations". That is two assumptions joined by an "and", and because it was two, the test had two success signals and the decision rule branched on both, which meant no result could cleanly pass or fail it.

### The riskiest assumption, v0.3

> **Students will judge an AI-built shortlist as accurate, meaning they recognise the openings we show them as genuinely fitting their profile.**

One claim. It is about **trust**, not about intended use.

### Why trust and not intended use

1. **It is upstream.** A student cannot use a list they do not believe. Intended use is downstream of accuracy, so testing use first measures the far end of a chain whose near end is untested. If trust fails, use cannot follow. If trust holds and use does not, we have a different and much smaller problem, about packaging and distribution.
2. **It is the only one of the two our strategy rests on.** Our ERRC grid eliminates employer influence and raises verification depth. Both are trust moves. If accuracy turns out not to matter to students, the entire grid is answering a question nobody asked, and the venture has no reason to exist. Intended use, by contrast, can be bought with marketing by anyone, which is why it does not differentiate us.
3. **It is observable rather than claimed.** "Would you use this?" costs a student nothing to say yes to, and students say yes to be kind. "Does this specific opening fit you?" is a judgement about a real thing in front of them, made six times, that produces a number we did not choose.
4. **The one real student we have named it first, unprompted.** Asked when he would start trusting a new site, he said: if, when he gives it the relevant information, it does not show him jobs that do not suit his profile or interests. He did not say "if it explains itself" and he did not say "if it is easy to use". See [user-feedback.md](user-feedback.md).

### What happens to intended use

It stays on this list as an assumption. It is **not** being tested now, and nothing in the test may score it. The two closing questions in the trust test, whether they would use it as a first filter and what would stop them, are recorded in user-feedback.md as context for reading the number. They are not part of the number.

### The assumption map, re-sorted

| # | Assumption | Status after v0.3 |
|---|---|---|
| 1 | Students will judge an AI-built shortlist as accurate | **THE RISKIEST. Under test now**, test run 03 |
| 2 | Students would use an accurate shortlist as a first filter | Demoted. Next in line, not tested now |
| 3 | Trust depends on showing no opening that does not fit | Folded into 1. This is what accuracy means for us |
| 4 | Explanations build trust | CHALLENGED by interview 01 and now deliberately not load bearing. Each card carries one line of reasoning, but the metric does not score it |
| 5 | Students are willing to upload CV and profile data | **Actively avoided**, not assumed. The prototype asks four questions and no CV. See [privacy.md](privacy.md) |
| 6 | Verified openings are scarce enough to be worth paying for | **SUPPORTED by a run of our own**: 7 of 12 candidates failed verification, test run 01 |
| 7 | A university would pay about 18,000 dollars a year | **CONTRADICTED**, see below |
| 8 | A US careers office will adopt a second tool alongside Handshake | No evidence at all. Funnel B rests on it entirely |
| 9 | Students want to be told which entry level roles are shrinking | ASSUME, our Create row. Survey question 10 |

### New assumptions produced by our own test runs

These did not come from a workshop. They came from running something and being surprised.

| Assumption | Where it came from | Status |
|---|---|---|
| "Still open" can be determined reliably by an AI reading a posting | Test run 01 | **FALSIFIED.** The model misread status on 2 of the 3 postings it read. The check was taken away from the model and is now a stated deadline compared against today's date |
| Postings state a closing date | Test run 01 | **FALSIFIED.** 4 of the 5 verified openings stated no deadline at all. Our card now says "deadline not stated" rather than claiming the role is open |
| Verification is cheap enough to ignore in the plan | Test run 01 | **FALSIFIED.** 12 page checks produced 5 usable openings. The cost appears nowhere in either funnel |
| A university would pay about 18,000 dollars a year for our licence | Test run 02 | **CONTRADICTED.** Handshake charges universities about 8,000 dollars a year for the system that replaces their whole legacy careers stack. We were proposing more than twice that for a second tool that does less. Funnel B's revenue line has to be rebuilt or defended |
| Removing employer influence is a meaningful differentiator | Test run 02 | **STRENGTHENED, with a date.** Handshake is rolling out paid employer promotion inside student feeds, in beta with about 30 employers and a broader rollout planned for early 2026 |

## v0.4 (7 October 2026): what survey round 1 did to this list

Round 1, n=4. See [survey.md](survey.md) for the counts and [user-feedback.md](user-feedback.md) for the evidence read. Nothing here is validated by four people; this records direction and, more importantly, damage.

| # | Assumption | Change after round 1 |
|---|---|---|
| 1 | Students will judge an AI-built shortlist as accurate | **Still the riskiest, unchanged.** All 4 named accuracy as their first trust condition, which is consistent with our v0.3 choice. Still untested with a real shortlist |
| 3 | Trust depends on showing no opening that does not fit | **WEAKENED.** 0 of 4 said one or two bad matches would break their trust; all 4 chose 3 to 5 or more. Accuracy ranks first, but the absolute version of this assumption, which came from interview 01, is not supported |
| 5 | Students are willing to upload CV and profile data, which we avoid | **Reframed.** Only 1 of 4 picked privacy as a trust factor. Our data position is a principle we chose, not a demand students expressed, and it is presented that way |
| 9 | Students want to be told which entry-level roles are shrinking | Consistent: 4 of 4 said it would change what they apply for. Still bounded by what spike-shift-monitor.md says is buildable |
| 8 | A US careers office will adopt a second tool alongside Handshake | Unchanged. 4 of 4 students would use it through their university, which says nothing about whether a careers office would buy it. Still no evidence at all on the office side |

### The assumption round 1 damaged most

> **Students apply at high volume and still do not get hired.**

This sits underneath our opportunity statement, our press release and the Mass Applier persona. Round 1: 2 of 4 sent five applications or fewer, and 2 of 4 have been hired through a platform.

**Status: CHALLENGED.** Not falsified, because all four are bachelor students and three are 21 or under, so they are earlier in the search than interview 01. But it can no longer be stated as a general fact about students. It is a claim about a segment we have not yet defined, and defining that segment is now a job for the interviews.

### New risks, from the written objections

| Risk | Where it came from | Status | How we would test it cheaply |
|---|---|---|---|
| Employers are starting to state that they do not accept applications made through agencies or AI tools, which could make our shortlist unusable at the point of applying | Survey Q8, one respondent, raised against our own idea unprompted | **NEW, n=1, and the sharpest objection we have received** | Read 20 real entry-level US postings and count how many carry such a clause. One desk run, no participants needed |
| A verified, narrow list may simply not cover the industry a student wants | Survey Q8, one respondent | NEW, n=1 | Ask in the interviews which industry, then check whether our verification method can reach it |
| Cost is an objection before any price exists | Survey Q8, one respondent answering only "money" | NEW, n=1 | The payment questions were cut from the short survey. They go to the interviews |
| Students want everything in one place, which is the opposite of our Reduce row | Survey Q8, one respondent | NEW, n=1, and strategically awkward. See ERRC.md | Ask directly in the interviews whether fewer, checked results beat more, unchecked ones |
