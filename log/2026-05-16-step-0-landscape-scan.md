# Literature survey kickoff — step 0 landscape scan (2026-05-16)

The literature survey planned in conversation begins today. Approach is staged: step 0 (shallow public-positions scan) → stage 1 (territories map) → stage 2 (existing artifacts to adopt) → stage 3 (per-territory literature pass) → stage 4 (read + integrate via `add-evidence`) → stage 5 (feed back to foundation via `update-foundation`). Working artifacts during the survey live under `evidence/survey-2026-05/`; only the durable outputs (reading-list entries, literature notes, foundation revisions) become permanent.

## What was done today

Three subagents ran in parallel, each covering a cluster of major public actors in the AI-for-research space. Twenty entities canvassed in total. Each entity's public position on *how research should be done with AI* was captured in one line with the canonical positioning URL verified by fetch. "No explicit position found" was treated as a valid finding.

Output: [`../evidence/survey-2026-05/step-0-landscape.md`](../evidence/survey-2026-05/step-0-landscape.md).

## What it surfaced

Five vectors in the field:

1. **Agentic delegation** (OpenAI, Sakana, FutureHouse, parts of Anthropic's internal alignment work) — AI does the research; human selects problems and evaluates.
2. **Augmentation with architectural prescription** (Elicit, Karpathy, NotebookLM, public Anthropic, DeepMind) — AI generates, human verifies; loop design matters.
3. **Craft / skill preservation** (Willison, Mollick, Royal Society) — practice matters; smallest vector by player count; closest to this repo.
4. **Governance / disclosure / cautionary** (Nature, Science, Bender, Marcus, NIH Bridge2AI, NSF) — frames what AI must not do, not how it should be used.
5. **Silence** (Brian Nosek / Center for Open Science most notably) — the natural institutional home for AI methodology norms in the open-science world has not staked a position.

**The exact niche the repo occupies** — positive methodology, individual-researcher scale, evidence-grown, foundation→guidelines structured, empower-not-replace as a positive design criterion (not only a warning) — appears unoccupied. Adjacent positions exist (Willison, Elicit, Mollick) but none is constructed as a methodology artifact. The repo is therefore not duplicate work, but lands in a space with adjacent voices that should be tracked.

## What changed in the inquiry's understanding

Three things worth carrying forward into the foundation:

- **The frontier-lab implicit principle is "automate what can be automated, keep humans for what cannot yet be automated."** This is the closest thing to a foil for the repo's empower-not-replace framing. Naming it explicitly in `foundation/00-why-reimagine.md` (e.g., in §1 or §4) would sharpen the argument by contrast. *Suggested for `update-foundation`, not done here.*
- **The centaur / cyborg vocabulary (Mollick) is mainstream in this space.** The repo currently uses neither. A decision — adopt, refine, or contest — should be made before the methodology gains more guidelines that touch on this vocabulary.
- **The open-science silence is significant if real.** COS / Nosek not staking a position on AI's effect on replication / preregistration is consequential and should be re-verified in stage 3 before the foundation treats it as durable.

## Still open

- Stage 1 (territories map) is the next concrete step. The territories list should be drafted with the maintainer rather than by the assistant alone, since the territory selection is the load-bearing decision for the rest of the survey.
- The step-0 doc's URLs were subagent-verified at fetch time but not re-verified. None of its citations are foundation-grade until they flow through `add-evidence`.
- The four "what to investigate at depth" items in §6 of the step-0 doc are candidates for stage-3 territories but are not yet committed.
