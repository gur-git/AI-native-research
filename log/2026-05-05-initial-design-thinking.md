# Initial design thinking (2026-05-05)

> **Preserved as a log entry.** This was the agent's first pass at a design for the repo, written after the initial reading and before any structure had been committed. It was superseded later the same day by a redirection from the maintainer (see [2026-05-05-direction-shift-foundation-first.md](2026-05-05-direction-shift-foundation-first.md)) toward a foundation-first approach. The original framing — "two well-built tools (lit-triage + research-log) plus a methodology document" — is no longer the v0 plan, but the analysis of attributes, decompositions, and tradeoffs is kept here for reference.

The original file:

---

Design notes for this repo. Written before any code or scaffolding. The point is to commit on paper to a defensible structure before building, and to flush out the questions that actually need a researcher's input.

---

## 1. What I read first, and what stuck

The brief named five sources as required reading. Here is what I took from each, condensed to the points that shape design choices.

### 1.1 Tao on Dwarkesh — the spine

The single most useful framing in the interview is that **AI cannot make partial progress**. Tao's image is a climber who can jump two metres in a random direction but cannot grab a handhold halfway up the cliff and pull from there. A new chat session "has forgotten everything it just did. Its understanding of math has not improved at all." Per-problem, the success rate on a representative slate of math problems is around 1–2%; the visible wins (e.g., ~50 of 1,100+ Erdős problems) come from publication bias on a much larger denominator.

Where AI clearly *does* help him: producing plots and numerics that previously took hours, drafting code, running secondary literature scans, formatting. The result is that his papers are now "richer and broader, but not necessarily deeper." The deep work is still pen and paper.

Two further points have outsized methodological weight:

1. **Formal verification (Lean) gives you atomic checking.** A long AI-generated proof can be decomposed lemma by lemma; you can run "ablation tests, removing parts of the proof to see what breaks." This is the only place in the workflow where AI output can be trusted at scale, because the checker is not the generator.
2. **Serendipity is an asset that AI workflows can quietly destroy.** Tao notes that hallway encounters and inefficient browsing have produced ideas; over-optimization can starve a researcher of inputs. Even a year at IAS with no distractions eventually dried him up. This is a counter-pressure to the "automate every step" instinct.

### 1.2 Beel / Kan / Baumgart on Sakana's AI Scientist (arXiv 2502.14297)

The honest evaluation of an autonomous-research system. The headline numbers I am keeping:

- **42% of experiments failed** because of coding errors.
- Literature reviews **misclassified established techniques as novel** (their example: micro-batching for SGD).
- Manuscripts had a **median of 5 citations**, only 5 of 34 from 2020 or later — a structural sign of poor lit-review depth.
- **The system could not critique itself.** Methodological flaws and logical inconsistencies passed.
- Papers contained **hallucinated numerical results**.

Reading this alongside Tao: Sakana is the empirical proof of his "AI cannot do partial progress" claim at the scale of an entire paper. The system can produce something that *looks like* research; the failure surfaces are exactly the places that need self-critique and cumulative iteration.

### 1.3 METR's 2025 RCT — the cautionary anchor

Sixteen experienced open-source developers, 246 randomized tasks, frontier tools (Cursor + Sonnet 3.5/3.7). Headline: **AI-allowed conditions made tasks 19% slower.** The crucial second number is the perception gap — pre-task they expected ~24% speedup; post-task they reported ~20% speedup; the data showed −19%. **A 39-point gap between felt and measured productivity.**

Implication for any methodology: **self-reports about AI's effect on research speed are systematically unreliable.** A serious AI-native methodology has to bake in some form of objective measurement, or at minimum a calibration practice, or it is hype-shaped.

### 1.4 The system-level builders (FutureHouse, DeepMind, OpenAI, Anthropic, PSI)

The point of reading these is to know what this repo is *not* trying to be.

