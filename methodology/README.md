# methodology/

The prescription. This is where the methodology lives — but in this repo, the methodology is **deliberately under construction**. Most of the file space here is empty by design.

## Why empty

A methodology built before the foundation is settled, and before evidence has been collected, is opinion in formal clothing. The point of this repo is to grow a methodology that can stand on what it claims, by accumulating evidence first and prescribing second.

So this directory contains:

- **`guidelines.md`** — accumulated practices, each tagged with a status (`proposed`, `testing`, `adopted`, `retired`) and traced to the foundation attribute(s) and evidence that motivated it.

That's it for now. As the methodology matures, more files will arrive: longer-form sections covering specific phases of research, worked examples, prompts, templates. None of those exist yet because none of them have earned their place.

## Guidelines vs the log

The repo separates two things that often get conflated:

- **`methodology/guidelines.md`** is **cumulative and normative**. It states the current best practices the inquiry has converged on, with explicit status. Read this for "what should I do."
- **`log/`** is **chronological and descriptive**. It records what happened in the inquiry, when, and why. Read this for "how did we get here."

A guideline is the *position*; the log is the *story*. Every guideline links to the log entries that produced it; every log entry that motivates a guideline links to it.

If you find yourself wanting to write something that is part-position-part-story, it goes in the log first as a description, and a `proposed` guideline gets drafted from it separately.

## Status lifecycle of guidelines

- `proposed` — written down, not yet tested. Default state for any new guideline.
- `testing` — actively being tried, with data being collected (a self-experiment, a structured trial in the pilot project, etc.).
- `adopted` — evidence supports it; this is part of the live methodology.
- `retired` — evidence contradicted it, or it was superseded. Stays in the file with a post-mortem so the reasoning is preserved.

Use the `add-guideline` skill to add new ones. Use `update-foundation` for changes to the foundation that *motivate* changes to guidelines.
