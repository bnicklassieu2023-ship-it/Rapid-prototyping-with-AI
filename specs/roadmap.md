# Roadmap

Version 0.1, 6 October 2026. Status: preliminary, to be revisited after the survey and the interviews.

## Step 1: The verified shortlist

A student enters field, location and year of study and receives five openings. Each one is checked as real, still open and explicit about work authorisation, and carries one line on why it fits and what does not. The student marks each as "fits me" or "does not fit me".

**Why this one and not the most impressive one:** it is the thinnest thing that tests our riskiest assumption, that students will trust and use AI-generated recommendations as a first filter [evidence-log/assumptions.md]. The shift monitor is more impressive and tests nothing we need to know first.

**Must pass:** at least 70% of testers say they would use it as a first filter, and most recommendations are marked "fits me" [evidence-log/experiment-card.md].

**Open from the Persona rehearsal:** five results may read as a weak search rather than a careful one. The interviews ask what number feels like a real search.

## Later steps

- **Step 2: Learning from rejections.** The list improves when a student marks something unsuitable. Check: a student's second list has fewer rejected matches than their first.
- **Step 3: The entry-level shift view.** Sector trend, official occupational outlook and adjacent roles, shown beside the student's field, led by where their profile also fits rather than by a warning. Check: a student can say, unprompted, what the view told them. Scope bounded by evidence-log/spike-shift-monitor.md.

## Not in this prototype

- Writing applications, resumes or cover letters, because it conflicts with our non-goals and with why students distrust AI
- Employer-facing tools of any kind, because nothing we build may let an employer influence a student's list
- Accounts, logins and profiles beyond what one test session needs
- Any university integration, because no careers office has agreed to anything yet

## Step 1 revised, 7 October 2026

**This replaces the Step 1 wording above, which is kept as the audit trail.**

Two things changed it: the graded feedback on the venture chain, and what test run 01 found when we tried to build a verified shortlist by hand for the first time.

### Step 1: the verified shortlist

A student enters field, location, year of study and whether they need sponsorship, and receives openings that have each been checked as a real posting, with their stated deadline shown, with the student's eligibility checked, and with the employer's work authorisation position quoted. Each carries one line on why it is there. The student marks each "fits me" or "does not fit me".

**Must pass:** a **median fit rate of at least 70%** across at least five students. One metric. [evidence-log/experiment-card.md](../evidence-log/experiment-card.md), v0.2.

The previous wording, "at least 70% of testers say they would use it as a first filter, and most recommendations are marked fits me", measured two different things and could not be cleanly failed. Whether a student would use it is still asked, and is still recorded, and no longer counts.

**Why this step and not a more impressive one:** it is the thinnest thing that tests our riskiest assumption, that students will judge an AI-built shortlist as accurate [evidence-log/assumptions.md, v0.3]. The shift monitor is more impressive and tests nothing we need to know first.

### Three changes forced by test run 01

| Change | Why |
|---|---|
| "Still open" is never a model judgement. The posting's stated deadline is parsed and compared against today's date, and shown to the student | The model misread posting status on 2 of the 3 postings it was asked to read |
| Where no deadline is stated, the card says "deadline not stated". It never says "open" | 4 of the 5 verified openings stated no closing date at all |
| A dead link check runs first, before anything else | 2 of 12 candidates were already dead, HTTP 410 and HTTP 404, while still appearing in search results. It costs one request and saves the student the click |

### The cost we had not counted

Twelve page checks produced five usable openings. Verification is not a feature, it is a unit cost, and it appears nowhere in either funnel in market-research.md. Before the next funnel revision, somebody has to put a number on it.

**Open from the Persona rehearsal:** five or six results may read as a weak search rather than a careful one. The interviews ask what number feels like a real search.
