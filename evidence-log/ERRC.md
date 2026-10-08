# Eliminate-Reduce-Raise-Create Grid

**Status:** Team-confirmed structure, 6 October 2026. The four strategic moves below were decided by the team. The evidence status of each move is unchanged: this is a value innovation hypothesis, not a validated blue ocean.

**Target user:** US undergraduates looking for a job or an internship

**Job to Be Done:** Find openings that really fit their profile and interests, so applications turn into interviews and offers instead of hours of searching and mass applying (evidence-log/jtbd.md)

**Strongest current alternative:** the manual routine of mass applying, carried out inside Handshake and LinkedIn, which US careers offices put in front of students by default

**Evidence basis for the baseline:** interview 01 (n=1): hundreds of applications through job platforms, some interviews, never hired through one. Supported by NACE 2025 (about 30 applications per role) and by the New York Fed (42% underemployment among recent graduates, Q2 2026). Limitation: our only user evidence is one interview, conducted in Europe. The survey and the 7 filmed interviews test whether this baseline holds.

## ERRC Grid

| Action | Strategic move | Assumption challenged | Cost effect | Buyer value effect | Evidence status | What must be verified |
|---|---|---|---|---|---|---|
| Eliminate | Employer influence over what a student is shown. Employers may still pay for other things, such as a verified employer profile or aggregate hiring analytics, but they can never buy position, visibility or ranking in a student's list | That early-career platforms are funded by letting the side that wants attention pay for it, which is how Handshake and LinkedIn monetise | Removes paid-placement revenue and the sales operation behind it. A smaller employer revenue line survives through products that do not touch ranking, so the gap the university payer must close is narrower than a total ban | Nothing a student sees is there because an employer paid for it, and we can say that without an asterisk | Plausible hypothesis | Whether students notice or care about paid ranking today, and whether non-ranking employer products plus university licences actually cover the gap |
| Reduce | Breadth of listings shown, far below the market standard | That more postings mean a better service | Less indexing, storage and matching across roles we will never show | Less time lost on roles that were never realistic | Partly supported: interview 01 said trust starts when no unsuitable job is shown. Survey Q7 measures the tolerance | How few results a student accepts before the service feels empty rather than focused |
| Raise | Verification depth per posting. Every listing we show is checked as real, still open, and explicit about work authorisation, and carries a plain reason why it fits this student and what does not fit | That a posting is worth showing simply because it exists in a feed, and that the student should do the checking | More verification work per listing, whether automated or manual, and a catalogue that grows more slowly | A student can act on the list without re-checking every posting, and international students can see immediately whether they are eligible | Partly supported: interview 01 (n=1). Survey Q6 measures what earns trust | Whether verification is the factor students value, how much it costs per listing at scale, and whether work-authorisation status can be read reliably from postings |
| Create | An entry-level shift monitor: which entry-level roles in the student's field are shrinking as AI absorbs tasks, and which adjacent roles their profile already transfers to | That a careers tool only matches a student to today's openings | New data pipeline, occupation mapping and maintenance | A student can see where their field is heading before spending a year applying into it | Unsupported novelty, feasibility spike planned | Whether students want it, whether posting data supports a credible signal, and the cost of telling someone wrongly that their target role is shrinking |

## How the four moves differ from each other

- **Eliminate** sets employer influence over ranking to zero. It is about who the list serves.
- **Reduce** lowers the number of postings shown, far below the standard. It is about quantity.
- **Raise** increases what we know and state about each posting we do show. It is about depth per item.
- **Create** adds a factor no alternative offers at all: a forward view of the student's field.

Quantity down, depth up, influence gone, foresight added. No two rows describe the same benefit.

## Value innovation hypothesis

We do not compete on how many jobs we can show. We show far fewer, verify every one of them, and never let an employer buy a place in the list, and we add a view of which entry-level roles are disappearing. Lower cost comes from a far smaller catalogue and no paid-placement sales operation. Higher buyer value comes from a list that can be acted on without double-checking, and from foresight no current alternative offers.

This remains a hypothesis, not a validated blue ocean or a confirmed business model.

## Team decisions recorded on 6 October 2026

1. **Reduce stays breadth, Raise becomes verification depth.** The earlier draft had Reduce (fewer listings) and Raise (match accuracy) describing one benefit twice, which the course's own ERRC guidance rules out. Depth per posting is a genuinely different factor from the number of postings.
2. **Employers may pay, but never for visibility.** The team chose this over a total ban on employer money. It keeps a revenue option open while the claim "nothing here is paid placement" stays true.

## Why the US changes the grid

