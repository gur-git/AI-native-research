# Foundation restructure and empower-not-replace as central mindset (2026-05-06)

The largest single update the foundation has had since its initial draft. Recording the full scope.

## What prompted it

Conversation with the maintainer over several rounds, in which the foundation as written through 2026-05-05 was diagnosed as one-legged. Specifically:

- **The cost-structure framing in `00-why-reimagine.md`** treated AI's effect on knowledge work as uniformly inverting the production/judgment cost balance. The maintainer pointed out — correctly — that this misses what is actually new about AI compared to prior tools.
- **What is actually new** is that AI is the first tool that can produce useful output without requiring the user to develop any reciprocal skill. Prior tools (calculators, compilers, GPS) all changed the skill set; the user still developed compensating capability. AI breaks the pattern.
- **The right response** is not just better verification practices (which the previous foundation already gestured at) but a mindset shift: *empower, not replace.* Use AI in ways that grow the researcher, not as a substitute for them.
- **Several things follow** that the previous foundation did not say: the temptation to outsource is a trap (skill atrophies without compensation), research tasks resist clean decomposition (so partial outsourcing is awkward and the gradient pulls toward whole-task outsourcing), research has two outputs (the deliverable and the researcher's growing competence) and AI specifically endangers the second.
- **The foundation's structure was also unclear.** The numbering created false hierarchy (innovation as 04 felt like an afterthought when it is a deep-dive on the central argument), and naming `02-what-this-implies.md` was vague about purpose.

## What changed

### Foundation restructure

Files renumbered/renamed for a clearer reading order:

- `04-innovation.md` → `02-innovation.md` (deep-dive comes right after the catalog)
- `02-what-this-implies.md` → `03-implications.md` (clearer name, repositioned)
- `03-open-questions.md` → `04-open-questions.md` (questions last)

`00-why-reimagine.md` and `01-ai-attributes.md` kept their numbering. Foundation README rewritten as a strong reading guide explaining what each file is for and what reading order to follow.

### `foundation/00-why-reimagine.md` — substantial rewrite

Rewritten per a new §1–§6 structure agreed in conversation:

- **§1 Shared starting points** — what most thoughtful researchers already see about AI's impact. Establishes the floor.
- **§2 What you may not have followed through on yet** — the structural claim. AI as the first tool that substitutes for skill without reciprocal skill. The three consequences that follow (outsourcing as trap, tasks resist decomposition, two outputs).
- **§3 Why research is the case that matters most** — four structural reasons research is sharply exposed. Includes the recombination/innovation distinction in compact form (with pointer to `02-innovation.md`).
- **§4 Why now: the default is degradation** — the urgency section, grounded in the gradient toward replacement. Inertia is not neutral; waiting is a vote for the default.
- **§5 The mindset shift: empower, not replace** — the central call to action. Explicit: AI used in ways that grow the researcher (empower) vs. AI used to produce outputs the researcher could not have produced and now will not learn to produce (replace).
- **§6 What this repo is** — compressed; carries the structure-of-the-inquiry information.

### `foundation/01-ai-attributes.md` — cluster V added

New cluster V "AI changes the user" with two attributes, both `structural`:

- **A16: Output without reciprocal skill development.** The structural fact about AI as a tool. Argues this is the load-bearing claim of the empower-not-replace mindset.
- **A17: Tasks resist clean decomposition into "AI part" and "human part".** Why partial outsourcing is awkward and the gradient pulls toward whole-task outsourcing. Joint property of research tasks and how AI is offered.

Cross-cluster note updated to flag that A16 and A17 are the attributes most underweighted in mainstream AI commentary, because they describe slow effects on the user that are invisible in short-term productivity measurement. A1 (breadth without depth) cross-references the new cluster.

### `foundation/02-innovation.md` — light update for consistency

Connected explicitly to the empower-not-replace mindset. The §3 "AI's role in innovation" gains a paragraph noting that innovation work is where the empower/replace question lands hardest, because innovation requires exactly the skills (taste, depth, negative-space recognition) that whole-task outsourcing erases. Cross-references updated for the new file numbering.

### `foundation/03-implications.md` — reframed around empower-not-replace

Reframed from four cluster-derived directions to: a meta-frame (empower-not-replace as the question every gesture is evaluable against) plus five cluster-derived directions, with cluster V (AI changes the user) as the new fifth direction. The four original directions also reread under the new frame; e.g. "research as portfolio" now flagged as having both empowering and replacing variants depending on whether the researcher's taste develops through repeated direction-and-outcome practice.

### `foundation/04-open-questions.md` — new questions added

Q10 (how does a researcher distinguish empowerment from replacement in the moment), Q11 (how should the methodology track researcher development), Q12 (does empower-not-replace generalize across research domains). Cross-references updated for new file numbering.

### `foundation/README.md` — strong reading guide

Rewritten as a substantial reading guide explaining purpose of each file and suggested reading paths for different time budgets.

### `methodology/guidelines.md` — schema update + 15 initial guidelines

Schema updated to require a **Skill implication** field. The point: a guideline that cannot articulate what skill it builds is one that risks substituting for skill, and the methodology's central principle cannot tolerate that.

15 initial guidelines added, all at status `proposed`, drawn from the foundation as written through today:

- **G1: Treat empower-vs-replace as a question to ask at every AI use.** The meta-guideline.
- **G2: Maintain external project state in version-controlled files.** Cluster III.
- **G3: Verify AI output from a different source than the one that generated it.** Cluster II; three modes (formal, replication, human review).
- **G4: Distinguish recombination from innovation work; apply different practices to each.** Cluster I + innovation framework.
- **G5: For tasks that resist clean decomposition, refuse whole-task outsourcing.** Cluster V.
- **G6: Track the second output (researcher development) deliberately.** Cluster IV + V.
- **G7: Maintain a calibration log of personal AI-vs-no-AI productivity.** Cluster IV.
- **G8: Score AI-generated candidates against your own ranking before AI evaluates.** Cluster I + II.
- **G9: Pre-mortem prompt before any experimental design.** Cluster II.
- **G10: Treat AI literature reviews as starting graphs, not finished reviews.** Cluster II (A8); color-coded citation system.
- **G11: Maintain a direction-and-outcome log to develop taste over time.** Innovation framework; addresses Q7.
- **G12: Resist the exploitation gradient; deliberately maintain exploration share.** Innovation framework (March's drift).
- **G13: Use AI as terrain map, not as agent.** Cluster V; especially for innovation work.
- **G14: Replicate a recent paper as a verification primitive.** Cluster II; Wissner-Gross GPD operationalized.
- **G15: Standardize logging of model, prompt, parameters, and date for reproducibility.** Cluster III (A12).

None of these have evidence yet. All start at `proposed`. Promotion requires deliberate trial.

### `methodology/README.md`

Rewritten to state empower-not-replace as the guiding principle and to make explicit that every guideline must articulate its skill implication.

### `.claude/skills/add-guideline/SKILL.md`

Skill-implication input added to the schema; flagged as required, with the rationale that a guideline that cannot articulate the skill it builds is one that risks substituting for skill.

### `CLAUDE.md`

Fourth discipline added: **empower over replace**. Tools and practices proposed in this repo should grow the researcher, not substitute for them. Status updated to "Foundation v1 as of 2026-05-06."

### `README.md` (top-level)

Rewritten central summary to lead with the structural claim (AI as the first tool that substitutes for skill without reciprocal skill) and the empower-not-replace mindset. "What this is not" updated to include "not a way to do research faster while letting AI do more of it."

### `evidence/reading-list.md`

Added a new section "Empower-not-replace lineage (foundation cluster V anchors)" with two entries:

- **Engelbart (1962) — Augmenting Human Intellect.** Foundational; computing-as-augmentation framing predates AI by 60 years and is the lineage cluster V's central claim sits in.
- **Anthropic (Feb 2026) — How AI assistance impacts the formation of coding skills.** Direct empirical anchor: 17% lower mastery scores for AI-assisted vs by-hand learning, with the countervailing finding that participants who used AI as a learning aid (asking explanations, posing conceptual questions) maintained mastery. Empirical support that the empower/replace distinction matters in the data, not just in principle.

## Files touched today

```
CLAUDE.md
README.md
foundation/README.md
foundation/00-why-reimagine.md
foundation/01-ai-attributes.md
foundation/02-innovation.md (renamed from 04-innovation.md)
foundation/03-implications.md (renamed from 02-what-this-implies.md)
foundation/04-open-questions.md (renamed from 03-open-questions.md)
methodology/README.md
methodology/guidelines.md
.claude/skills/add-guideline/SKILL.md
evidence/reading-list.md
log/2026-05-06-foundation-restructure-empower-not-replace.md (this entry)
```

## What is still open after today

The open-questions file now has 12 entries. The most pressing for the methodology's near-term progress:

- **Q10:** How does a researcher distinguish empowerment from replacement in the moment? The mindset is now central; recognizing it at the point of choice is not yet operational.
- **Q11:** How should the methodology track researcher development? G6 proposes one candidate; others need to be tried.
- **Q9:** Is the methodology biased toward defense? The empower-not-replace framing is meant to address this in part, but the generative side (what new research becomes feasible) is still underdeveloped.

The next concrete steps the inquiry needs are evidence — interviews with working researchers, structured self-experiments by the maintainer, the choice of pilot research domain. The foundation has done as much as the current evidence base supports; further refinement requires new input.