- **FutureHouse / Robin** orchestrates Crow / Falcon / Owl / Phoenix / Finch agents and produced a published candidate (ripasudil for dry AMD); humans ran the wet lab. Good demonstration of multi-agent decomposition.
- **DeepMind's AI co-scientist** (Gemini 2.0 multi-agent, generate-debate-evolve) reproduced an antimicrobial-resistance hypothesis at Imperial that took the human team years.
- **OpenAI Deep Research** — fast, cited synthesis, but documented failures: outdated data, deference to less reliable sources (Reddit), overconfidence in its own corroboration.
- **Anthropic's Claude for Life Sciences / Operon** is closer to our layer: domain skills, scoped tools, "encode the methodology as a skill" rather than autonomous agency. Cheeseman lab's emphasis on **confidence levels** is worth borrowing.
- **Wissner-Gross's Physical Superintelligence (PSI) / GPD** — see §1.5 below; treated separately because of one specific contribution that isn't replicated by the others.

These are competing at the *systems* layer. This repo is at the **methodology and practice** layer for an individual or small-group researcher who wants to use the best off-the-shelf tools well, rather than build a new agentic system.

### 1.5 Wissner-Gross / PSI / GPD — replication as a verification primitive

Wissner-Gross frames PSI as building "an AI system that reasons like a theorist, validates like a computational physicist, tests like an experimentalist, discovers what none of them could alone." The interesting methodological move sits underneath that framing: the **Get Physics Done (GPD)** framework, which Lawrence Berkeley used to "flawlessly" replicate a 2023 condensed-matter paper on emergent magnetic monopole lattices end-to-end with JAX. He also flags the GPT-5.4 Pro proof of Erdős Problem 1196 that was then adapted to crack an Erdős-Sárközy-Szemerédi conjecture — which he calls "perhaps the first AI-generated proof to have downstream impact."

Two things to take from this for the methodology:

1. **Replication is a verification mode that doesn't fall to the Sakana failure pattern.** When AI generates *and* AI evaluates, you get the self-validation bias the Sakana paper documented. When AI replicates a third party's published result end-to-end, the published result is the oracle — the generator is not the judge. This sits alongside formal verification (Lean) and human review as a third independent verification primitive. Operationally cheap to adopt: pick a recent paper in your area, ask AI to re-derive or re-implement it, see what breaks.

2. **The Erdős 1196 → ESS-conjecture chain is a partial counterexample to Tao's "AI cannot make partial progress."** It worked because a *human* recognized the AI's first proof was a building block for a second problem. The lesson isn't that AI now does cumulative work — it's that the **human researcher's role as the carrier of cumulative state** is exactly the bottleneck the methodology should address (§3.1).

PSI itself is a competitor at the systems layer; this repo is not trying to build GPD. But "replication of a recent paper" is a methodology primitive worth promoting as a practice that any researcher can do today.

---

## 2. The decomposition

The brief warned against assuming the standard "lit review → experiment → writing" decomposition is right. I think it is wrong, or at least lossy, for AI-native work. Two things that decomposition hides:

- **Continuity.** An AI session forgets. The methodology has to specify *where the state lives* across sessions.
- **Calibration.** Felt productivity is wrong by ~40 points (METR). The methodology has to specify how the researcher knows whether AI is actually helping.

I prefer to decompose by **cognitive operation**, not by project phase. The operations recur at every phase.