The Eliminate row is sharper here than in Europe, because the dominant US player monetises exactly what we remove: employer access to students. The channel is harder, because Handshake already sits inside 1,200 careers offices, so our university route is a competition rather than an open door. See evidence-log/market-research.md, funnels A and B.

## Critical outstanding validation points

1. How many unsuitable matches a student tolerates before abandoning the tool. This sets the bar for the Reduce row.
2. Whether verification depth is what earns trust, or whether students only want fewer, better matches and do not care how we got there.
3. Whether a US careers office will adopt a second tool alongside Handshake. The partnership funnel rests on this and has no evidence.
4. Whether non-ranking employer products plus university licences can replace paid-placement revenue.
5. Whether the entry-level shift monitor is wanted by students or only interesting to us.

## Evidence boundaries

- Based on real evidence (n=1): trust begins with never showing an unsuitable job; high application volume produces interviews but no hire.
- Based on team judgement: the employer-influence rule, the university payer, the shift monitor, and every partnership figure in market-research.md.
- Open contradiction: our Sceptic persona assumed explanations earn trust, while interview 01 named accuracy. Survey Q6 separates them.
- Declared assumption: our survey respondents are mostly in Spain and the team treats their behaviour as a proxy for US students.

## Rehearsal pressure test, 6 October 2026

Our three Personas were run as synthetic Persona Agents against this grid (evidence-log/persona-agent-rehearsal.md). The session produced four challenges. None is evidence; all are now questions for the 7 real interviews.

1. **Reduce** assumes fewer is better. The floor at which a short list reads as empty rather than focused is unknown.
2. **Raise** is worth much less to an international student if work-authorisation status cannot be stated reliably, which the data spike lists as unproven.
3. **Eliminate** is a cost and integrity move rather than a persuasion lever, so it should not lead the pitch.
4. **Create** should lead with the adjacent roles a profile transfers to, not with a warning that a field is shrinking. This also matches what the spike says we can actually build.

The synthetic session ended with all three Personas saying they would try the product, which is the known failure mode of synthetic Personas. Only the objections were kept.

## Survey round 1 against the grid, 7 October 2026

Four real students. Counts, not percentages, because n=4. Full results in [survey.md](survey.md).

| Row | What round 1 says | Verdict |
|---|---|---|
| **Eliminate**: employer influence over what a student is shown | Not asked directly. Test run 02 is the stronger evidence here: Handshake is rolling out paid employer promotion inside student feeds | Unchanged, and strengthened from elsewhere |
| **Reduce**: breadth of listings | **Challenged.** One respondent asked for the opposite, in writing | See below |
| **Raise**: verification depth per posting | Consistent. All 4 named accuracy first; 3 of 4 named provenance; 3 of 4 named verified employers. Those are the three things this row delivers | Unchanged, still resting on interview 01 and test run 01 rather than on four answers |
| **Create**: entry-level shift monitor | Consistent. 4 of 4 said it would change what they apply for | Unchanged, still bounded by spike-shift-monitor.md |

## The Reduce row has its first real objection

> "No clear distinction where the job offers come from and little integrations to job search engines. **I would like a platform that centralizes all the job offers in one place**"
> Survey round 1, Q8, verbatim

This is awkward and it should stay awkward. Our Reduce row deliberately shows a student fewer listings. One of the four people we have asked wants more of them, in one place, which is the aggregator model we defined ourselves against.

**What we are not doing:** quietly rewriting the row, or reading the same answer as support because its first half asks for provenance, which our Raise row does provide.

**What the objection actually splits into.** The same sentence contains a complaint and a request. The complaint is that a student cannot tell where an offer came from, which is precisely what we raise. The request is for everything in one place, which is what we reduce. So the respondent is not rejecting verification; they are refusing to trade coverage for it. That is the real trade our strategy makes, and it has now been questioned by a real person.

**What decides it.** A direct question in the seven interviews, asked after the student has seen the six-card shortlist rather than in the abstract: would you rather have these six checked, or sixty unchecked? A preference stated before seeing a shortlist and a preference stated after are different measurements, and only the second one is worth anything here.

**What happens if the interviews side with coverage.** The Reduce row is rewritten, not deleted: reduce the breadth of what is *shown first* rather than the breadth of what is *held*. That is a different venture from the one in the current grid, so the team decides it, not the evidence log, and not AI.

## One more thing round 1 took away

Only 1 of 4 picked "my data stays private" as a trust factor, the joint lowest of the six options. Nothing in the grid rests on privacy, so no row changes. But if privacy appears on a slide as a reason students would choose us, that is not supported by anything we have collected, and [privacy.md](privacy.md) now says the same: it is a position we hold, not a demand we found.
