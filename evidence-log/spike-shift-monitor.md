# Technical spike: the entry-level shift monitor

**Date:** 6 October 2026
**Question:** can we build a credible signal telling a student which entry-level roles in their field are shrinking, using data we can actually get for free?
**Why it matters:** this is the Create row of our ERRC grid and it was marked "unsupported novelty". Without an answer we are promising something we cannot cost.
**Method:** desk spike. Search for public data sources with occupation or sector granularity, check licence, update frequency and access route. No code written.

## What we found

| Source | Granularity | Freshness | Access and licence | Useful for |
|---|---|---|---|---|
| Indeed Hiring Lab, job postings tracker | Country, sector, US metros and states | Daily data refreshed weekly | Public repository, CSV, Creative Commons Attribution 4.0 | Showing that postings in a sector are rising or falling now |
| Indeed Hiring Lab API | Finer slices | Current | Documented, access terms not confirmed for a student project | Would be needed for true occupation-level real-time trends |
| BLS Employment Projections | Occupation level, national | Ten-year projections, updated annually | Free, public | Which occupations are projected to decline, and by how much |
| O*NET | Occupation taxonomy, skills, related occupations | Periodic | Free, public | Mapping a student's field to adjacent roles their profile transfers to |

## Verdict

**Feasible in a limited form, not in the form we described.**

- Buildable now with free, licensed data: a sector-level trend, the official ten-year outlook for the target occupation, and a list of adjacent occupations.
- Not buildable without paid or permissioned data: a live, occupation-level claim that a specific entry-level role is shrinking right now because of AI. Sector data is not occupation data, and projections are not real-time.
- Attribution to Indeed Hiring Lab is required wherever their data appears.

## What this changes

1. The Create row drops the implied real-time precision. It is a sector trend plus an official outlook plus adjacent roles.
2. Attribution becomes a product constraint, not a footnote.
3. Causation stays out. None of these sources shows that AI caused a decline.
4. From the Persona rehearsal: the view should lead with adjacent roles rather than with a warning, which also fits what the data supports.

## What is still unknown

- Whether students find a sector-level signal useful or too vague. Survey Q10 describes the richer version, so a positive answer there over-reads what we can build.
- Whether Hiring Lab API access is open to a student project.
- The cost of keeping occupation mappings current.

## Sources

- Indeed Hiring Lab job postings tracker, public repository, 11 countries including the US, sector level, CC BY 4.0, accessed 6 October 2026
- Indeed Hiring Lab API documentation, accessed 6 October 2026
- US Bureau of Labor Statistics, Employment Projections, accessed 6 October 2026
- O*NET occupational taxonomy, accessed 6 October 2026
