---
name: inquiry-status
description: Produce a quick read of where the inquiry stands — recent log entries, recently added evidence, guidelines by status, and outstanding open questions. Use when starting a session, before adding evidence or revising the foundation, or when sharing the repo's current state.
---

# inquiry-status

Compile the current state of the inquiry into a short, structured report. The point is to re-ground a returning collaborator (or yourself, weeks later) on where things actually stand without having to read the whole repo.

## When to invoke

- Starting a working session in the repo after time away.
- Before invoking `update-foundation` or `add-guideline`, to make sure the change you're considering is consistent with recent work.
- When the maintainer wants to share the repo's state with someone (e.g., before a conversation at a conference).
- Periodically as a checkpoint, to notice drift.

## Procedure

1. **Read recent log entries.** List the last 5 entries from `log/`, by filename (which is dated). For each, give a one-line summary of what shifted.

2. **Read recently added evidence.** List the last 5 entries across `evidence/interviews/`, `evidence/experiments/`, `evidence/observations/`. For each, give: type, date, source, the headline claim, confidence label.

3. **Tally registry practices by status.** Read the registry in `METHODOLOGY.md` §7 and count practices in each status: `proposed`, `testing`, `adopted`, `retired`. List the names of practices in `testing` (these are the active trials).

4. **Confront the open questions.** Read `foundation/03-open-questions.md`, then grep `evidence/` for `related_questions` references and Q-number mentions. For each open question report: a one-line summary, and what evidence (if any) has accumulated against it since it was opened. For any question where the accumulated evidence looks like it answers, narrows, or contradicts the question — say so and offer the open/close move explicitly (the maintainer decides; `update-foundation` executes).

5. **Surface stale items.** Note:
   - Practices in `proposed` for more than 90 days with no evidence added → these may be aspirational.
   - Foundation attributes whose last revision date is older than the relevant evidence dates → may need an `update-foundation` pass.
   - Open questions with no evidence touching them for 180+ days → consider whether they're still the right questions.

## Output format

Print a single markdown report:

```markdown
# Inquiry status — YYYY-MM-DD

## Recent log entries

- YYYY-MM-DD — <topic>: <one-line summary>
- ...

## Recently added evidence

- YYYY-MM-DD [interview] <source> — <headline claim> (confidence: X)
- ...

## Practice registry

- Proposed: N
- Testing: N (<names>)
- Adopted: N
- Retired: N

## Open questions (with evidence accumulated)

- Q1: <one-line summary> — <evidence touching it, or "none since opened">
- ...

## Stale items (action suggested)

- ...
```

Keep it terse. The report should be readable in under a minute.

## Reminders

- This skill does not change anything. It only reads and summarizes.
- If the report surfaces a stale item, do not act on it within `inquiry-status`. Note it in the report; the maintainer can choose to invoke `update-foundation` or `add-guideline` as a separate, deliberate step.
- If a directory or file referenced above doesn't exist yet (early-state repo), say so explicitly. "0 entries" is a valid and useful signal.
