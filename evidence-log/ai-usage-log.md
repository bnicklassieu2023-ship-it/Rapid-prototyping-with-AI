# AI Usage Log

## Tool used
ChatGPT

## Where AI helped
- Framing the opportunity clearly
- Structuring the product goal and sprint goal
- Mapping assumptions
- Drafting the first experiment card
- Suggesting a beginner-friendly GitHub repository structure

## What the team verified manually
- The final wording of the business idea
- The selected target user
- The riskiest assumption to test first
- The final experiment design and threshold

## Notes
AI was used as a support tool for ideation, structuring, and drafting. Final decisions were reviewed and confirmed by the team.


## v0.1 (Session 8): AI Usage Log table

| Date | Tool & version | Stage/ Step | Use | Output used | Student's decisions |
|---|---|---|---|---|---|
| Sessions 3 to 5 (date not recorded) | ChatGPT (version not recorded) | Opportunity, goals, assumptions, experiment card | Framing the opportunity, structuring product and sprint goals, mapping assumptions, drafting the experiment card, suggesting a repository structure | opportunity.md, goals.md, assumptions.md, experiment-card.md, repo structure | Team confirmed the business idea wording, target user, riskiest assumption, experiment design and 70% threshold |
| 2026-09-21 | Claude (Cowork), claude-opus-5 | Session 6: Jobs to Be Done | Drafted the working Job from our existing evidence log and marked the evidence status of each element | jtbd.md v0 | Linda kept the trigger as an open gap instead of inventing one |
| 2026-09-21 | Claude (Cowork), claude-opus-5 | Session 6: Personas | Researched secondary sources (NACE, Eurostat, Handshake) and drafted three proto-personas with evidence boundaries | personas/ai-persona-01 to 03, drafts/persona-hypothesis-01 | Linda set the target (students 19 to 24, jobs and internships), chose the three personas and kept them labelled as not validated |
| 2026-09-21 | Claude (Cowork), claude-opus-5 | Session 8 presentation | Rebuilt the Canva persona slides and a known vs. assumed slide | Canva deck | Linda chose the design direction and cut the text to decision-relevant traits |
| 2026-09-22 | Claude (Cowork), claude-opus-5 | Session 8: real-user evidence | Drafted short interview questions about past behaviour | Interview question list | Linda rewrote questions 3 and 4, then ran and filmed the interview with a real student herself |
| 2026-09-22 | Claude (Cowork), claude-opus-5 | Session 8: evidence trail and Venture Skeleton v0.1 | Turned the interview answers into user-feedback.md, updated jtbd.md, personas and the v0.1 sections of our evidence files, drafted persona-hypothesis-02 to 06, and added the "From assumption to evidence" slide | user-feedback.md, jtbd.md, personas/, goals.md, assumptions.md, experiment-card.md, opportunity.md, venture-skeleton-v0.1.md | Linda confirmed the interview answers are from a real student. The team kept the riskiest assumption unchanged. AI answers were not used as validation |