| # | Operation | Where AI clearly helps | Where AI clearly hurts | Methodological response |
|---|-----------|------------------------|------------------------|-------------------------|
| 1 | **Scoping** — turning intuition into a tractable question | Reframings, related-field analogies, sanity-checking the question hasn't been answered | Cannot judge "interestingness"; will validate any framing the user proposes | Use AI for breadth, never to *decide* what's worth working on |
| 2 | **Mapping** — knowing what exists | Citation graph traversal, structured summaries, finding obscure related work | Hallucinated citations; outdated data passed as current (Deep Research); novelty misclassification (Sakana) | Treat AI lit reviews as a starting graph; spot-check every cited claim against the source |
| 3 | **Hypothesis generation** | High volume of plausible candidates; cross-domain transfer (DeepMind co-scientist) | Cannot distinguish "novel-sounding" from novel; no taste | Score candidates AI-blind by an expert before AI gets to evaluate them |
| 4 | **Design** (experiment / proof / artifact) | Scaffolds, edge-case checklists, code skeletons, protocol drafts | Subtle methodological flaws; missing controls; no falsification thinking by default (Sakana) | Pre-mortem prompt that forces explicit "what would falsify this"; design review with a separate AI session and a human |
| 5 | **Execution** | Cheap code, fast plotting, fast numerics (Tao); compress months → hours on routine analysis (Anthropic case studies) | Buggy code (42%, Sakana); 1–2% per-problem success in math (Tao); experts ~19% slower in coding (METR) | Instrument actual outcomes; do not trust felt speed |
| 6 | **Verification & critique** | Second-reader sanity checks; rough self-consistency | Self-validation; cannot reliably catch its own mistakes (Sakana, Deep Research) | Verification must come from a *different source* than generation. Three modes work: **formal tools** (Lean — Tao), **replication of a third-party result** (PSI/GPD at LBNL — §1.5), and **human review**. Pick at least one before trusting an AI output. |
| 7 | **Synthesis & writing** | Drafts, formatting, plot generation, structuring arguments | "Richer and broader, not deeper" (Tao); fluent text masking empty claims | Human owns the thesis; AI helps the prose; never ship unread AI text |
| 8 | **Continuity** — keeping state across sessions | Almost nothing, by default | Session forgetting is the *default* failure mode (Tao) | This is where most of the methodology's leverage lies — see §3 |
| 9 | **Calibration** — knowing whether AI is helping | Very little | Felt vs measured productivity gap of ~40 points (METR) | Track time, track decisions, log negative findings; build a personal dataset |

I'd argue **8 and 9 are the underweighted ones in every framework I read for this brief.** Most "AI for science" work is at operations 1–7. The repo's distinctive contribution should be heavy on 8 and 9, because they are where individual researchers can act *today* with no infrastructure and where a public methodology document has the highest marginal value.

---

## 3. The two underweighted operations, in more detail

### 3.1 Continuity — the external state commitment

Tao's "AI has forgotten everything" is the deepest structural problem with AI-native work. A serious response is not "use a longer context window" — that's a tooling answer. The methodology answer is:

> The researcher commits to maintaining an explicit, version-controlled, human-curated **external state** of the project — a research log, decision journal, prompt library, and result ledger — that any AI session can be re-grounded on, and that survives across model upgrades, vendors, and even the researcher's own forgetting.

This is structurally similar to lab notebooks but adapted for the AI loop: every session starts by loading state, every session ends by updating it. The artifact is the state, not the chat.

Concrete things this implies for the repo:
- A research log template that is *designed to be re-loaded* into context, not just written to be read.
- A prompt library where prompts include the project's accumulated context and assumptions.
- An "AI contribution ledger" — what AI did, which model, what prompt, what verification was applied — attached to every result, for reproducibility and honest attribution.

### 3.2 Calibration — beating the perception gap

METR shows that experts thought they were 20% faster while being 19% slower. That gap will appear in research too, and probably worse, because research outcomes are slower to fall out than passing a test or merging a PR.

A methodology that answers this needs at least:
- **Time-on-task tracking** for AI-assisted vs unassisted work, even crudely (per-day estimates).
- **Negative finding logs** — places where the AI wasted time, suggested wrong things, or required so much correction that it would have been faster by hand. These need a frictionless place to live, or they don't get written.
- **A decision journal entry** for any AI suggestion that materially shaped a research direction, so that in 6 months you can audit which directions actually paid off.

This is unglamorous but it's the part of an AI-native methodology that a working researcher could *credibly publish on* with a year's data. There's a real artifact-shaped opportunity here.

---

## 4. What artifacts would actually help a working researcher today

Sorted by my view of leverage. Each is a candidate first build.

