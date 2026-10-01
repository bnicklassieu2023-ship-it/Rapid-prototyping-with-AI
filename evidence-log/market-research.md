# Market Research (United States)

**Scope decision:** the market is the United States. Spain was dropped on 1 October 2026 after the team chose the US as the target market. The earlier Spanish funnel is no longer part of our analysis and is kept only in the repository history.

**Method:** the five steps taught in Session 10. Scope, Map, Compare, Stress-test, Hypothesise. Market evidence and user evidence are kept separate throughout. Market research tells us what exists, never what our users do.

---

## 0. Why we moved from Europe to the United States

**Status of this decision:** a team decision, shaped by discussions in class. The reasoning below is our judgement plus supporting context, not validated market evidence.

| Reason | What we mean | Evidence status |
|---|---|---|
| Users are more open to new AI providers | US students appear readier to try an unfamiliar AI tool, so adoption should cost us less persuasion than in Europe | TEAM JUDGEMENT, with one supporting indicator: 33% of US graduating seniors used AI in their job search (NACE 2025), against about 18% of UK students and graduates using a chatbot for careers advice (Prospects 2026). The two surveys ask different questions of different populations, so this is directional only |
| Lighter regulatory load for a small team | In the EU, the AI Act brings conformity assessment, technical documentation, database registration, an authorised representative for non-EU providers and human-oversight duties. Most provisions apply from 2 August 2026, with high-risk deadlines proposed to move to December 2027 and sector obligations to August 2028, subject to Council agreement. The US has no single equivalent federal statute; rules are sector and state level | SUPPORTED for the EU timeline. The comparison with the US is our reading and should be checked before we claim it on stage |
| Bigger single market in one language | 19.4M US postsecondary students under one regulatory regime, versus 27 member states with different labour markets, languages and job boards | SUPPORTED by enrolment data; the implied cost saving is our inference |
| Clearer incumbent to position against | Handshake sits inside US careers offices and is funded by employers, which is exactly the convention our ERRC grid eliminates | SUPPORTED that the incumbent exists; our ability to displace it is untested |

**What we gave up by moving:** our only real-user evidence so far was gathered in Europe, and our survey respondents are mostly Spanish students. The team decided to treat them as a proxy for US behaviour. That is a declared assumption, recorded in assumptions.md, and the honest counter-argument is that regulation and openness to AI tools may change behaviour in exactly the ways we are claiming.

**What would make us reconsider:** if US respondents turn out to be no more willing to try a new tool than European ones, the main reason for the move disappears, and the EU's larger regulatory burden alone would not justify the harder channel fight against Handshake.

---

## 1. Fermi estimate before any research

How many US undergraduates are applying for an internship or a job this month?

| # | Step | Basis | Working | Result |
|---|---|---|---|---|
| 1 | US undergraduates | KNOWN, National Student Clearinghouse, fall 2025 | 16.2M | 16,200,000 |
| 2 | In a year where they look for a job or internship | ASSUME 30 to 50%, use 40% | 16.2M x 0.40 | 6,480,000 |
| 3 | Searching in any given month of the academic year | ASSUME 20 to 40%, use 25% | 6.48M x 0.25 | 1,620,000 |
| 4 | Applications sent per searching student per month | ASSUME 3 to 10, use 5 | 1.62M x 5 | 8,100,000 applications |
| 5 | DERIVED | Applications per month in the US | | about 8 million |

Sanity check: at roughly 30 applications per hire (NACE 2025) that implies about 270,000 hires a month across US early careers, which is the right order of magnitude for a market with 16 million undergraduates.

This is a back of the envelope figure. The funnels below replace the guesses with sourced anchors wherever we have them, and name what is still an assumption.

---

## 2. Market claims, with evidence strength

Claim, evidence, source, strength, contradiction or gap, implication.

