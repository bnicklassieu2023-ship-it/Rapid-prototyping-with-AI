# Decision log

**What this file is for.** Every step in this project is recorded here with the same five questions answered: why we did it, what we wanted to validate, what the result was, whether the assumption turned out right or wrong, and what we cut or added because of it.

It exists because a venture log that only records what we built reads as a list of activity. This one is meant to show the reasoning, including the steps that produced an uncomfortable answer and the things we removed. Cutting something out is a result, not a failure, and it is logged here the same way as adding something.

**How to use it.** Add an entry for every step, including interviews, before moving on to the next one. If an entry cannot answer "what did we want to validate", the step was activity rather than a test, and that is worth noticing at the time.

---

## 1. Opportunity, goals, assumptions and first experiment card
**Sessions 3 to 5.** Tool: ChatGPT.

- **Why:** we needed a first statement of the problem and a riskiest assumption before anything could be tested.
- **What we wanted to validate:** nothing yet. This step produced the claims that everything later would test.
- **Result:** a working opportunity statement, an assumption map, and a riskiest assumption: "users will trust and use AI-generated opportunity recommendations as a first step."
- **Right or wrong:** the framing held, but the riskiest assumption was two assumptions joined by an "and". That flaw survived until 7 October and cost us marks. See entry 15.
- **Cut or added:** added the first evidence log. Nothing cut yet.

## 2. Job to Be Done
**Session 6, 21 September 2026.**

- **Why:** to express the problem as progress a student is trying to make, rather than as a feature list.
- **What we wanted to validate:** whether we could name the circumstance, trigger and forces without inventing them.
- **Result:** we could name most of it. The trigger, the moment that starts a search, could not be named from anything we had.
- **Right or wrong:** correct to leave it blank. The trigger is still an open gap today, which is honest rather than tidy.
- **Cut or added:** cut "job or further study" down to jobs and internships. Master's programmes parked, not rejected.

## 3. Personas
**Session 6, 21 September 2026.**

- **Why:** to decide who we were building for before testing anything.
- **What we wanted to validate:** whether our target split into distinguishable types.
- **Result:** six persona hypotheses drafted, three selected: the Mass Applier, the Sceptic, the Starter.
- **Right or wrong:** partly wrong, and only found out much later. Survey round 1 showed one respondent of four resembling the Mass Applier. See entry 19.
- **Cut or added:** cut three of six drafts. Kept all six in `personas/drafts/` so the discarded ones stay visible.

## 4. Interview 01, filmed, with a real student
**Session 8, 22 September 2026.** Run by Linda.

- **Why:** the evidence log was entirely our own reasoning. We needed one real person.
- **What we wanted to validate:** what makes a student trust a job site, and whether high application volume really fails to convert.
- **Result:** he had sent hundreds of applications, got interviews, and had never been hired through a job site. His condition for trusting a new site was being shown no job that did not suit him.
- **Right or wrong:** it contradicted us. We had assumed explanations build trust. He named accuracy instead.
- **Cut or added:** cut "explanations earn trust" from the centre of the venture. Added accuracy as the trust condition, which eventually became the riskiest assumption in entry 15.

## 5. Venture Skeleton v0.1
**Session 8, 22 September 2026.**

- **Why:** to rebase the whole chain on the first piece of real evidence.
- **What we wanted to validate:** whether one interview changed the venture or merely decorated it.
- **Result:** it changed the success definition. Sending more applications was not the problem; getting hired was.
- **Right or wrong:** right at the time, on n=1.
- **Cut or added:** added "getting hired" to the desired progress. Added a second measurement to the test: how many recommendations students reject.

## 6. Competitor and alternatives scan
**Session 10, 29 September 2026.**

- **Why:** we could not claim a gap without knowing what already existed.
- **What we wanted to validate:** whether anyone already does verified, employer-neutral shortlists.
- **Result:** a four-category alternatives map: direct competitors, substitutes, manual workarounds, doing nothing.
- **Right or wrong:** directionally right, but it was a desk scan of other people's descriptions. Re-run properly on 7 October, see entry 17.
- **Cut or added:** added "doing nothing" as the real competitor, which we had been ignoring.

## 7. Market moved from Europe to the United States
**1 October 2026.** Team decision after class discussions.

