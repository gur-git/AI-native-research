# Shipped the first researcher-facing tool: HANDOFF.md (2026-06-02)

The repo took its first step as a *tool*, not only a record. `HANDOFF.md` is a general,
domain-agnostic file a researcher drops into a fresh repo and hands to their own AI agent,
which then scaffolds an AI-native research workspace. Built for the pilot's first user (the
maintainer) but written for a stranger with no guide but the file.

## What was added

- **`HANDOFF.md`** (repo root) — v0, provisional. Has the researcher's agent scaffold: a thin
  operating `CLAUDE.md` (the disciplines as a one-line checklist, the source pin, an AI-provenance
  convention, a session ritual, and a DO-NOT block), an external `state.md`, two thin ledgers
  (calibration; judgment), an `INTAKE.md` (question / what-would-verify / empower-replace map /
  t=0 skill baseline / task-classification), and a `FRICTION.md` feedback channel. The agent is
  explicitly barred from doing the domain research.
- **`README.md`** — added a "For researchers: using this repo to run your own research" section
  (the three-step use), and refreshed the `case-studies/` description and the Status block for
  coherence with the updated `GOAL.md` / `CLAUDE.md`.

## How it was built

A draft → critique → synthesize workflow (12 agents) scoped hard to *lightest-viable*. The
adversarial critics confirmed no research-doing (the central constraint), no promotional language,
and coherence with the foundation. The finalizer cut the over-built pieces the completeness critic
flagged (a standalone source-pin file, a third ledger, prescribed notes/artifacts directories) and
folded in the disciplines it had been missing (adversarial pre-mortem, exploration-share,
replication, keep-navigation-yours).

## The operative content

The handoff encodes nine disciplines — one mechanism each, the agent enforcing structure and the
human supplying judgment — all marked `proposed` upstream, presented as a *view* on the
foundation/guidelines/process draft rather than a copy (one source, many views).

## Still open

- The handoff is v0 and the interface is under study; the pilot's friction log is the primary
  evidence for revising it.
- Uncommitted: this sits alongside the `CLAUDE.md` / `GOAL.md` reconciliation edits, awaiting the
  maintainer's word to commit.