| Claim | Evidence | Source | Strength | Contradiction or gap | Implication |
|---|---|---|---|---|---|
| The US has 16.2M undergraduates and 19.4M postsecondary students | Enrolment data, fall 2025 | National Student Clearinghouse, published January 2026 | Strong | Includes 2-year colleges whose career paths differ | Segment four-year institutions for the partnership funnel |
| One third of graduating seniors used AI in their job search | 33% used it, 67.1% did not | NACE 2025 Student Survey, 1,479 graduating seniors | Medium | Seniors only, and attitudes are moving fast | Treat 33% as the early-adopter ceiling, not a trend line |
| Students who avoid AI do so mainly on ethics and skill, not indifference | 28.9% ethics, 24.6% lack of expertise, 15.9% fear employers notice | NACE 2025 Student Survey | Medium | Those reasons concern AI writing for them, not AI filtering for them | Position as a filter that never writes on their behalf, and say so in the product copy |
| The early-career market is genuinely hard right now | 5.6% unemployment and 42% underemployment for recent graduates, Q2 2026 | Federal Reserve Bank of New York | Strong | Hardship does not prove demand for our tool | Use as urgency in the press release, never as evidence of demand |
| Handshake is the incumbent inside US careers offices | 18M students across 1,200 institutions | Company figures reported 2021, most recent published | Weak and dated | No public pricing, and the figure is five years old | Assume incumbency in the channel and test switching directly |
| Students send about 30 applications per role | Class of 2025 averages | NACE 2025 | Medium | An average hides heavy variance | Basis for the time-value calculation below |
| Trust starts with accuracy rather than explanation | One student: hundreds of applications, interviews, never hired through a platform; would trust a tool that shows no unsuitable jobs | Our interview 01, n=1 | Very weak | A single interview, and conducted in Europe | The live survey measures it; see survey.md |
| University careers offices will adopt a second tool alongside Handshake | None | No evidence | None | This is the assumption the partnership funnel rests on | Next test: two careers-office conversations |

---

## 3. Competitive alternatives, four categories (US)

| Alternative | Simple test | Target-user behaviour evidence | Compare on | Evidence so far and gaps | So what? Decision or action |
|---|---|---|---|---|---|
| Direct competitors: Handshake, LinkedIn, Indeed, Jobright.ai | Same user, essentially the same job? | HYPOTHESIS for our segment. Handshake is embedded in US careers offices, but we have not observed our own target users choosing it | Match accuracy, explanation, price, trust, switching cost | Handshake reaches students through institutions; Jobright gives a match score with an explanation and a free tier; LinkedIn sells fit assessment in its paid tier. GAP: no observed behaviour from US students in our segment | Explanation is table stakes. Compete on accuracy and on the entry-level shift view, and test switching away from Handshake first |
| Indirect substitutes: ChatGPT and other chatbots, auto-apply copilots, the campus careers office | Same progress, different route? | REPORTED. 33% of graduating seniors used AI in the job search (NACE 2025), mostly for cover letters, interview prep and resumes | Effort, repeatability, cost, habit | Chatbots are free and already in students' hands; careers offices are free and trusted but capacity-limited | Our survey asks what they used last time, which moves this from hypothesis to evidence |
| Manual workarounds: mass applying, spreadsheets, scrolling listings | Is the user still assembling it themselves? | REPORTED, n=1. Hundreds of applications, some interviews, never hired through a platform | Time, hit rate, error risk, control | About 30 applications per role (NACE 2025). GAP: one case is not a pattern | This is the real baseline. Quantify the friction, then remove it with the least change to habits |
| Doing nothing: keep applying the same way, or wait until senior year | Delay or accept the pain? | HYPOTHESIS. Our JTBD trigger is still an open gap | Urgency, pain cost, trigger | 42% underemployment among recent graduates makes waiting costly, but students may not feel that until late | Find the trigger. The interviews ask what made them start last time |

---

## 4. Testing the strategic bets

