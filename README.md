# AI-native research

A public, evolving inquiry into how research should be done when AI is treated as a first-class collaborator.

The repo is a record of an inquiry, not a framework. The diagnosis — what about AI forces research workflows to change — is settled enough to write down. The methodology is deliberately under construction, and is built up from evidence over time as the maintainer applies it to a real research project.

If you are a researcher curious about whether AI is reshaping your work in ways you have not fully reckoned with, this is meant for you to read along with.

## What's here

- **[foundation/](foundation/)** — the diagnosis. Two documents:
  - **[Why reimagine research](foundation/00-why-reimagine.md)** — what is happening to knowledge work generally, why research is a particular case, and why this inquiry exists.
  - **[AI attributes](foundation/01-ai-attributes.md)** — fifteen attributes of current AI systems, in four clusters, each tagged `structural` (likely permanent — design around it), `temporary` (likely solvable — do not over-commit), or `ambiguous`. Each attribute has a short description and a thorough explanation of why the tag is right.
- **[methodology/](methodology/)** — mostly empty by design. Practices accumulate here only when they have earned it, in `methodology/guidelines.md`, with status (`proposed` / `testing` / `adopted` / `retired`) and links back to the evidence that motivated them.
- **[evidence/](evidence/)** — interviews, structured experiments, working-session observations, and an annotated reading list. The substrate the foundation and methodology rest on.
- **[log/](log/)** — the chronicle. What happened in the inquiry, when, why something changed.
- **[case-studies/](case-studies/)** — empty for now. The maintainer's pilot research project will live here once a domain is chosen.

## Read first

If you have ten minutes, read **[foundation/00-why-reimagine.md](foundation/00-why-reimagine.md)** and skim **[foundation/01-ai-attributes.md](foundation/01-ai-attributes.md)**. Those two documents are the inquiry's current position.

If you want the shorter version: AI is not just a faster tool for existing research workflows — it shifts the cost structure in ways that force reorganization. Production (drafting, summarizing, exploring) has become cheap. Judgment, verification, and selection have become the binding constraints. A research methodology that does not promote those operations to first-class is producing more output of less-verified quality.

## What this is not

- Not a framework. The methodology is grown from evidence over time, not asserted upfront.
- Not a recipe for autonomous research. The reimagining is about the human's workflow, not about AI agents replacing the human.
- Not a competitor to system-level efforts (FutureHouse, DeepMind co-scientist, PSI / GPD, Sakana). It operates at a different layer — the practice of an individual or small-group researcher using best-in-class tools well.
- Not finished. Expect things to be revised, retired, or rewritten. Expect tags on attributes to move as the technology evolves.

## Status

Foundation v0 — written 2026-05-05. The two foundation documents are in place. The methodology is empty by design. Evidence collection beyond the initial reading list has not yet begun. The pilot research domain has not yet been chosen.

## How this repo works

Four skills under [`.claude/skills/`](.claude/skills/) maintain the repo as it grows:

- **`add-evidence`** — record a new interview, experiment, observation, or noteworthy reading.
- **`update-foundation`** — revise a foundation document based on evidence, with a traceability trail.
- **`add-guideline`** — promote a practice from "the foundation suggests this" to "the methodology proposes trying this."
- **`inquiry-status`** — quick read of where the inquiry stands.

The discipline is foundation-first and evidence-driven: every claim in `foundation/` traces to a citation; every guideline in `methodology/` traces to evidence and to one or more attributes. See [CLAUDE.md](CLAUDE.md) for the full operating principles.

## Following along, contributing

The repo is **not currently accepting external contributions**. See [CONTRIBUTING.md](CONTRIBUTING.md) for the read-only / collaboration policy. If you are working on related problems and want to discuss a collaboration, email **masuryg@post.bgu.ac.il**. Useful kinds of outreach are described in CONTRIBUTING.

If you want to follow along, watch or star the repo. Updates are recorded in [log/](log/).

## License

MIT. See [LICENSE](LICENSE).

## Citing

If the framing or a specific document is useful in your work, citation is welcome. See [CITATION.cff](CITATION.cff).