| Artifact | What it is | Why it matters | Build cost |
|---|---|---|---|
| **A. Research-log scaffold** | Markdown templates (daily / weekly / per-thread) + a small Python helper that compiles them into a single context block to paste into a new AI session | Directly addresses §3.1 (continuity). Frictionless. Useful from day one. The "load state into AI" step is the unique insight. | Low |
| **B. Literature-triage tool** | Python CLI: takes a research question and a list of papers (or a search), uses Claude with structured output to produce a triage table with extracted claims, methods, and explicit "I might be wrong about this" confidence flags. Cites with links. | Operations 2 and 3. Most universally useful runnable artifact. Demonstrates "use AI well" with prompt-caching, structured outputs, source grounding. | Medium |
| **C. AI-contribution ledger** | Markdown schema + Python helper that wraps a research code run and records: model, prompts, diffs accepted, verification applied. Drops a `.aicontrib.md` next to each artifact. | Reproducibility and honest attribution. Operationalizes the Sakana lesson into a small commitment. | Low–Medium |
| **D. Pre-mortem / experiment-design prompt suite** | A versioned set of prompts that force a research design through "what would falsify this," "what control is missing," "what would a hostile reviewer say" before any code is written. | Operation 4. Cheap, methodologically rich. | Low |
| **E. Calibration tracker** | Tiny CLI: log "task X: estimated AI helped by Y%, actual time vs baseline Z." Accumulates personal data over time. Outputs a monthly self-report. | §3.2. The piece of the methodology that produces *evidence* over a year. | Low |
| **F. Reproducibility scaffold for AI-coauthored code** | Project template: standard layout, `aicoauthor.toml` manifest of which models/prompts touched the code, examples of declaring AI contributions in papers. | Bridges to publication norms. Probably v0.2 of the repo, not v0.1. | Medium |

**My recommended first pair:** **B (Literature triage) + A (Research log).**

Reasoning: B is the one that *runs* — it's the Karpathy-style runnable artifact that a visitor will skim, run, and remember. It also demonstrates real engineering (prompt caching, structured outputs, source grounding, honest "confidence" surfaces). A is the one that *commits* the methodology to a workable practice — it makes the continuity argument concrete and the repo immediately useful even without code execution.

Together they hit both halves of the brief: a runnable tool *and* a methodological artifact.

**Strong alternative:** **B + E (calibration tracker).** This pair leans harder into the "honest about AI in research" angle and would produce a self-experiment over a year. Less immediately useful to other researchers; more distinctive as a public-methodology project.

I'd want the user's input here before committing. See open questions §7.

---

## 5. Proposed repo structure

```
/
├── README.md                  ← public face; honest "in-progress"; no-contributions notice; contact
├── LICENSE                    ← MIT (recommended; see §7)
├── CONTRIBUTING.md            ← read-only policy; how to follow along; collaboration contact
├── CITATION.cff               ← so people can cite the repo if they reference it
│
├── methodology/
│   ├── 00-overview.md         ← the foundational methodology document
│   ├── 01-continuity.md       ← (later) deeper treatment of §3.1
│   ├── 02-calibration.md      ← (later) deeper treatment of §3.2
│   └── README.md              ← reading order
│
├── tools/
│   ├── lit-triage/            ← runnable tool B
│   │   ├── README.md
│   │   ├── pyproject.toml
│   │   ├── src/lit_triage/
│   │   ├── examples/
│   │   └── tests/
│   └── research-log/          ← scaffold A
│       ├── README.md
│       ├── templates/
│       ├── prompts/
│       └── scripts/           ← state-compilation helper
│
├── case-studies/
│   └── README.md              ← placeholder; pilot research will land here once domain chosen
│
├── references/
│   └── reading-list.md        ← annotated, with the sources used to build this
│
└── .github/                   ← issue templates noting "not accepting PRs yet" if helpful
```

**Choices baked in here that I want to flag:**

- **No top-level `pyproject.toml`** for the whole repo. Each tool gets its own. Reason: the tools are independent; coupling them now invents complexity. Reverse-able.
- **`methodology/` not `docs/`.** "docs" implies reference material; "methodology" signals the substance.
- **`case-studies/` is a real directory with a placeholder.** This is where the pilot research will live. Naming it now shapes the repo's identity as evidence-driven, not essay-driven.
- **`references/reading-list.md` not `bibliography.bib`.** A reading list with annotations is more honest about what shaped the methodology than a flat citation file. If/when the methodology document is more academic we add `.bib`.

