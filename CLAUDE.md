# CLAUDE.md

Operating principles for any AI assistant (or person) working in this repo. Read this before doing anything else here.

## What this repo is

A public, evolving inquiry into AI-native research methodology. The diagnosis (what about AI forces research workflows to change) is settled enough to write down. The prescription (the methodology itself) is deliberately under construction, and is meant to be built up from evidence over time — interviews, structured self-experiments, observations of real working sessions, and the maintainer's own pilot research project.

The repo is not a framework. It is a record of an inquiry, in the open.

It is also, increasingly, meant to be *used*, not only read. The aim is that a working researcher could pick the repo up — and share it with peers — to run their own research in an AI-native way, eventually with no guidance but the repo itself. That gives everything here two first-class readers: the researcher, and the researcher's AI agent. Readability for the first and clean, loadable structure for the second are design priorities, not afterthoughts. This does not make the repo the kind of framework the inquiry rejects — the tools it ships encode current, revisable understanding, not a finished method — and *how* the methodology reaches a researcher and changes their practice (the interface itself) is treated as one of the inquiry's open research questions, not a settled mechanism.

The repo's charter — the compressed why and how, the commitments everything else aligns to — is in [`GOAL.md`](GOAL.md). The operating guidance in this file serves the charter. When they appear to conflict, the charter is authoritative and this file should be reconciled to it.

## Discipline

Four commitments shape how work in this repo should be done.

**Foundation-first.** Don't add to the methodology before the foundation supports it. If a guideline doesn't trace to an attribute and a piece of evidence, it doesn't go in.

**Evidence-driven.** Every claim in `foundation/` and `methodology/` should be traceable to something in `evidence/` or to a cited source. Untraceable claims are debt; flag them rather than letting them accumulate.

**Honest tone.** Observational, not promotional. The reader is a working researcher who can sense when something is overclaimed. Note things matter-of-factly. Distinguish what is known from what is suspected from what is speculation.

**Empower over replace.** The methodology's central principle (`GOAL.md` §The commitment, substantiated in `foundation/00-why-reimagine.md` §7). Tools and practices proposed in this repo should grow the researcher's capacity to do the research job at the level it is actually judged on, not substitute for that capacity. Every guideline must articulate the skill it develops, preserves, or risks substituting; guidelines that cannot are not added. Lower-level skills the researcher is comfortable letting AI handle (routine syntax, formatting, mechanical operations) are a different category — the principle is judged at the whole-job level. When AI is used to do work in this repo, the same standard applies at the same frame: the work should leave the maintainer more capable at the research job, not less.

## Building for researchers

The repo's deliverable for a researcher is **tools and guides, not research**. Work done here builds the methodology and the general, user-facing means by which a researcher (and their AI agent) can do their own research — it does not do any specific researcher's domain research for them. That is empower-not-replace applied to the user. When the inquiry has a pilot, the research itself lives in the researcher's own, separate, possibly private repo and stays theirs; this repo contributes the scaffolding, the operating guidance their agent runs on, and the channel to feed their experience back.

Three constraints follow:

- **General and shareable by default.** Build for a stranger online with no guide but the repo, not for one researcher or one domain. Specific adaptations come later, and only when a general version genuinely cannot serve.
- **Near-zero cost, researcher independence first.** The cooperation should cost the researcher as close to nothing as possible. Push the methodology to them, then let them work freely; it should empower the work, never hold it back.
- **The interface is under study.** What form of contact actually helps — what a researcher reads, what their agent runs on, what feeds back — is itself a research question the pilot is meant to answer. Prototype the lightest version and learn from it; do not fix it by fiat.

## Coherence and revision

Every addition is judged against the whole, not only on its own merits. New material — and new evidence when it arrives — must leave the repo's story coherent: a tool, guideline, or claim that contradicts another is a defect to reconcile, not a parallel truth to file beside it. Two practices keep that affordable:

- **One source, many views.** Don't restate a claim in several places. A tool or guide should be a *view on* the foundation and methodology, deriving from them, so that when understanding shifts the source changes once and the views follow — instead of copies drifting apart.
- **Mark the evidence level; stay revisable.** Much of what is written now rests on reading rather than the repo's own evidence. That is acceptable for now, provided it is marked as such (the `grounded` / `inferred` / `speculative` tagging used in `methodology/ai-native-research-process.md` is the model). When the pilot returns experience, the repo adapts to it; revision is expected, not a failure.

## Structure

```
foundation/    — the diagnosis. why research must be reimagined; what about AI forces this.
methodology/   — the prescription. starts mostly empty; grows as evidence accumulates.
evidence/      — the substrate. interviews, experiments, observations, reading.
log/           — the chronicle. what happened in the inquiry, when, and why.
case-studies/  — the pilot. the record of real research the methodology is applied to, and what is learned from it.
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
- Don't do a specific researcher's domain research from this repo. Build the general tool or guide that lets them — and their agent — do it themselves.
- Don't restate a claim across files. Derive tools and guides from the foundation and methodology so the story keeps one source of truth.
- Don't build researcher- or domain-specific tooling where a general, shareable version would serve.

## Tone reference

When in doubt about tone, the standard is: **the kind of writing a careful researcher uses in a methods section.** Not the introduction. Not the discussion. The methods section. Specific, neutral, source-cited, comfortable with caveats.

## Status

Foundation v1 as of 2026-05-06: five documents (`00`–`04`) covering diagnosis, attributes catalog, innovation deep-dive, implications, and open questions. The methodology has 19 guidelines, all at status `proposed`, plus a speculative `v0` synthesis of the end-to-end process ([`methodology/ai-native-research-process.md`](methodology/ai-native-research-process.md)) — explicitly a hypothesis to test, not evidence-backed guidance. Evidence collection has begun beyond the reading list: a self-study stream ([`evidence/self-study/`](evidence/self-study/)), a lab survey ([`evidence/lab-surveys/`](evidence/lab-surveys/), awaiting data), and the pilot phase's first interview and observation entries (2026-06-10).

The repo is in its first user-facing phase. Its first pilot — and first user — is a real research project (the maintainer's own; documented in [`case-studies/snn-research/`](case-studies/snn-research/)), against which the methodology is applied and from which the repo learns through two standing channels: background audits of the pilot's public workspace, and conversations with the pilot team and with their supervising professor about how research is classically conducted. The first pilot-phase evidence produced guidelines G16–G19 (an explain-back knowledge gate, a five-part research proposition, an MVP-first execution posture, and early parallel expert review — classical practices adapted AI-natively, not copied). No guideline status has changed on the strength of the pilot yet; that waits for its evidence.
