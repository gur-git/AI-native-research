# Update 0001 — The gate-carried posture, modes, and the starter workspace

```
date:            2026-06-10
applies_from:    any pin at or before fc00c47 (2026-06-02)
cut_at:          708ce62cf72b96029186ab67fe3b480f6fe916e8   # the inquiry commit this release was cut from
starter_version: 0.1.0
supersedes:      HANDOFF.md v0 and methodology/agent-operating-guide.md (both retired;
                 the methodology now lives in METHODOLOGY.md at the repo root)
```

*For the researcher's agent: walk these items with your researcher in conversation, one at a time. Each is theirs to adopt, skip, or adapt; record skips in `context/records/`. When done, re-pin to the commit you fetched this from.*

---

## 1 · The posture: junior colleague, gate-carried apprenticeship

**What changed.** The methodology no longer asks the researcher to author load-bearing content. The agent does the heavy lifting — including writing every document — and is never fully trusted; the researcher contributes through conversation, and the second output (the researcher's own development) is carried by **gates**: interview-conversations at closures and commitments. Authorship rules are retired (old discipline 5 / G5); decision ownership and independent verification are not relaxed. Full statement: `METHODOLOGY.md` §2–3.

**Why.** The pilot rejected the authoring posture within two days while keeping and validating the verification gate ([meeting](../evidence/interviews/2026-06-10-pilot-team-meeting.md), [audit](../evidence/observations/2026-06-10-pilot-workspace-audit.md)). The revision is a tracked bet (Q13).

**Ask your researcher.** "The methodology now officially works the way you chose to work — AI drafts, you own decisions and pass gates in conversation. Do you want me to reconcile the workspace's posture docs to this?" (For the pilot specifically: this resolves the deferred 'posture reconciliation' in `state.md`.)

**How to apply.** Update the workspace CLAUDE.md's methodology section: agent may author; gates close understanding/commitments; researcher-reserved decisions unchanged; hard lines now protect gates (no closure over unresolved gaps, no understanding without a gate, overrides recorded, no fabricated sources).

## 2 · Gates: interview protocol and closure rules

**What changed.** The verification gate (the pilot's `quiz` pattern) is now the general primitive, in interview form: questions the work needs, gaps treated as findings, artifacts fixed when the miss traces to them. The agent closes the gate when the conversation stops producing value, may vote to prolong, and the researcher may override — recorded in one line, never argued. Early-stage gates legitimately lean test-like (articulation *is* the goal there). `METHODOLOGY.md` §3, registry G20/G16.

**Ask your researcher.** "Keep your quiz flow as is, or adopt the closure rules (I close by default when value runs out; you can always override on record)?"

**How to apply.** The finished general form rides with this update: install [`0001-files/gate-SKILL.md`](0001-files/gate-SKILL.md) as `.claude/skills/gate/SKILL.md` (or merge its closure/override/record mechanics into your existing quiz skill, keeping your domain specifics). Log gate transcripts under `context/records/` (create it if absent).

## 3 · Named modes

**What changed.** Two named modes, introduced to the researcher and invocable by name: **work mode** (default) and **conversation mode** (read-only, short replies; automatic for gates, researcher-reserved decisions, and thinking-out-loud; explicit exit followed by a summary of what was concluded). `METHODOLOGY.md` §4, registry G21.

**Ask your researcher.** "Want me to announce and honor these two modes?"

**How to apply.** Add a modes section to the workspace CLAUDE.md.

## 4 · Workspace shape: cursor + store; ledgers retired

**What changed.** `state.md` slims to a cursor (where the work is *now*) pointing into a `context/` store (`profile.md`, `knowledge/`, `records/`). The two researcher-written ledgers are retired; their function moves to gate-generated records plus a periodic review conversation. Provenance is carried as inline authorship/status headers. `METHODOLOGY.md` §6.

**Why.** The ledgers got zero entries in a month of real use; the inline-header form is what was actually practiced ([audit](../evidence/observations/2026-06-10-pilot-workspace-audit.md)).

**Ask your researcher.** "Retire the empty ledgers and let the records + a periodic review conversation replace them?"

**How to apply.** Delete `ledgers/` (or archive), create `context/records/`, keep `state.md` lean with links into existing knowledge files.

## 5 · The starter and this channel

**What changed.** New researchers now start from a template workspace (the starter repo) rather than a HANDOFF file; existing workspaces don't migrate — they just consume updates from this directory (`updates/`, agent-addressed, per-item adoption) and keep `FRICTION/` (a folder now; agent-drafted entries, researcher notes welcome) as the upstream channel, read by the maintainers by arrangement.

**Ask your researcher.** "Nothing to adopt here unless you want the FRICTION file converted to the folder convention — shall I?"

**How to apply.** `FRICTION.md` → `FRICTION/` with dated entry files; note the `updates/` path next to the source pin.
