# methodology/

The prescription. This is where the methodology lives — practices the inquiry proposes, is testing, has adopted, or has retired. Unlike the foundation, the methodology is meant to grow over time. The first 15 guidelines were drafted alongside the foundation; the rest will arrive as evidence accumulates.

## Guiding principle

Every guideline in this directory is evaluable against one question: **does this practice grow the researcher's capacity to do the research job at the level it is actually judged on, or does it substitute for that capacity?**

The repo's central commitment ([`../GOAL.md`](../GOAL.md) §The commitment, substantiated in [`../foundation/00-why-reimagine.md`](../foundation/00-why-reimagine.md) §7: *empower, not replace*) is the methodology's working principle. The principle is applied at the level of the whole research job, not at every micro-task; routine operations AI can handle without invoking the test (syntax, formatting, mechanical conversions) are a different category. A guideline that produces fluent output *at the level the job is judged on*, without developing the researcher's capacity at that level, is not an improvement over the default — it *is* the default the methodology exists to push against.

Every guideline therefore has a `Skill implication` field that names what capacity the practice develops, preserves, or risks substituting. Guidelines that cannot articulate this are flagged and revisited, not added. The boundary between skills the methodology is comfortable seeing replaced and skills it insists on preserving moves upward as AI improves; guidelines are reviewed periodically against that drift.

## Files

- **`guidelines.md`** — accumulated practices, each with status (`proposed`, `testing`, `adopted`, `retired`), addressed attribute(s), evidence trail, skill implication, practice description, success criteria, costs, and notes.

That is the directory's content right now. As the methodology matures, more files will arrive — longer-form sections covering specific phases of research, worked examples, prompts, templates. None of those exist yet because none of them have earned their place.

## Guidelines vs the log

The repo separates two things that often get conflated:

- **`methodology/guidelines.md`** is **cumulative and normative**. Read this for "what should I do."
- **`../log/`** is **chronological and descriptive**. Read this for "how did we get here."

Every guideline links to the log entries that produced it; every log entry that motivates a guideline links to it. A guideline does not get drafted directly from a thought — it gets drafted from log entries (and foundation claims) that have earned it, via the `add-guideline` skill.

## Status lifecycle of guidelines

- `proposed` — written down, not yet tested. Default state for any new guideline. Most of the current set is at this status because the inquiry has not yet collected its own evidence.
- `testing` — actively being tried, with data being collected (a self-experiment, structured trial in the pilot project, etc.).
- `adopted` — evidence supports it; this is part of the live methodology.
- `retired` — evidence contradicted it, or it was superseded. Stays in the file with a post-mortem so the reasoning is preserved.

Use the [`add-guideline`](../.claude/skills/add-guideline/SKILL.md) skill to add new ones. Use [`update-foundation`](../.claude/skills/update-foundation/SKILL.md) for changes to the foundation that *motivate* changes to guidelines.

## Why the methodology will never be finished

AI is changing. What works changes with it. A methodology that treats "under construction" as a phase ending in some future v1.0 will be wrong by the time v1.0 ships. The expectation is permanent revision: guidelines added, retired, refined; the rate slows but does not stop. The first imperfect version is more useful than the perfect-but-future one.
