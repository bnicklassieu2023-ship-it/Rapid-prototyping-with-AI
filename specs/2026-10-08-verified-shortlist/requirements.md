# Requirements: the verified shortlist

Feature spec for Step 1 of [../roadmap.md](../roadmap.md). Written 8 October 2026.

**Nothing in this folder is built.** `prototype/` stays empty until Session 16. This document exists so that when the build starts, it starts from a specification the team argued about rather than from a prompt typed in the moment.

## Why this feature and not another one

Step 1 is the thinnest thing that can test the riskiest assumption in [../../evidence-log/assumptions.md](../../evidence-log/assumptions.md) v0.4: that students will judge an AI-built shortlist as accurate. The shift monitor is more impressive, the rejection-learning loop is more interesting, and neither tests anything we need to know first. If students do not recognise our five openings as fitting them, nothing downstream matters.

## What a student does

One screen, one action, one list.

1. The student answers four questions: field, location, year of study, and whether they need visa sponsorship.
2. They receive five openings.
3. Each opening shows one line on why it is there and what is uncertain about it.
4. They mark each one "fits me" or "does not fit me", and give one line of reasoning on every rejection.

That is the whole feature. Anything that is not on that list is out of scope, and the out-of-scope list below is the part of this document most likely to be ignored under time pressure, which is why it is written down.

## Functional requirements

| ID | Requirement | Source | Label |
|---|---|---|---|
| R1 | Intake asks exactly four questions: field, location, year of study, sponsorship needed yes or no | [privacy.md](../../evidence-log/privacy.md) | DESIGN DECISION |
| R2 | No account, no login, no email address required to receive a shortlist | privacy.md | DESIGN DECISION |
| R3 | No CV, transcript or document upload anywhere in the flow | privacy.md | DESIGN DECISION |
| R4 | Every opening shown has been confirmed to resolve to a live page before it is shown | [run 01](../../evidence-log/test-runs/run-01-shortlist-feasibility.md): 2 of 12 candidates were dead, HTTP 410 and HTTP 404, while still appearing in search results | OBSERVED |
| R5 | "Still open" is never a model judgement. The posting's own stated deadline is shown, compared against today's date | run 01: the model misread posting status on 2 of the 3 postings it read | OBSERVED |
| R6 | Where a posting states no closing date, the card reads "deadline not stated". It never reads "open" | run 01: 4 of the 5 verified openings stated no closing date at all | OBSERVED |
| R7 | The employer's work authorisation position is quoted from the posting, not summarised. A mention of E-Verify is treated as "not stated" | run 01: E-Verify reads like an answer to sponsorship and is not one | OBSERVED |
| R8 | Each card carries one line on why this opening is here, and one line on what is uncertain | Survey round 1: 3 of 4 named "it explains why each job fits me" and 3 of 4 named "I can see where the posting came from" as trust conditions, n=4 | REPORTED |
| R9 | Employers cannot pay for placement, ordering or visibility anywhere in the list | [ERRC.md](../../evidence-log/ERRC.md) Eliminate row; run 02 found Handshake rolling out paid employer promotion in student feeds | DESIGN DECISION |
| R10 | Five openings per shortlist for the first test | roadmap Step 1 | ASSUMPTION, see open questions |

## Explicitly out of scope

Each line is here because somebody will otherwise suggest it.

- Writing or auto-filling applications, resumes or cover letters. It conflicts with our non-goals, and survey round 1 produced an unprompted objection against exactly this: one respondent wrote that employers are starting to refuse applications submitted through agencies or AI tools, and asked whether that affects our idea. It does, and the answer is that we never apply on a student's behalf.
- Any employer-facing surface at all.
- Accounts, saved profiles, or any persistence between sessions.
- University system integration. No careers office has agreed to anything. 0 of 2 conversations held.
- The shift monitor. Step 3, and bounded by [spike-shift-monitor.md](../../evidence-log/spike-shift-monitor.md).

## Open questions we are not pretending to have answered

| Question | Why it is open | Who settles it |
|---|---|---|
| Is five openings a careful search or a weak one? | The Synthetic Persona rehearsal flagged that five results may read as a thin search rather than a thorough one. Nobody real has told us | The 7 interviews |
| What triggers a student to start searching at all? | The trigger question was cut from the short survey and remains an open gap in [jtbd.md](../../evidence-log/jtbd.md) v0.2 | The 7 interviews |
| Do students want a narrow verified list or broad coverage? | Survey round 1 produced one respondent asking for the opposite of our Reduce row: "I would like a platform that centralizes all the job offers in one place" | The 7 interviews |
| How many bad matches before trust breaks? | Interview 01 said one. Round 1 said 3 to 5 or more, with nobody choosing 1 or 2. Our two real-user sources contradict each other | The 7 interviews |
| What does verification cost per usable opening? | 12 page checks produced 5 openings and this appears in neither funnel | Before the next revision of market-research.md |

## The sample this rests on, stated plainly

One interview, four survey responses on our own form, two desk runs, and three AI personas that count as nothing. Round 2 of the survey has not been merged. Every requirement labelled REPORTED above rests on four people, and the two labelled ASSUMPTION rest on nobody.