- **Why:** we judged the US a better first market for an AI product.
- **What we wanted to validate:** two claims. That US students take up new AI tools more readily, and that the regulatory load is lighter.
- **Result:** the regulatory claim is checkable. The adoption claim is our judgement and nothing more.
- **Right or wrong:** the honest answer is that one of the two reasons is evidence and the other is opinion.
- **Cut or added:** cut Spain and Europe from the entire analysis, including rewriting three personas, the recruitment plan and the press release. Added the two funnels. Added a declared proxy assumption: Spanish survey respondents are treated as a stand-in for US students, and we say so out loud.

## 8. ERRC grid
**1 to 6 October 2026.**

- **Why:** the course requires a strategy statement, and we needed to say what we would deliberately not do.
- **What we wanted to validate:** whether our four moves were genuinely different from the incumbents.
- **Result:** Eliminate employer influence, Reduce breadth of listings, Raise verification depth, Create an entry-level shift monitor.
- **Right or wrong:** three of four have survived contact with evidence. The Reduce row has since been challenged by a real respondent who asked for the opposite. See entry 19.
- **Cut or added:** added the grid. Cut nothing yet, and the Reduce row is now openly under question rather than quietly defended.

## 9. Survey built, then cut from 20 questions to 11
**1 October 2026.**

- **Why:** one interview is not evidence. We needed a second, wider test.
- **What we wanted to validate:** whether interview 01's trust condition generalises.
- **Result:** a live 11-question survey with decision rules fixed in writing before any answer arrived.
- **Right or wrong:** cutting it was right. A 20-question survey that nobody finishes measures nothing.
- **Cut or added:** cut nine questions, including both payment questions and the trigger question, and moved them to the interviews where follow-ups are possible.

## 10. Technical spike on the shift monitor
**6 October 2026.**

- **Why:** the Create row promised something we had never checked was buildable.
- **What we wanted to validate:** whether free data supports a per-role claim that AI is shrinking a job.
- **Result:** no. Feasible only in a reduced, sector-level form using Indeed Hiring Lab, BLS and O*NET.
- **Right or wrong:** wrong as originally promised. The spike contradicted our own Create row.
- **Cut or added:** cut the per-role AI-causation claim. The contradiction is left visible in the file rather than smoothed over.

## 11. Repository restructured into the three layers
**Session 12, 6 October 2026.**

- **Why:** the course defines one repository with three layers of truth.
- **What we wanted to validate:** nothing. This was compliance with a required structure.
- **Result:** evidence-log, specs, AGENTS.md and agents/ in place.
- **Right or wrong:** right, and worth noting we got the structure right while getting the contents of `prototype/` wrong. See entry 20.
- **Cut or added:** renamed `interview-evidence.md` to `user-feedback.md` and updated every reference. Added `.gitignore` so no key can be committed.

## 12. Persona Agent rehearsal
**6 October 2026.** Prompted by the professor's question in class.

- **Why:** he asked whether we had used our personas to prompt an AI and take their perspective.
- **What we wanted to validate:** whether our personas would challenge our own assumptions if we argued with them.
- **Result:** all three synthetic personas agreed to use the product. That is the known failure mode of the technique.
- **Right or wrong:** the exercise was useful, the output was not evidence. We said so.
- **Cut or added:** cut every agreeable answer. Kept only the objections and turned them into five new interview questions.

## 13. Graded feedback received, 5.68 out of 8
**Previous submission.**

- **Why:** the professor marked the work.
- **What we wanted to validate:** not applicable. This is the result of being marked.
- **Result:** Venture chain, Riskiest Assumption and Experiment fit all marked Revise for the same underlying fault: trust and intended use were mixed together. Rough Test marked Rework at 0 of 0.8. Traceability full marks.
- **Right or wrong:** he was right on every point, and three of the four flagged items were still unchanged in the repository when we re-checked on 7 October.
- **Cut or added:** this entry is the reason for entries 14 to 18.

## 14. The chain collapsed onto one assumption
**7 October 2026.**

- **Why:** the feedback said to pick trust or intended use and carry one through.
- **What we wanted to validate:** which of the two is actually upstream.
- **Result:** we chose trust. A student cannot use a list they do not believe, our whole ERRC grid is a trust strategy, and accuracy is observable where intended use is merely claimed.
- **Right or wrong:** externally checked on 7 October. All four survey respondents named accuracy first, so the choice survived its first test.
- **Cut or added:** cut the word "use" from the assumption, the sprint goal, the metric and the decision rule. Cut the second success signal from the experiment card. Added one metric, the fit rate, and a three-branch decision rule on that single number. "Would you use this?" is still asked and deliberately not scored.