| Bet | Hypothesis | Method | Metric | Threshold | Decision rule |
|---|---|---|---|---|---|
| Direct competitors | Students will use an accurate shortlist instead of Handshake's feed as their first filter | Prototype test with 5 to 8 US-relevant students, each marking every recommendation as fits me or does not fit me | Share using it as a first filter; share of matches rejected | 70% first-filter use; most matches accepted | Met: keep the accuracy wedge. Missed: fix matching before building anything else |
| Indirect substitutes | A filtered shortlist beats asking a chatbot | Same student runs one search with ChatGPT and one with our shortlist | Usable roles found; time spent | Our shortlist produces more usable roles in less time for 4 of 7 | Met: position against chatbots on repeatability. Missed: our advantage is not the matching, rethink |
| Manual workaround | Students will trade volume for fit | Interview question on applications sent versus interviews obtained, plus survey Q4 and Q5 | Share reporting high volume and no hire | Half or more | Met: the push force generalises beyond interview 01. Missed: our problem statement is weaker than we thought |
| Doing nothing and the channel | A careers office will promote a second tool | Two interviews with US careers-office staff about how they adopted their last tool | Willingness to pilot; stated procurement path | At least one says yes to a pilot | Met: the partnership funnel stays. Missed: the partner route is blocked and the direct funnel is all we have |

---

## 5. Funnel A: United States without university partnerships

| Step | Who | Keeps | Running total | Label | Why we cut |
|---|---|---|---|---|---|
| Start | All US postsecondary students | | 19,400,000 | KNOWN, NSC fall 2025 | The first assumption: every student in America |
| 1 | Undergraduates only | 84% | 16,200,000 | KNOWN, NSC | Our Job is first jobs and internships, not experienced hires |
| 2 | Actively looking this year | 40% | 6,480,000 | ASSUME | Being enrolled is not a trigger; our JTBD trigger is still open |
| 3 | Open to using AI in the job search | 33% | 2,138,400 | SOURCE, NACE 2025 | Two thirds actively avoid AI, mostly on ethics |
| 4 | Would try a new platform instead of Handshake or LinkedIn | 40% | 855,360 | ASSUME | Handshake is built into US careers offices, so switching is hard |
| 5 | Accept our model: free, student login, share a profile | 60% | 513,216 | ASSUME | We removed employer-paid placement, so the student must accept our route |
| 6 | Fit one of our three personas | 70% | 359,251 | ASSUME | The Starter persona still has no real-user evidence |
| 7 | Reachable in year one with no partnerships | 0.5% | 1,796 | ASSUME | No contracts, no budget, 3,931 institutions to choose from |

**Addressable in year one: about 1,800 students, which is 0.009% of the starting market.**

**Value created:** about 30 applications per role at roughly 20 minutes each is about 10 hours per search. An accurate shortlist that halves it saves about 5 hours per student. At a student hourly value of 15 dollars that is 75 dollars per student per year, so about 135,000 dollars of time value across 1,800 students.

**Tightest filter:** step 7, reach, which keeps only 0.5%. The tightest demand filter is step 4, switching away from Handshake, which keeps 40%.

**Low, base, high**

| Scenario | Step 2 | Step 4 | Step 5 | Step 7 | Year-one students |
|---|---|---|---|---|---|
| Low | 30% | 25% | 50% | 0.25% | about 350 |
| Base | 40% | 40% | 60% | 0.5% | about 1,800 |
| High | 50% | 55% | 70% | 1% | about 7,200 |

---

## 6. Funnel B: United States with university partnerships

Scenario assumptions. None of the partnership numbers below is evidence. They are planning figures the team invented to see what the channel would be worth.

**Institutional starting point**

| Step | Who | Number | Label |
|---|---|---|---|
| Start | Title IV degree-granting institutions in the US | 3,931 | KNOWN, NCES 2020-21 |
| 1 | Four-year institutions | 2,637 | KNOWN, NCES |
| 2 | Large enough to run a careers platform and buy software | 1,582 | ASSUME 60% |

**What one partner campus is worth per year**

| Step | Logic | Keeps | Result | Label |
|---|---|---|---|---|
| Undergraduates at one partner campus | Mid-size public university | | 20,000 | ASSUME |
| Actively looking this year | Same as Funnel A | 40% | 8,000 | ASSUME |
| Hear about us because the careers office promotes it | Email, portal link, orientation | 60% | 4,800 | ASSUME |
| Create an account | Endorsement lifts sign-up above cold | 25% | 1,200 | ASSUME |
| Use it more than once | Activation | 60% | 720 | ASSUME |

