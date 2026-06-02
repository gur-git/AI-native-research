# AI-native research workspace — handoff (v0, provisional)

## What this is

A single self-contained file you drop into a fresh, empty repo and hand to your AI coding agent (e.g. Claude Code). The agent reads it and scaffolds a research workspace: a thin operating `CLAUDE.md`, a version-controlled project-state file, two thin ledgers, a short intake you fill, and a friction log. You then fill the intake and do your own research in that workspace. The agent never does the research.

It is general and domain-agnostic — no field, method, or toolchain is assumed. It encodes a small set of operative disciplines and the structure to run them; it does not contain or produce any research.

It derives from a source methodology repo (the "AI-native research" inquiry). This file is a *view* on that work, kept deliberately thin so it can be picked up cold. For the reasoning and evidence behind each discipline, see the source repo (pinned in `CLAUDE.md`). This file is usable standalone; the pointer is for depth, not dependency.

**Status: v0, provisional.** This is the lightest prototype that carries the disciplines, not a finished system. The disciplines themselves are `proposed` upstream — hypotheses under test, not validated results — and the right *form* of this scaffold is itself an open question. Keep what helps; if a piece isn't earning its place in your work, drop it and note why in the friction log. Send friction back to the source repo — that is how the methodology revises.

## How to use it

1. Put this file in a fresh repo. Hand the repo to your agent and tell it to follow the **Scaffolding instructions** below.
2. Fill in `INTAKE.md` (the agent creates the template; only you can answer it).
3. Start your research. Re-load `state.md` into each new agent session; update it at the start and end of each session.

## The operative principle

The controlling question, asked at the level of the whole job — not every keystroke:

> Will my capacity to do the research job, at the level it is judged on, be greater because of how I use AI here, or smaller?

Routine work below where research value is created — syntax, formatting, conversions, mechanical edits — is fine to delegate. The line is crossed only when AI's output would *be* the substantive contribution. The line moves as AI improves; the principle doesn't.

## The operative disciplines

These disciplines operationalize the principle. Each is one mechanism: the agent enforces structure, **you** supply judgment. They are `proposed` upstream — try them, don't trust them. They are stated once here, in full; the scaffolded `CLAUDE.md` carries a compact checklist that points back here, rather than restating them.

1. **External, version-controlled project state.** A single `state.md` is the source of truth across sessions — not chat history. You own it; the agent reads it to re-ground at session start and may *propose* edits, but never decides what gets logged.
2. **Independent-source verification.** Before you build on any AI output, name a verification mode whose source is independent of the generator: a formal check, your own critical reading with the primary source open, or — periodically — replicating a recent result from different ground, which depends on nothing the generator produced. Treat AI-produced literature as a starting graph: source-walk each cited claim and mark it green / yellow / red. Yellow and red do not become foundation without re-derivation.
3. **Attack before you adopt.** Before committing to a design or a finding, ask AI the adversarial form, not the confirming one: *what would falsify this? what control is missing? what would a hostile reviewer say?* Use AI to attack the work, not to validate it. The cheap version of this run at design time saves the expensive version at review time.
4. **Rank before AI ranks.** When the agent produces a candidate set (hypotheses, designs, framings), read the candidates without AI commentary and rank them yourself with a one-line rationale each, *then* ask AI to rank, then reconcile divergences deliberately. Test: could you defend your ranking without AI in six months?
5. **Classify the task before delegating.** Before any non-trivial task, name it: *recombination* (assembling known elements — AI as a parallel engine, verification dominant) or *innovation* (out-of-distribution moves — AI maps the terrain, you make the move). When in doubt, treat it as innovation. This is the meta-checkpoint: it decides how much of the rest applies.
6. **Keep navigation yours.** Use AI as a terrain-map, not as the agent that chooses the route. It can lay out the options, costs, and adjacencies; *which way to go* is the call the job is judged on. Outsourcing direction is the most consequential form of replacement — when you catch yourself asking AI "what should I do next," stop and answer it yourself first.
7. **Protect exploration share.** AI makes exploiting a known vein cheap, which pulls steadily toward more exploitation and less exploration. Hold a deliberate share of effort for exploratory moves and check it periodically; if everything you've done lately is refinement of one thread, that is the gradient at work, not a finding.
8. **Thin retrospective ledgers** (two, minutes each, written by you, never the agent). *Calibration:* expected vs. actual time, AI-assisted or not, felt vs. measured help (review when an entry surprises you). *Judgment:* what you chose and rejected and why, what later came of it; what you delegated that you might be losing; what was hard a month ago and is now easy (revisit on a low-frequency cadence you set — monthly is a reasonable starting point).
9. **Pause at the substantive moments.** At phase transitions (not every prompt), ask the controlling question. The honest answer is usually "yes if I do X, no if I just accept it" — note the X. Sharper test: which apprenticeship am I declining here, and can I name and accept that trade?

Keep the disciplines light. They are heaviest exactly where least needed; let the mechanical parts (provenance, re-grounding) lighten as tooling absorbs them, without weakening the core: selection, verification, navigation, and the empower/replace line.

## Scaffolding instructions (for the agent)

Create the files below in the repo root. Use the contents given. Keep every file minimal; do not pad and do not add files not listed here unless the researcher asks. Where a template has fields, leave them blank — do not fill them. After scaffolding, print a short summary of what you created and stop — **do not begin any research work.**

### Files to create

```
CLAUDE.md           # thin operating guidance for this repo (created below)
INTAKE.md           # researcher fills this first; agent leaves fields blank
state.md            # external project state — the source of truth, not chat history
FRICTION.md         # feedback channel back to the methodology
ledgers/
  calibration.md
  judgment.md
```

