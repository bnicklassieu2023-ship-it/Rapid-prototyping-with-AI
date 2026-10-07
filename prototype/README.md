# Prototype

**v0.2, 7 October 2026. The files are in this folder. Nothing here is a list of files to add.**

The previous version of this file listed two files that were never committed, and the graded feedback picked that up: "Add the actual rough prototype and a backup. The README lists files to add, but the submission does not include them." That is fixed. Everything named below is in this folder.

## What is here

| File | What it is |
|---|---|
| `index.html` | **The prototype.** Open it in any browser. No install, no server, no internet needed |
| `prototype-v01.pdf` | The earlier paper version, v0.1, kept as the backup and as the audit trail |
| `prototype-v01-backup.png` | Image backup of v0.1, for the slides and in case the PDF will not open on the day |
| `scoring-sheet.csv` | One row per student. The fit rate from each session goes here |

If `index.html` will not open on the day of the presentation, the PDF and the PNG are the backup.

## What it does

1. Asks the student four questions: field, location, year of study, whether they need visa sponsorship.
2. Shows six openings. For each one: the facts, a line on why it is on their list, the verification status of each of our four criteria, any gap we could not close, and a link to the original posting.
3. The student marks each one "fits me" or "does not fit me", and gives one line of reasoning for every rejection.
4. It calculates the **fit rate**, which is the single metric of test run 03, and produces a result block to paste into `scoring-sheet.csv`.

## What it is honestly not

**The shortlist is picked by hand. There is no matching algorithm behind this page.** This is a wizard of oz prototype and the repository says so in every place it is described. The six openings were found, opened and verified by a person on 7 October 2026 in [test run 01](../evidence-log/test-runs/run-01-shortlist-feasibility.md), and they are hard coded into the page.

That is deliberate, and it is the course's own point: you do not need a build to start testing. We are testing whether a student accepts a shortlist as accurate. If they do not accept a hand picked one, no amount of engineering will save an automated one.

## The openings are real

All six are genuine postings that were open on 7 October 2026, with working links, stated pay where the employer stated it, and the eligibility gates left in rather than smoothed over. Five of the six passed all four of our verification criteria. The sixth, Constellation Brands, is shown with its gap marked, because the product position is that we show what we could not confirm rather than hiding it.

They are a snapshot. By the time of the presentation some will have closed, and the Endeavor one closes on the day it was found. That is the point of the venture, so it is not a flaw to apologise for on stage. It is the demonstration.

## Data

Nothing the student types leaves the page. No account, no CV upload, no server, no cookies, no analytics, no browser storage. The answers live in the tab and are gone when it closes. The only record that survives is the fit rate the operator copies into the scoring sheet by hand. See [evidence-log/privacy.md](../evidence-log/privacy.md).

## How to run a session

Protocol, threshold and decision rule are in [test run 03](../evidence-log/test-runs/run-03-student-trust-test.md). The short version: fifteen minutes, hand over the laptop, say nothing, and never defend a card.

## Version history

| Version | Date | What changed |
|---|---|---|
| v0.1 | Session 8 | Paper prototype, PDF and PNG. Designed, never run with a student |
| v0.2 | 7 Oct 2026 | Working HTML prototype with six verified real openings and built in fit rate scoring. Built in response to the graded feedback on Rough Test and Experiment fit |