Synthetic or AI-written answers were only used to rehearse the interview, never as evidence.
| 2026-09-29 | Claude (Cowork), claude-opus-5 | S10 · Market research | Searched for and summarised direct competitors, substitutes and manual alternatives for our segment | Competitor list and positioning read-out used in market-research.md | Linda asked for direct competitors specifically; the team must still verify pricing and Spanish availability before presenting |
| 2026-10-01 | Claude (Cowork), claude-opus-5 | S10-S11 · Group Project I setup | Read the new course slides, checked the repository against the required structure, and added the missing ai-prompt-ERRC.md helper to downloads after verifying its checksum against the course file | Complete downloads folder; gap list for Group Project I | Linda set the critical test herself: 7 filmed interviews plus a survey to double-test |
| 2026-10-01 | Claude (Cowork), claude-opus-5 | S10-S11 · Market scan, ERRC and survey | Drafted market-research.md with the four-category alternatives map and a sourced Fermi funnel, a draft ERRC grid, recruitment.md, the press-release opener and the survey instrument with decision rules set before data collection | Draft files committed to the repository for team review | Draft only. Every ERRC row and every funnel assumption is marked for team confirmation; figures to be re-checked against the original sources by the team before the presentation |
| 2026-10-01 | Claude (Cowork), claude-opus-5 | S10-S11 · Survey build | Built the survey in Google Forms from our draft, shortened it from 20 to 11 questions on request, and checked the live form question by question | Live survey at forms.gle/mxvmrjHJAyEPbP3V6 and a linked response sheet | Linda authorised the Google account access herself, asked for the shorter version, and sends the link to respondents. Decision rules were fixed before any answers arrived |
| 2026-10-01 | Claude (Cowork), claude-opus-5 | S10-S11 · Consistency pass | Checked every existing evidence-log file against the new US scope and rebased the three personas, recruitment.md and the Venture Skeleton so no artifact still describes a Spanish market | personas 01 to 03 rewritten for the US, recruitment and skeleton updated | Linda instructed that the market is the US only and that Spanish survey respondents may be treated as a proxy. The team must still confirm the persona details, which remain hypotheses with no US user interviewed yet |
| 2026-10-01 | Claude (Cowork), claude-opus-5 | S10-S11 · Market scope rationale | Checked the EU AI Act compliance timeline and the comparable US position, then wrote up the team's reasons for moving from Europe to the United States with an evidence label on each one | market-research.md section 0; scope note in opportunity-v02.md | Linda stated the reasons: class discussions, US openness to new AI providers and lighter regulation. The team's judgement is recorded as judgement, and the one claim we cannot yet support (that US users adopt more readily) is flagged for checking before it is said on stage |
| 2026-10-06 | Claude (Cowork), claude-opus-5 | S12 · Repository structure | Re-read the course site, found Sessions 12 and 13 published with a new helper, added downloads/ai-prompt-constitution.md after checksum verification, moved the Persona Agent to agents/persona-agent.md, wrote a coding-agent AGENTS.md pointing at specs/, and renamed interview-evidence.md to user-feedback.md with every reference updated | Repository now matches the Session 12 three-layer structure | Linda asked to follow the course structure exactly. The team owns every line of the constitution and has not yet answered the tech-stack questions |
| 2026-10-06 | Claude (Cowork), claude-opus-5 | S12 · Constitution v0.1 | Drafted specs/mission.md from the evidence log with a claim status on each line, plus preliminary tech-stack.md and roadmap.md leaving the team's open decisions as explicit TBDs | specs/ v0.1 | Draft only. The five tech-stack questions are listed unanswered in the file rather than filled in by AI, and were sent to the team to answer |
| 2026-10-06 | Claude (Cowork), claude-opus-5 | S11 · Shift-monitor spike | Desk spike on whether free data supports the entry-level shift monitor: checked Indeed Hiring Lab open data, its API, BLS Employment Projections and O*NET for granularity, freshness and licence | evidence-log/spike-shift-monitor.md, verdict that the feature is feasible only in a reduced, sector-level form | The team must decide whether to reword the Create row. The spike contradicts the original promise and that contradiction is left visible |
| 2026-10-06 | Claude (Cowork), claude-opus-5 | S10-S11 · Decision table and outreach | Drafted the decision table with thresholds and stop conditions, and a careers-office outreach script with decision rules set in advance | experiment-card.md decision section; careers-office-outreach.md | Owners and dates proposed and marked as needing team confirmation |
| 2026-10-06 | Claude (Cowork), claude-opus-5 | S6-S9 · Persona Agent rehearsal | Ran our three Personas as synthetic Persona Agents against the ERRC grid and the riskiest assumption, with course evidence labels on every answer, then kept the objections and discarded the agreement | evidence-log/persona-agent-rehearsal.md; four challenges recorded in ERRC.md; five questions added to the interview guide | Linda asked for this after the professor's question. The team treats none of it as validation: all three synthetic Personas ended up agreeing to try the product, which is the known failure mode, so only the objections were kept and turned into questions for real students |
