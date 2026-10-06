# Tech stack

Version 0.1, 6 October 2026. Status: preliminary. **The team has not answered the five stack questions yet**, so every row below is either a constraint we already know or an explicit TBD. No tool appears without a reason.

| Layer | Choice | Why | Status |
|---|---|---|---|
| How the user interacts | TBD | Needs the team's answer to question 1 below | Missing |
| Where job postings come from | TBD. Our hardest dependency | A live posting source is required for Step 1 of the roadmap and we have no free route yet | Missing |
| Trend data for the shift view | Indeed Hiring Lab open data, sector level | Free under Creative Commons Attribution 4.0, refreshed weekly | Evidence-supported: evidence-log/spike-shift-monitor.md |
| Occupation reference data | BLS Employment Projections and O*NET | Free and public, occupation level, needed to map a field to adjacent roles | Evidence-supported: same spike |
| Where data lives | TBD, local files or a free hosted database | Prototype scale only, a handful of test users | Missing |
| What processes it | TBD | Depends on whether matching is rules-based or model-based | Missing |

## AI role

Our Job is to show fewer, better-verified matches. The deterministic checks (does this posting exist, is it still open, does it state work authorisation, does it match the stated field and location) should be rules, not a model. AI earns its place reading messy posting text and writing the plain reason a role fits. When it is wrong the result is a bad match, which is exactly what breaks trust, so every AI output needs a check before a student sees it. [Team decision pending]

## Accounts and keys

- Job posting source: TBD, free route unknown. Biggest technical dependency
- Indeed Hiring Lab data: free, CC BY 4.0, attribution required wherever it appears
- BLS and O*NET: free, public

## Questions the team still has to answer

1. What must the first prototype let a student do, end to end, in one sentence?
2. Which layers do we actually need for that, and which can we skip?
3. For each layer we keep, what is the simplest thing we already know or can learn this week?
4. Where does AI belong, and what happens when it is wrong?
5. Which accounts, keys or paid services would we depend on, and is there a free route?