Do not create directories for the researcher's own notes or outputs — their working layout is theirs to choose. Do not initialize git unless the researcher asks; do not add files beyond those listed.

### 1. `CLAUDE.md` (thin — a pointer, not a copy)

Write a short operating file containing, in this order, kept to roughly one screen:

- One line on what this repo is: *this researcher's own research project, run with an AI agent under the empower-not-replace discipline.*
- The controlling question (verbatim from *The operative principle* above) and the one-line carve-out that routine low-level work is fine to delegate.
- The nine disciplines as a compact checklist, **one line each** — titles plus the bare mechanism. Do not expand into an essay; note that they are `proposed`, and for depth point to the handoff file's *operative disciplines* section and to the source repo at the pinned commit (below).
- A **session ritual** the agent runs every session, stated as two steps: *At session start — load `state.md` and re-ground in the current question, constraints, and open threads before doing anything else. At session end — update `state.md` (or propose the update for the human to commit).* Add the high-frequency note: re-ground against `state.md` whenever the thread drifts, not only at the boundaries.
- A line stating that the human — not the agent — updates `state.md` and the ledgers (the agent may propose, never commit).
- The **source pin**, as three lines: `source_repo:`, `pinned_commit:`, `scaffolded_on:`. The researcher provides the repo URL and commit; leave `TODO` markers if you do not have them — do not invent them. Add one line: *disciplines are status `proposed` upstream; re-pin deliberately when adopting upstream changes.*
- The **AI-provenance convention**, one line: *for any relied-on AI output, record model + version, prompt, non-default parameters, and date — in the artifact's commit message (default) or a sibling `<artifact>.aimeta.md`. Expect this to lighten as tooling absorbs it.*
- The **DO NOT** block (copy from *DO NOT* below, verbatim).

Do not reproduce the source methodology's full process document here. If this file grows past about one screen, it is too long.

### 2. `state.md` (external project state)

Create with these headers and a one-line placeholder under each:

```
# Project state
_Loaded at the start of every session as the source of truth — not chat history.
The human updates this at session start and end. The agent reads it to re-ground
and may propose edits; it does not decide what goes in._

## Current question
## Constraints and assumptions
## Decided directions
## Dead ends (and why)
## Open threads
## Last updated
```

### 3. `INTAKE.md` (the researcher fills this; agent leaves fields blank)

```
# Intake
_Fill this in before starting. This is yours; the agent does not answer it for you._

## 1. Research question
What are you actually trying to find out? (One or two sentences.)

## 2. What would convincingly verify an answer
What evidence or check would make you — and a skeptical reader — believe an answer
is right? Name the independent source of that verification.

## 3. Empower / replace map
- **Protect** (the skills the job is judged on — keep these yours; AI may assist, not produce):
- **Delegate** (routine work below where research value is created — fine to hand to AI):
- **Watch** (uncertain which side of the line, or tasks that interleave routine and original moves — revisit):

## 4. Skill baseline (t=0)
Name the capacities the work is judged on and where you stand on each today. This is
the reference point the capability entries in your judgment ledger measure drift against.

## 5. Default task-classification
Your honest current habit: which kinds of task do you reach for AI on, and which do
you keep by hand? (Recombination vs. innovation — discipline 5. This is the meta-check
you'll recalibrate as you go.)
```

### 4. `ledgers/` (two thin ledgers; agent creates headers only, never authors entries)

Create each with a one-line purpose and a column header row. The agent must not fill these in.

`ledgers/calibration.md`:
```
# Calibration ledger — felt help vs. measured help (~minutes per entry)
| date | task | AI-assisted? | expected time | actual time | felt help vs. measured |
|------|------|-------------|---------------|-------------|------------------------|
```

`ledgers/judgment.md`:
```
# Judgment ledger — direction, drift, and replication (revisit ~monthly, a starting cadence)
| date | direction chosen / rejected (+ why) | later: what came of it | delegated — might be losing | was hard a month ago, now easy | replicated lately? |
|------|--------------------------------------|------------------------|-----------------------------|--------------------------------|--------------------|
```

### 5. `FRICTION.md` (feedback channel back to the methodology)

```
# Friction log
_What in this scaffold helped, chafed, was ignored, or felt like ceremony with no
payoff. The form of this scaffold is itself under study, so this is the primary
evidence the source methodology wants back._

## How this returns
Skim this log on a regular cadence (a reasonable default: monthly, and at the end of
the project). Carry anything worth saying back to the source repo as an issue — or a
pull request if you can name the fix. A link to this log is enough; raw entries are fine.

## Entries
<!-- date | discipline (1–9) or file | what happened | helped / chafed / ignored -->
```

## DO NOT (for the agent)

- **Do not do the researcher's domain research.** Do not propose research questions, hypotheses, directions, methods, or findings; do not fill `INTAKE.md`, `state.md`, or any ledger with substantive content; do not rank candidates before the researcher has; do not answer "which way next" for them (discipline 6). Your job is to build and maintain the workspace and to run inside the disciplines above — not to supply the substantive contribution. If a request would have you produce the substantive contribution, surface the controlling question and hand the decision back.
- Do not decide what gets logged in `state.md` or the ledgers — that is the human's call (you may propose, never commit).
- Do not expand `CLAUDE.md` into a copy of the source methodology; keep it a thin operating file with a pointer.
- Do not add structure beyond what is listed here. If something seems missing, note it in `FRICTION.md` rather than building it.
- Do not invent the source repo URL or commit SHA; leave TODO markers if you do not have them.

## A note on v0

This is the lightest viable version, marked provisional on purpose. The goal is that after a project run with it you are *more* able to do the research job — frame questions, design verification, hold direction, judge results — not less, even though AI did a lot of the work along the way. Use it, strip what doesn't earn its place, and log the friction. The methodology improves from real use — yours included.