**Scaling scenario**

| | Partner campuses | Students reached | Accounts | Active users | Share of US institutions | Time value created |
|---|---|---|---|---|---|---|
| Year 1 | 3 pilots | 60,000 | 3,600 | 2,160 | 0.08% | about 162,000 dollars |
| Year 2 | 15 | 300,000 | 18,000 | 10,800 | 0.4% | about 810,000 dollars |
| Year 3 | 50 | 1,000,000 | 60,000 | 36,000 | 1.3% | about 2.7M dollars |

**Revenue scenario, if universities pay:** at an assumed 18,000 dollars per campus per year, 54,000 dollars in year one, 270,000 in year two, 900,000 in year three. Handshake does not publish institutional pricing, so this number is the weakest figure on the page and we say so.

**Tightest filter:** whether the careers office actually promotes the tool. If promotion reaches 20% rather than 60%, year three active users fall from 36,000 to about 12,000.

**Low, base, high for year three**

| Scenario | Campuses | Hear about it | Sign up | Active | Active users |
|---|---|---|---|---|---|
| Low | 20 | 50% | 15% | 50% | about 6,000 |
| Base | 50 | 60% | 25% | 60% | about 36,000 |
| High | 80 | 70% | 35% | 70% | about 110,000 |

**What the comparison says:** partnerships are worth roughly the same as the direct route in year one and about twenty times more by year three, because each campus delivers 20,000 students at once. They are also slower and have the weakest evidence behind them, since US procurement runs six to twelve months, pilots are normally unpaid, and a student-data product must pass a FERPA and security review.

---

## 7. Opportunity stress test, all four lenses

| Lens | Question | Our answer |
|---|---|---|
| Entry | What would stop a credible new entrant? | Very little. Jobright shows that match scores with explanations are already buildable. Our defences are the segment, the channel and the shift monitor, not the matching itself |
| Substitution | What could users choose instead? | A free chatbot they already have. If students accept chatbot answers as good enough, our wedge narrows to verifiable accuracy |
| Dependencies | What external dependency could block us? | Access to job-posting data, and occupation data for the shift monitor. If posting access is restricted or priced, the offer changes shape |
| Major shifts | What could make this irrelevant? | If AI collapses entry-level hiring further, the job we serve changes from finding a fitting role to retraining into a different one |

**The three findings most likely to change our decision**

1. The channel we depend on is already owned by Handshake, so the partnership funnel is a competition, not an open door.
2. Our only real evidence of the trust condition is one interview. Everything in the ERRC grid rests on it until the survey lands.
3. Underemployment at 42% means the painful part may not be finding a role, but finding one worth taking. If the survey says that, our Job statement needs rewording.

---

## 8. Limitations we state in the presentation

- Four of the seven filters in Funnel A, and every number in Funnel B, are assumptions rather than sources.
- Our survey respondents are mostly students in Spain. The team decided to treat their behaviour as a proxy for US students. That is an explicit assumption, not a finding, and it is the first thing we would re-test with US respondents.
- Handshake's scale figure is from 2021 and its pricing is not public.
- Market research here establishes what exists in the market, not what our users do.

## Sources

- National Student Clearinghouse Research Center, Final Fall Enrolment Trends, fall 2025 data published January 2026: 19.4M postsecondary, 16.2M undergraduate, 3.2M graduate. Accessed 1 October 2026
- NACE 2025 Student Survey, 1,479 graduating seniors: 33% used AI in the job search; non-users cite ethics 28.9%, lack of expertise 24.6%, fear employers notice 15.9%; about 30 applications per role. Accessed 1 October 2026
- Federal Reserve Bank of New York, The Labor Market for Recent College Graduates, Q2 2026: 5.6% unemployment, 42% underemployment. Accessed 1 October 2026
- National Center for Education Statistics, Fast Facts, 2020-21: 3,931 Title IV degree-granting institutions, 2,637 four-year. Accessed 1 October 2026
- Handshake company figures as reported in 2021: 18M students, 1,200 institutions. Accessed 1 October 2026
- Jobright.ai and LinkedIn product pages for competitor features. Accessed October 2026
