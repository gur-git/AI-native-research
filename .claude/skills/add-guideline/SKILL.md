---
name: add-guideline
description: Draft a methodology guideline based on accumulated evidence and one or more foundation attributes. Each guideline starts as proposed, can move to testing, then adopted or retired. Use when the evidence is strong enough to warrant trying a practice, not just describing a problem.
---

# add-guideline

Promote a methodological practice from "thing the foundation suggests" to "thing the methodology proposes trying." Guidelines live in `methodology/guidelines.md` and accumulate over time. Each one is tied to the attribute(s) it addresses and the evidence that motivated it.

## When to invoke

- A foundation attribute (or cluster of attributes) has been stable for a while, and a practice that addresses it has emerged from evidence or a structured experiment.
- Multiple pieces of evidence converge on the same recommended practice.
- The maintainer or a collaborator has tried something and it appears to work, and is ready to be written up so it can be tested more deliberately.

Do not invoke to add aspirational practices. A guideline must trace to evidence, not to what would be nice.

## Inputs to gather

1. **Name** — short, imperative-mood title. Example: *"Score AI-generated hypotheses against your own ranking before showing the AI."*
2. **Diagnostic motivation** — which attribute(s) does this address? Reference by number from `foundation/01-ai-attributes.md`.
3. **The practice** — concretely, what does the researcher do? Step-level, not principle-level.
4. **Evidence trail** — which evidence files motivated this? List by path.
5. **Status** — where is this guideline in its lifecycle?
   - `proposed` — written down, not yet tested.
   - `testing` — being trialed in real research work; data being collected.
   - `adopted` — evidence supports it; promoted to the live methodology.
   - `retired` — evidence contradicts it, or it was superseded by a better practice. Keep retired guidelines in the file; do not delete.
6. **What success looks like** — how will the researcher know this guideline is helping? Specific, measurable where possible.
7. **Known costs** — what does this guideline cost in time, attention, or friction? Honest accounting.

## File to write

Append to `methodology/guidelines.md`. Each guideline is a section with this shape:

```markdown
## G{N}: <Name>

**Status:** proposed | testing | adopted | retired (last reviewed YYYY-MM-DD)
**Addresses attribute(s):** N, N
**Evidence trail:** [file](../evidence/...), [file](../evidence/...)

### Practice

<step-level description>

### What success looks like

<observable outcome>

### Known costs

<honest accounting>

### Notes

<edge cases, things you've already learned not to do, related guidelines>
```

Number guidelines sequentially (G1, G2, ...) and never reuse a number, even if the guideline is retired.

## After writing

Append a log entry:

```markdown
## Guideline added

**Number:** G{N}
**Name:** <name>
**Status:** proposed
**Addresses:** attribute N (and N)
**Evidence:** [file paths]
**One-line motivation:** <why now>
```

## Status transitions

When a guideline's status changes, that is also a foundation/methodology event and should be logged. Specifically:

- `proposed → testing`: log when active trial begins, and what data is being collected.
- `testing → adopted`: log the supporting evidence (link to experiment files in `evidence/experiments/`).
- `testing → retired` or `adopted → retired`: log the contradicting evidence and write a short post-mortem.

## Reminders

- A guideline that addresses a `temporary` attribute (one likely to be solved by AI capability improvements) should be flagged as such — its useful life may be short.
- A guideline whose evidence is one anecdote stays at `proposed` indefinitely until either (a) more evidence accumulates or (b) a structured trial promotes it to `testing`.
- The methodology earns its credibility by retiring guidelines that don't survive contact with reality. Don't be precious about removals.
- Each guideline should be small enough to evaluate. A guideline that says "do good research" is not a guideline.
