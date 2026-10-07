# Privacy and data sharing

**Status: a position, taken 7 October 2026, with one part of it already built and two parts still untested.**

Written because the graded feedback asked directly: "How do you handle privacy and data sharing concern?" We had no answer anywhere in the repository. The honest reason is that we had treated data sharing as a feature question, how much CV data we could get, rather than as the objection it actually is.

## The problem in one line

Our product is more accurate the more it knows about a student, and students are most suspicious of exactly the tools that ask to know a lot about them. Those two pull against each other, and a venture that does not say which way it leans is avoiding the question.

## Where we lean, and why

**We ask for the least that makes a shortlist possible, and we ask for it without an account.**

The prototype asks four things: field, location, year of study, and whether the student needs visa sponsorship. That is enough to do the matching, and it is the test of the claim. If a useful shortlist can be built from four answers and no CV, then the CV was never the price of entry and we should stop assuming it is.

This is also a competitive position, not only an ethical one. [Test run 02](test-runs/run-02-does-this-already-exist.md) found the incumbents monetise the student side through employers: Handshake is rolling out paid employer promotion inside student feeds, and Jobright's pitch is automatic applying at volume. Both of those need to know a lot about a student. A product whose Eliminate row is employer influence has no business building the same data position as the products it is defining itself against.

## What is built today

| Commitment | Status | Where |
|---|---|---|
| No account, no login, no email required to get a shortlist | **Built** | `prototype/index.html` |
| No CV or transcript upload | **Built** | Not asked anywhere in the prototype |
| Nothing the student types leaves the page: no server, no cookies, no analytics, no browser storage | **Built** | The prototype is a single file with no network calls. Open the source and check |
| No secrets or keys in the repository | **Built** | `.gitignore`, added 7 October 2026, and the production principles in `AGENTS.md` |
| Interview and survey consent recorded before filming | **Built** | `recruitment.md`, `survey.md` |
| The survey collects an email only if the student volunteers it for a follow up interview | **Built** | Question 11, optional |

## What is a position, not yet a product

| Commitment | Status |
|---|---|
| We never sell or share student data with employers, and employers never see a student unless the student applies | **Stated, nothing built.** No employer side exists yet to test it against |
| A student can see and delete everything we hold about them | **Stated, nothing built** |
| We do not store rejection reasons against a named student, only against the opening | **Stated.** The prototype does not store anything at all, so this is untested |

These are written down now so that the first version that does store something has to argue against them rather than quietly ignore them.

## What we do not know, and how we will find out

| Open question | How it gets answered |
|---|---|
| Does the four question version actually produce an acceptable shortlist, or does accuracy need the CV after all? | [Test run 03](test-runs/run-03-student-trust-test.md). If the fit rate fails at 50 to 69%, the first thing to check is whether the missing information was the cause |
| Would students share more for better matches, and where is the line? | Survey question "which of these would you share", and the open objection question. Any privacy objection raised by three or more respondents becomes a named risk in `assumptions.md` |
| Does a university careers office have a data position we would have to meet? | Added to the careers office script in `careers-office-outreach.md` |
| Does "we hold nothing" read as trustworthy or as unserious to a student? | Ask it in the trust test sessions, recorded as context, not scored |

## The risk in this position

Holding almost no data is easy at the prototype stage and gets harder with every feature. Roadmap Step 2, where the list improves when a student rejects something, needs a memory of that student. The moment we build it, this page has to be rewritten rather than left as a claim we made once and stopped meeting. Whoever writes Step 2 owns that rewrite.
