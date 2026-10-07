# Venture Skeleton v0.1

**Status:** Updated from v0 after persona research and 1 real-user interview, then rebased on the United States market for Group Project I. Still provisional.

| Field | v0.1 | Changed? | Source |
|---|---|---|---|
| Opportunity | US undergraduates looking for jobs and internships apply at high volume and still struggle to find openings that really fit | Refined twice: target narrowed, then market set to the United States on 1 October 2026 | opportunity.md, opportunity-v02.md, user-feedback.md |
| Product Goal | Help students and recent graduates reduce time and uncertainty when identifying the right job or university opportunities | Kept | goals.md |
| Jobs to Be Done | Find openings that really fit their profile and interests so applications turn into interviews and offers. Trigger still unknown | Refined | jtbd.md |
| Personas | The Mass Applier, The Sceptic, The Starter (selected from 6 drafts). Proto-personas, checked against 1 interview | New in v0.1 | personas/ |
| Riskiest Assumption | Users will trust and use AI-generated opportunity recommendations as a first step in their decision process | Kept, word for word | assumptions.md |
| Sprint Goal | Learn whether students trust AI-generated job and internship recommendations enough to use them as a first filter when every match fits their stated profile and interests | New | goals.md |
| Smallest Test | Rough prototype with 5 to 8 students; each marks every recommendation as "fits me" or "does not fit me" | Revised | experiment-card.md |
| Decision rule | 70% first-filter use plus mostly fitting matches: continue. High use but many rejected matches: fix accuracy first. Otherwise narrow scope or redesign trust | Revised, pre-committed | experiment-card.md |

## What changed because of real-user evidence

- Trust: we assumed explanations build trust. Interview 01 linked trust to accuracy (no unsuitable jobs).
- Success: the outcome that matters is getting hired, not sending more applications.
- Test: we now also count how many matches students reject as unsuitable.

## What is still assumption or unknown

- Everything rests on 1 interview. It is a signal, not validation.
- The trigger that starts a search.
- Willingness to share CV and personal data.
- Who pays: students (freemium) or universities.
- Whether The Starter Persona exists as described.

Test access: 5 to 8 students aged 19 to 24 from our network. AI traceability: ai-usage-log.md

## Market size (added for Group Project I)

| Route | Year one | Year three | Source |
|---|---|---|---|
| Without university partnerships | about 1,800 students | not modelled | market-research.md, Funnel A |
| With university partnerships | about 2,160 active students across 3 pilot campuses | about 36,000 active students across 50 campuses | market-research.md, Funnel B |

Starting market: 19.4M US postsecondary students, of whom 16.2M are undergraduates. Every filter below the first two is an assumption or a proxy, and the partnership figures are team planning numbers.

## v0.2 (7 October 2026): the chain, carrying one assumption end to end

**This is the current skeleton. The table at the top of this file is v0.1 and is kept as the audit trail.**

Rewritten because the graded feedback found the chain carrying two assumptions at once: "trust and intended use are mixed together. Choose one and carry it consistently through the test and decision rule." Below, the same word appears in every row.

| Field | v0.2 | Changed from v0.1? |
|---|---|---|
| Opportunity | US undergraduates apply at high volume and still cannot tell which openings are real, still open, and actually open to them | Sharpened. "Really fit" became three checkable conditions after test run 01 |
| Product Goal | Help students reduce time and uncertainty when identifying the right job or internship, with getting hired as the outcome that matters | Kept |
| Jobs to Be Done | Find openings that really fit, so applications turn into interviews. Trigger still unknown | Kept |
| Personas | The Mass Applier, The Sceptic, The Starter. Proto-personas, checked against 1 interview, rehearsed as AI personas and not validated | Kept |
| **Riskiest Assumption** | **Students will judge an AI-built shortlist as accurate, meaning they recognise the openings we show them as genuinely fitting their profile** | **CHANGED.** The "trust and use" wording is gone. This is trust alone, and assumptions.md v0.3 says why trust and not use |
| **Sprint Goal** | **Learn whether students judge the openings we put in front of them as genuinely fitting** | **CHANGED.** One claim, not three |
| **Smallest Test** | **Six real verified openings in a working prototype. Seven students mark each one "fits me" or "does not fit me"** | **CHANGED.** The prototype now exists and the openings in it are real, from test run 01 |
| **Metric** | **Fit rate: the share of shown openings a student marks "fits me". One number** | **NEW.** There was no single metric before, which is what the feedback caught |
| **Decision rule** | **70% or above: continue. 50 to 69%: rewrite the matching criteria and re-run. Below 50%: stop** | **CHANGED.** Three branches on one metric, instead of branches on two signals at once |
| Not measured | Whether they would use it. Asked, recorded, deliberately not scored | **NEW, and deliberate** |
| Status of the test | **Not run. 0 of 7 students.** Owner Linda, 15 October 2026 | Honest, and the gap the Experiment fit criterion is still waiting on |

## Tests actually run since v0.1

| Run | Result |
|---|---|
| [Test run 01](test-runs/run-01-shortlist-feasibility.md), 7 Oct | 5 of 12 candidates passed verification. The AI misread posting status on 2 of 3 postings it read, so that check was taken away from the model |
| [Test run 02](test-runs/run-02-does-this-already-exist.md), 7 Oct | Nobody claims verification. Handshake is building paid employer promotion into student feeds. Our 18,000 dollar university price is contradicted by a public 8,000 dollar comparator |
| [Shift-monitor spike](spike-shift-monitor.md), 6 Oct | Create row feasible only in reduced, sector level form |

## What is still assumption or unknown

- The riskiest assumption is still untested with a student. Everything else here is downstream of that.
- The trigger that starts a search.
- Who pays. Funnel B's price is now contradicted rather than merely unproven.
- Whether any careers office will adopt a second tool. Nobody has been contacted.
- Whether The Starter Persona exists as described.
