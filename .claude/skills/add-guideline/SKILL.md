---
name: add-guideline
description: Add a practice to the registry in METHODOLOGY.md, or move an existing practice's status, based on accumulated evidence and one or more foundation attributes. Practices start as proposed, can move to testing, then adopted or retired. Use when evidence is strong enough to warrant trying a practice (or changing one's standing), not just describing a problem.
---

# add-guideline

Promote a practice from "thing the evidence suggests" to "thing the methodology proposes trying" — or move an existing practice through its lifecycle. The registry lives in [`METHODOLOGY.md`](../../../METHODOLOGY.md) §7; it is the methodology's revisable layer, and this skill is how it changes.

## When to invoke

- A foundation attribute (or cluster) has been stable for a while, and a practice that addresses it has emerged from evidence.
- Multiple pieces of evidence converge on the same recommended practice.
- Evidence justifies moving a practice's status (`proposed` → `testing` → `adopted`, or → `retired`).

Do not invoke to add aspirational practices. A practice must trace to evidence, not to what would be nice.

## The bar for a new entry

Every entry must have all three, or it does not go in:

1. **Attribute(s)** — which AI attribute(s) from `foundation/01-ai-attributes.md` it addresses, by number.
2. **Evidence** — which evidence files motivated it, linked.
3. **Skill implication** — what capacity the practice develops, preserves, or protects in the researcher. A practice that cannot articulate this risks substituting for skill, which the central principle cannot tolerate. If you genuinely cannot answer, do not add the practice; revisit the foundation instead.

## Entry format

Append a row to the registry table in `METHODOLOGY.md` §7:

```
| G{N} | **<Imperative name.>** <One-to-three-sentence practice statement, with the skill it protects evident.> (A{n}, A{n}) | proposed | New YYYY-MM-DD; evidence: <links>. |
```

Numbers are sequential and never reused, even after retirement. If the practice needs more explanation than a registry row carries, the explanation belongs in the relevant section of `METHODOLOGY.md` (§2–§6), with the row pointing at it — not in a parallel document.

## Status transitions

Each transition is logged, and statuses move only on evidence:

- `proposed` → `testing`: a deliberate trial is running; name what data is being collected and where.
- `testing` → `adopted`: link the supporting evidence.
- any → `retired`: keep the row, mark the status, and write a one-line post-mortem in the Disposition column linking the fuller reasoning in the log. The methodology earns its credibility by retiring practices that don't survive contact with reality.

## After writing

1. **Log entry** in `log/YYYY-MM-DD-{topic}.md`:

   ```markdown
   ## Registry change

   **Practice:** G{N} — <name>
   **Change:** added at proposed | status moved X → Y
   **Addresses:** attribute(s) N
   **Evidence:** [file paths]
   **One-line motivation:** <why now>
   ```

2. **If the change affects researcher-facing behavior** (what an agent in a workspace should do differently), draft an update document in `updates/` per its README conventions, and note that the starter needs a corresponding revision.

3. **Offer the open-questions move** if the change bears on one (per `CLAUDE.md` §Coherence and revision).

## Reminders

- A practice addressing a `temporary` attribute should be flagged as such — its useful life may be short.
- A practice whose evidence is one anecdote stays at `proposed` indefinitely until more evidence accumulates or a structured trial promotes it.
- Each practice should be small enough to evaluate. "Do good research" is not a practice.
