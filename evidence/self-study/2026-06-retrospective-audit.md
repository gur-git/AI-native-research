---
type: observation
source: this repository's own development history (git log, log/, structure) — maintainer's AI-native practice, n=1
date: 2026-06-01
confidence: weak (retrospective, n=1, self-observed; observable "was-it-practiced" cells are moderate, outcome cells are unfilled by design)
related_attributes: [2, 10, 11, 13, 16]
raw_material: this repo (git history through 4957ef7, 2026-05-17; log/ 11 entries)
---

# Retrospective audit — this repo against the 15 guidelines (first pass)

## What this is

A first pass of the self-study method: take an AI-native project whose artifacts are fully
observable, and score each methodology guideline by **whether the practice it describes was
actually followed** in that project — not whether it helped (that is a [maintainer] judgment), only
whether it was done, and what artifact shows it.

The subject here is **this repo itself**. It is an AI-native methodology inquiry, built with AI
assistance over ~2 weeks of active work (foundation 2026-05-05/06, methodology 2026-05-06,
literature survey + charter 2026-05-16/17). It is a *partial* subject: it exercises the guidelines
about state-keeping, literature work, and direction-choice well, but has no experiments,
replications, or hypothesis design yet, so several guidelines are simply **not-yet-applicable**
here and need one of the maintainer's actual research repos as their subject. Identifying *which*
guidelines need *which* subject is itself a deliverable of this pass.

**No guideline statuses are changed by this document.** It is descriptive evidence. Promotions
happen separately and deliberately via `add-guideline` / `update-foundation`, with the maintainer.

---

## The four buckets

### Bucket A — Practiced and sustained here → testing-candidates

These were genuinely followed in this repo; the evidence is on disk. They are the guidelines closest
to a defensible `proposed → testing` move — pending the maintainer's outcome judgment.

- **G2 — Maintain external project state in version-controlled files.** *Practiced: strongly.*
  Artifacts: `GOAL.md` (charter), `CLAUDE.md` (operating state), `log/` (11 dated chronicle
  entries), the four `.claude/skills/`, plus the off-repo budget file and cross-repo TODO. The
  discipline has been *sustained* across the repo's life and (per `CLAUDE.md`/global config)
  months in other repos — which is itself signal on **Q3** ("does external-state discipline scale
  or become its own friction?"): it has not been abandoned. *Outcome — did it actually lower
  re-orientation cost, where did it create friction:* **[maintainer]**.

- **G11 — Maintain a direction-and-outcome log to develop taste.** *Practiced: partially.* The
  `log/` entries record direction-*choices* with the reasoning at the time (e.g.
  `2026-05-05-direction-shift-foundation-first`, `2026-05-06-innovation-doc-moved-to-evidence`,
  `2026-05-17-goal-document-and-alignment`). That is the front half of G11. The **missing half** is
  the retrospective loop-back — "what came of this choice" revisited later — and the quarterly
  review. So the practice exists in embryo but is not yet the taste-developing instrument G11
  specifies. *Whether the logged reasoning has paid off:* **[maintainer]**.

- **G13 — Use AI as terrain map, not as agent.** *Practiced: plausibly, needs confirmation.* The
  step-0 landscape scan used parallel subagents to *map* the field (47 entities canvassed) while the
  maintainer chose the framing and located the repo's niche — the terrain-vs-navigation split G13
  describes. But this is a process claim the artifacts only weakly support. *Did navigation stay with
  the maintainer, or did AI's map quietly set the direction:* **[maintainer]**.

### Bucket B — Designed but not yet exercised here → live trials in flight

The discipline is built into the repo's process but has not actually been run to completion. These
become real evidence the moment the in-flight work finishes.

- **G10 — Treat AI literature reviews as starting graphs; traffic-light citations.** *Designed, not
  exercised.* The literature survey is explicitly staged so that step-0's sources are
  "subagent-verified at fetch time but not re-verified" and "nothing is citation-grade until it
  flows through `add-evidence`." That gate **is** G10 — but the green/yellow/red source-walk has not
  been done yet. The survey's stages 4–5 are a ready-made, concrete G10 trial. This is the single
  most actionable in-repo trial.

- **G3 — Verify AI output from an independent source.** *Designed, not exercised.* Same gate as G10
  at the citation level; the `add-evidence` schema requires a confidence label and source. Not yet
  exercised because no evidence has flowed through it to foundation-grade.

### Bucket C — Not practiced here → prospective-instrumentation gaps

Real gaps. Nothing on disk implements these. They are the candidates to **start** in Step 2 (the
prospective phase), because they only produce evidence going forward.

- **G7 — Calibration log of AI-vs-no-AI productivity.** *Not practiced.* The budget file logs
  tokens, not felt-vs-actual productivity. No calibration data exists. Given A13 + METR, this is
  arguably the highest-value gap to fill first, because it disciplines every other self-judgment in
  this stream.

- **G6 — Track the second output (researcher development).** *Not practiced.* `log/` chronicles the
  *inquiry*, not the maintainer's developing/atrophying capacities. No capability journal exists.

- **G15 — Log model, prompt, parameters, date.** *Not practiced.* No `.aimeta`/`.aicontrib` files
  exist (confirmed by glob); commit messages do not record model or prompt. The simplest guideline,
  and the one most clearly un-adopted.

### Bucket D — Not-yet-applicable here → need a research repo as subject

These target experiment design, innovation/recombination judgment, candidate selection,
replication, and exploration-share — none of which this methodology repo exercises. Auditing them
needs one of the maintainer's actual research projects (the research-engine, the EE-degree research,
the health-longevity / methodical-innovation corpora named in the cross-repo TODO).

- **G4** (recombination vs innovation classification), **G5** (refuse whole-task outsourcing on
  non-decomposable tasks), **G8** (score candidates before AI evaluates), **G9** (pre-mortem before
  experimental design), **G12** (protect exploration share), **G14** (replicate a paper as a
  verification primitive).
- **G1** (the meta-guideline, empower/replace at the job level) sits across all buckets: its
  discipline is *encoded* repo-wide (GOAL §commitment, CLAUDE.md), but whether the maintainer
  actually applied it at the substantive moments is **[maintainer]** and is best observed
  prospectively per Q10.

---

## What this pass yields

1. **Testing-candidates from existing artifacts:** G2 (strongest), G11 (partial), G13 (tentative) —
   subject to the maintainer's outcome judgment.
2. **In-flight trials to finish:** G10 and G3, via the literature survey's verification stage.
3. **Prospective gaps to instrument now:** G7, G6, G15 — the disciplines that only generate evidence
   going forward; G7 first.
4. **Deferred to a research repo:** G1 (applied), G4, G5, G8, G9, G12, G14.

A defensible **Step 2** (prospective phase): confirm **G2** as a `testing` write-up using the
existing record; stand up **G7** (the calibration log) and the minimal **G15** convention from today;
and treat the literature survey's next stage as the **G10** trial. That is three guidelines moving
toward real evidence within weeks, on work already happening.

## What I need from you to go further

- **Outcome judgments** on the `[maintainer]` cells above — especially G2 (did external state lower
  re-orientation cost, where did it add friction?) and G11 (did the logged reasoning pay off?).
- **Which research repo** to re-run this audit against for Bucket D, and whether I should have access
  to it.
- Confirmation that **Step 2's three picks (G2 / G7+G15 / G10)** are the right first trials, or a
  different selection.