---

## 6. Tone, framing, and what the README must commit to

I want the README to have these properties, on the strength of what I read:

1. **Honest "in-progress."** Not "v0.1.0," not "early days but we're cooking" — a paragraph that says: the methodology is being written *while* the user does real research; it will change; expect to see things rewritten and removed.
2. **A specific anti-claim.** Something like: "this repo is not a recipe for autonomous research. It is a methodology for a researcher who wants AI to be a serious collaborator without lying to themselves about its contribution." Distinguishes from FutureHouse / Sakana / co-scientist explicitly.
3. **A "what's actually here right now" section** with two links — one to the methodology document, one to the runnable tool. So a 30-second visitor leaves with one thing they could try.
4. **A negative-findings section, even if empty at v0.** Signals seriousness.
5. **Read-only / collaboration note** with contact: `masuryg@post.bgu.ac.il` (per user's message above).

---

## 7. Open questions for the user

Before I build, I want answers — or explicit "your call" — on these. They have real tradeoffs.

1. **Pilot domain timing.** When the user picks a research domain, will artifacts from that pilot live in this repo (`case-studies/`) or stay private? This affects how I write the placeholder and how I scope the methodology document. *Default if no answer:* assume they will live here, eventually.

2. **First-pair choice.** I recommend **B (lit-triage) + A (research log)**. The strong alternative is **B + E (calibration tracker)**. Which?

3. **Stack preference.** Python with `uv` + `pyproject.toml` per tool, `pytest`, `ruff`. Anthropic Python SDK (since the user is on Anthropic infra). Anything to swap?

4. **Model-agnostic vs Claude-first.** Karpathy purity says model-agnostic; pragmatism says use Claude well (prompt caching, citations, structured outputs). I lean Claude-first with a clean abstraction so swapping later is one file. *Default:* Claude-first.

5. **License.** MIT (most permissive) or Apache-2.0 (patent grant)? *Default:* MIT.

6. **Voice.** First-person singular ("I find that…"), academic plural ("we propose…"), or methodology-document neutral ("the researcher should…")? Tone choice matters because the README will set it. *Default:* first-person singular for the methodology document, neutral for tool READMEs.

7. **Audience width.** Two profiles: (a) methodology-curious researchers who want a worked-out framing; (b) working researchers in any field who want a tool they can run today. The repo can serve both, but the README has to pick which voice leads. *Default:* (b) leads, (a) follows.

8. **Naming.** Repo is `AI-Native-research`. The methodology phrase I'd use throughout is "AI-native research methodology." Anything to push back on?

9. **First commit policy.** Squash everything into one initial commit, or commit step-by-step (scaffold → methodology → tool A → tool B)? Step-by-step gives a more readable history for visitors browsing commits. *Default:* step-by-step.

10. **Citation expectation.** Does the user want a `CITATION.cff` from day one, or is that premature? *Default:* yes from day one — it costs nothing and signals the repo is meant to be cited.

---

## 8. Risks I'm tracking

- **Looking like another "AI for science" hype repo.** Mitigation: the methodology document opens with the METR finding and the Sakana failure rates, before any optimism.
- **Building tools that don't actually run.** Mitigation: every tool ships with one working example you can run end-to-end with `uv run`.
- **Methodology that's too abstract.** Mitigation: every section of the methodology document closes with a concrete practice the reader could adopt this week.
- **Scope creep before v0.** Mitigation: two tools, well-built. Defer C–F to follow-up commits and make that explicit.

---

## 9. What happens after this file

Per the brief: **stop here, wait for feedback.** The next step is the user reviewing this file, answering the open questions in §7 (or telling me to use defaults), and then I build:

1. README, LICENSE, CONTRIBUTING, CITATION.cff, scaffolding
2. `methodology/00-overview.md` (the foundational document)
3. The first tool (whichever pair we agreed on)
4. The second tool
5. `references/reading-list.md`

Quality bar: a researcher at a conference clicks the URL, reads for two minutes, and thinks "this person is doing serious work." Two well-built tools, one substantive methodology document, an honest README.