## 15. Test run 01, can a verified shortlist be built by hand?
**7 October 2026.** Desk run, AI-assisted, no participants.

- **Why:** the cheapest possible test, and we had run nothing.
- **What we wanted to validate:** whether the verification our Raise row promises is achievable at all.
- **Result:** 5 of 12 candidates passed all four checks. 2 were already dead links. 4 of the 5 that passed stated no deadline.
- **Right or wrong:** the Raise row survived. Two of our own beliefs did not: that "still open" could be judged by an AI, and that verification was cheap enough to ignore in the plan.
- **Cut or added:** cut the "still open" judgement away from the model entirely; it is now a stated deadline parsed against today's date. Added "deadline not stated" as an honest card state. Added a dead-link check as the first step.

## 16. Test run 02, has this already been done?
**7 October 2026.** Desk run.

- **Why:** the feedback asked us to test whether the idea exists and what differentiates us.
- **What we wanted to validate:** whether anyone already removes employer influence or verifies postings.
- **Result:** nobody publicly claims verification. Handshake is rolling out paid employer promotion inside student feeds, in beta with about 30 employers.
- **Right or wrong:** the Eliminate row got stronger and dated. Our pricing assumption got contradicted: Handshake charges universities about 8,000 dollars a year against the 18,000 we assumed.
- **Cut or added:** added the Handshake promotion rollout as our sharpest contrast. Marked the 18,000 dollar assumption as contradicted rather than merely unproven. Added a pricing question to the careers-office script.

## 17. Privacy and data position
**7 October 2026.**

- **Why:** the feedback asked directly how we handle privacy and data sharing, and we had no answer anywhere.
- **What we wanted to validate:** whether a useful shortlist can be built without a CV.
- **Result:** a position: ask the least that makes a shortlist possible, and hold almost nothing.
- **Right or wrong:** partly undercut two days later. Only 1 of 4 survey respondents picked privacy as a trust factor, so this is a principle we hold rather than a demand students expressed. The file now says that.
- **Cut or added:** added the position. Cut the earlier assumption that we would need CV uploads.

## 18. Survey round 1 read against the pre-set rules
**7 October 2026.** n=4 on our own form. A parallel form run by another team is still to be merged as round 2.

- **Why:** the rules were fixed in advance, so the data had to be read against them whatever it said.
- **What we wanted to validate:** six pre-committed thresholds covering trust, tolerance, channel and the Create row.
- **Result:** accuracy named first by all four. Nobody chose 1 or 2 as their tolerance for bad matches. All four would use it free through their university. Two of four had already been hired through a platform.
- **Right or wrong:** our trust assumption held. Our push force did not. Interview 01 and the survey now contradict each other on tolerance, and we kept the contradiction rather than averaging it.
- **Cut or added:** cut "students apply at high volume and still do not get hired" from a stated fact to a CHALLENGED assumption about a segment we have not defined. Cut the Job to Be Done circumstance down to an open question. Added three new risks from the written objections, the sharpest being that employers are starting to refuse applications made through agencies or AI tools.
- **Not actioned:** no threshold rule was applied, because the stop condition we set in advance says a sample under 20 is reported as weak rather than presented as percentages.

## 19. The prototype was removed
**8 October 2026.**

- **Why:** the course structure on page 143 keeps `prototype/` empty until Session 16, and the team has not built a prototype. A working page had been generated with AI and committed into that folder, and several files had been written as though the team owned it.
- **What we wanted to validate:** nothing. This is a correction.
- **Result:** `prototype/index.html`, the scoring sheet and the earlier v0.1 PDF and PNG removed, the folder returned to empty, and every claim that a built prototype exists stripped from the other files.
- **Right or wrong:** we were wrong to have it there, and wrong in a way that mattered: the repository claimed an artefact the team had not made. Forward-looking references to a prototype we intend to test with are correct and were kept.
- **Cut or added:** cut the prototype and all claims arising from it. The Rough Test criterion from the graded feedback still needs an answer, and it will be a sketch shown on the day rather than a built page in this folder.
