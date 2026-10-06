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
