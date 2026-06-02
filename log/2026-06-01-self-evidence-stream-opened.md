# First evidence stream opened: self-study (2026-06-01)

The methodology has stood at 15 `proposed` guidelines with zero systematic evidence behind any of
them. Today the inquiry started closing that gap by opening its first **evidence stream**, after a
short planning step established the constraint: guideline promotion and most open questions resolve
through the *same* mechanism — instrumented observation of real AI-assisted research — so the next
step is to stand that engine up, not to write more guidelines or read more literature.

Of the three candidate streams (self-study / external interviews / pilot case study), the maintainer
chose **self-study first** — the cheapest, fastest-signal source, since the maintainer already runs
several of the guidelines de facto and months of artifacts exist to mine.

## What was done today

- Created `evidence/self-study/` as the workstream home, with a README stating the method, the
  honest n=1 / cluster-IV limitation, and the rule that an assistant records only what is observable
  and leaves outcome judgments to the maintainer.
- Ran the **first retrospective audit**
  ([`../evidence/self-study/2026-06-retrospective-audit.md`](../evidence/self-study/2026-06-retrospective-audit.md)),
  scoring this repo's own development history against G1–G15.

## What it surfaced

The 15 guidelines sort into four buckets against this repo:

- **Practiced & sustained (testing-candidates):** G2 (external state — strongest), G11 (direction
  log, partial), G13 (terrain-not-agent, tentative).
- **Designed but not yet exercised (in-flight trials):** G10 and G3, via the literature survey's
  not-yet-done verification/source-walk stage.
- **Not practiced (prospective gaps to start now):** G7 (calibration), G6 (second-output log), G15
  (AI metadata — confirmed absent: no `.aimeta` files, no model/prompt in commits).
- **Not-yet-applicable here (need a research repo):** G1-as-applied, G4, G5, G8, G9, G12, G14.

Proposed **Step 2** (prospective phase): confirm **G2** as a `testing` write-up from the existing
record; stand up **G7** + a minimal **G15** convention from today; treat the literature survey's
next stage as the **G10** trial. Three guidelines moving toward real evidence on work already
happening.

## Still open (maintainer)

- Outcome judgments on the `[maintainer]` cells (esp. G2 friction/benefit, G11 payoff).
- Which research repo to re-run the audit against for the Bucket-D guidelines.
- Confirm the Step-2 trial selection (G2 / G7+G15 / G10) or revise it.

## Housekeeping

- The lab survey (`evidence/lab-surveys/ai-tool-use-2026/`) remains awaiting data: the linked
  responses Sheet was created but had not propagated to the Drive integration's mirror by end of
  session. Reachable later via its file ID once it syncs.
