# AI-native research

A public, evolving inquiry into how research should be done when AI is treated as a first-class collaborator. The repo is a record of an inquiry, not a framework.

The diagnosis — what about AI forces research workflows to change — is settled enough to write down. The methodology is being grown from evidence over time, with explicit status on every guideline. The repo will keep changing as AI changes and as evidence accumulates.

If you are a researcher who has already adopted AI in some form, and you are wondering whether the way you are doing it is the way you should be doing it, this is for you.

## The inquiry's central claim

AI is the first tool in the history of knowledge work that can produce useful output without requiring the user to develop any reciprocal skill. Calculators changed arithmetic into calculator-literacy. Compilers changed assembly programming into higher-language fluency. GPS changed dead-reckoning into route-planning. AI breaks the pattern: a researcher can produce fluent output indefinitely without growing.

This makes the standard reassurance about technology and skills — *the worker is still skilled, just at different things* — fail specifically for AI. The methodology this repo is building responds to that with one principle: **empower, not replace.** AI should be used in ways that grow the researcher, not substitute for them. The full argument is in [`foundation/00-why-reimagine.md`](foundation/00-why-reimagine.md).

## What's here

- **[foundation/](foundation/)** — the diagnosis. Four documents covering the central argument (which includes the recombination-vs-innovation distinction in §3), the catalog of AI attributes (17 in 5 clusters, each tagged structural / temporary / ambiguous), the implications gestures, and open questions. Read [`foundation/00-why-reimagine.md`](foundation/00-why-reimagine.md) first. The deeper literature synthesis on innovation that backs the foundation lives in [`evidence/literature-notes/innovation-as-different-operation.md`](evidence/literature-notes/innovation-as-different-operation.md).
- **[methodology/](methodology/)** — the prescription. [`methodology/guidelines.md`](methodology/guidelines.md) currently has 15 initial guidelines, all at status `proposed`, each tied to an attribute, an evidence trail, and an explicit skill implication.
- **[evidence/](evidence/)** — interviews, structured experiments, working-session observations, and an annotated reading list. The substrate the foundation and methodology rest on.
- **[log/](log/)** — the chronicle. What happened in the inquiry, when, why something changed.
- **[case-studies/](case-studies/)** — empty for now. The maintainer's pilot research project will live here once a domain is chosen.

## Read first

If you have ten minutes: [`foundation/00-why-reimagine.md`](foundation/00-why-reimagine.md). The full argument in compact form.

If you have thirty minutes: `00`, then skim [`01-ai-attributes.md`](foundation/01-ai-attributes.md) for the detailed attribute catalog, then [`methodology/guidelines.md`](methodology/guidelines.md) for the initial guidelines.

If you want the full picture: read `foundation/` in order (`00` → `03`), then [the innovation literature note](evidence/literature-notes/innovation-as-different-operation.md), then the methodology, then the [reading list](evidence/reading-list.md).

## What this is not

- Not a framework. The methodology is grown from evidence over time, not asserted upfront. Guidelines have explicit status and can be retired.
- Not a way to do research faster while letting AI do more of it. The explicit goal is to use AI in ways that grow the researcher; faster-but-hollowing is the failure mode this repo exists to push against.
- Not a recipe for autonomous research. The reimagining is about the human's workflow.
- Not a competitor to system-level efforts (FutureHouse, DeepMind co-scientist, PSI / GPD, Sakana). It operates at a different layer — the practice of an individual or small-group researcher using best-in-class tools well.
- Not finished. Expect things to be revised, retired, or rewritten. The methodology is permanently under construction.

## Status

Foundation v1 as of 2026-05-06. The five foundation documents and the initial 15 guidelines are in place. Evidence collection beyond the initial reading list has not yet begun. The pilot research domain has not yet been chosen.

## How this repo works

Four skills under [`.claude/skills/`](.claude/skills/) maintain the repo as it grows:

- **`add-evidence`** — record a new interview, experiment, observation, or noteworthy reading.
- **`update-foundation`** — revise a foundation document based on evidence, with traceability.
- **`add-guideline`** — promote a practice from "the foundation suggests this" to "the methodology proposes trying this."
- **`inquiry-status`** — quick read of where the inquiry stands.

The discipline is foundation-first, evidence-driven, observational tone, and *empower over replace* — every claim and every practice traces to something concrete, and every practice articulates the skill it develops in the researcher. See [CLAUDE.md](CLAUDE.md) for full operating principles.

## Following along, contributing

The repo is **not currently accepting external contributions**. See [CONTRIBUTING.md](CONTRIBUTING.md) for the read-only / collaboration policy. If you are working on related problems and want to discuss a collaboration, email **masuryg@post.bgu.ac.il**. Useful kinds of outreach are described in CONTRIBUTING.

If you want to follow along, watch or star the repo. Updates are recorded in [log/](log/).

## License

MIT. See [LICENSE](LICENSE).

## Citing

If the framing or a specific document is useful in your work, citation is welcome. See [CITATION.cff](CITATION.cff).
