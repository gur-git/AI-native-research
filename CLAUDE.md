# CLAUDE.md

Operating principles for any AI assistant (or person) working in this repo. Read this before doing anything else here.

## What this repo is

A public, evolving inquiry into AI-native research methodology. The diagnosis (what about AI forces research workflows to change) is settled enough to write down. The prescription (the methodology itself) is deliberately under construction, and is meant to be built up from evidence over time — interviews, structured self-experiments, observations of real working sessions, and the maintainer's own pilot research project.

The repo is not a framework. It is a record of an inquiry, in the open.

The repo's charter — the compressed why and how, the commitments everything else aligns to — is in [`GOAL.md`](GOAL.md). The operating guidance in this file serves the charter. When they appear to conflict, the charter is authoritative and this file should be reconciled to it.

## Discipline

Four commitments shape how work in this repo should be done.

**Foundation-first.** Don't add to the methodology before the foundation supports it. If a guideline doesn't trace to an attribute and a piece of evidence, it doesn't go in.

**Evidence-driven.** Every claim in `foundation/` and `methodology/` should be traceable to something in `evidence/` or to a cited source. Untraceable claims are debt; flag them rather than letting them accumulate.

**Honest tone.** Observational, not promotional. The reader is a working researcher who can sense when something is overclaimed. Note things matter-of-factly. Distinguish what is known from what is suspected from what is speculation.

**Empower over replace.** The methodology's central principle (`GOAL.md` §The commitment, substantiated in `foundation/00-why-reimagine.md` §7). Tools and practices proposed in this repo should grow the researcher's capacity to do the research job at the level it is actually judged on, not substitute for that capacity. Every guideline must articulate the skill it develops, preserves, or risks substituting; guidelines that cannot are not added. Lower-level skills the researcher is comfortable letting AI handle (routine syntax, formatting, mechanical operations) are a different category — the principle is judged at the whole-job level. When AI is used to do work in this repo, the same standard applies at the same frame: the work should leave the maintainer more capable at the research job, not less.

## Structure

```
foundation/    — the diagnosis. why research must be reimagined; what about AI forces this.
methodology/   — the prescription. starts mostly empty; grows as evidence accumulates.
evidence/      — the substrate. interviews, experiments, observations, reading.
log/           — the chronicle. what happened in the inquiry, when, and why.
case-studies/  — the pilot. real research projects this methodology gets applied to.
```

`foundation/` and `methodology/` are normative (claims about what is and what to do).
`evidence/` and `log/` are descriptive (records of what was observed and what happened).

The repo's intellectual honesty depends on the descriptive side feeding the normative side, in that direction, with a paper trail.

## Skills

Four skills under `.claude/skills/` cover the core maintenance workflow. Use them rather than doing these operations ad-hoc.

- `add-evidence` — when a new interview, experiment, observation, or noteworthy paper has come in.
- `update-foundation` — when new evidence refines, contradicts, or extends a foundation claim.
- `add-guideline` — when an attribute plus accumulated evidence suggests a methodological practice worth trying.
- `inquiry-status` — quick read of where the inquiry stands.

Each skill, when invoked, also writes to `log/` so the chronicle stays current.

## Things not to do

- Don't write methodology guidelines that aren't supported by at least one attribute and one piece of evidence.
- Don't add foundation claims without a citation or a clearly-marked "speculative" tag.
- Don't promote — describe. Avoid words like "revolutionary," "powerful," "game-changing."
- Don't claim AI capabilities the repo hasn't verified. Cite the source. If the source is the maintainer's own observation, log it as such.
- Don't push to git remotes unless explicitly asked.
- Don't bundle unrelated changes into a single commit. Commits should track conceptual moves.

## Tone reference

When in doubt about tone, the standard is: **the kind of writing a careful researcher uses in a methods section.** Not the introduction. Not the discussion. The methods section. Specific, neutral, source-cited, comfortable with caveats.

## Status

Foundation v1 as of 2026-05-06. Five foundation documents (`00`–`04`) cover diagnosis, attributes catalog, innovation deep-dive, implications, and open questions. The methodology has 15 initial guidelines, all at status `proposed`, drawn from the foundation. Evidence collection beyond the initial reading list has not yet begun.
