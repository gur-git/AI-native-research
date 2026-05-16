---
type: survey-artifact
stage: step-0 (shallow public-positions scan)
date: 2026-05-16
status: provisional — orientation only, not citation-grade
---

# Step 0 — Landscape of public positions on research-with-AI

> **About this document.** This is a working artifact from the first step of a literature survey on AI-native research methodology, not a foundation claim and not a finished literature review. The survey's deeper stages (per-territory literature pass, primary reading, integration into the foundation) come later. Step 0 is a shallow public-positions scan whose job is to orient the inquiry — to answer "is the field converged, contested, or scattered?" — before deeper reading begins. URLs were verified at the time of writing by subagent fetch but have not been re-verified for the foundation; nothing in this document is citation-grade until it is.

---

## 1. Purpose

To map, at the shallowest useful depth, the public positions of major actors in the AI-for-research space on the question: **how should research be done with AI?**

The inquiry needed this before doing deeper literature work for three reasons:

1. To know whether the niche the repo occupies (positive methodology, individual-researcher scale, evidence-grown, foundation→guidelines structured, empower-not-replace as the design criterion) is already occupied by a major player. If it is, this repo is duplicate work and should pivot.
2. To know which adjacent positions are loud enough to need engagement (adoption, refinement, or contestation) when the foundation is revised.
3. To know what vocabulary the field has already settled on so the repo does not unwittingly reinvent terms.

## 2. Method

Three subagents ran in parallel on 2026-05-16, each covering a cluster of ~5–8 entities. For each entity, they were asked to find the canonical positioning piece (verified by fetch), summarize the explicit public position in one line, and classify the framing as augmentation / replacement / cautionary / other. "No explicit methodology position found" was treated as a valid finding rather than a failure.

Twenty entities were canvassed across three clusters:

- **Frontier labs and autonomous-research systems:** Anthropic, OpenAI, Google DeepMind, FutureHouse, Sakana AI.
- **Augmentation tools and individual voices:** Elicit, NotebookLM, ResearchRabbit, Perplexity Deep Research, Ethan Mollick, Andrej Karpathy, Simon Willison.
- **Institutions, metascience, critics, and venues:** Stanford HAI, Allen Institute for AI (Ai2), the Royal Society, NSF AI Institutes, NIH Bridge2AI, Brian Nosek / Center for Open Science, Emily Bender / Gary Marcus, Nature and Science editorial policies.

Limits of this method are stated in §5. The canvass is not exhaustive — it samples enough entities to detect dominant vectors but cannot establish absence of a position with confidence.

## 3. The five vectors found

### Vector 1 — Agentic delegation / "AI does the research"

**One-line.** AI takes over execution of the research cycle (literature, hypothesis, experiment, paper); the human retains problem selection, evaluation, and ethical decisions.

**What research looks like in practice.** A human submits a research area or question. An autonomous agent (or multi-agent system) executes the full pipeline — literature search, hypothesis generation, experimental design, code, sometimes wet-lab execution paired with automation, paper drafting. The human reviews at end of cycle, redirects, or evaluates. The unit of work is the project, not the task. Productivity claims are stated in cycle-time compression (FutureHouse: "one day of our AI Scientist accomplishes what human scientists accomplish in 6 months"; Sakana AI Scientist v2 published in Nature, March 2026, after running the full pipeline). Methodology emphasis is on automated verification (benchmarks, outcome-grading, replication) because human inspection cannot scale to the volume of output.

**Tools associated with this vector.** Sakana AI Scientist (v1, v2), FutureHouse's Robin / Phoenix / Finch / Crow / Owl agents, OpenAI Deep Research (for the literature portion), Google DeepMind's AI co-scientist (for hypothesis generation), Anthropic's internal Automated Weak-to-Strong Researcher framework.

**Players and evidence.**

- **OpenAI** — Deep Research framed as doing work "for you independently." Sam Altman: "intern-level research assistant by September 2026," "legitimate AI researcher by 2028" (TechCrunch, October 2025). Sources: [introducing-deep-research](https://openai.com/index/introducing-deep-research/), [Altman / 2028 researcher](https://techcrunch.com/2025/10/28/sam-altman-says-openai-will-have-a-legitimate-ai-researcher-by-2028/).
- **Sakana AI** — AI Scientist v2 published in Nature, March 2026. The architecture is fully autonomous end-to-end; human involvement is initial direction + ethical oversight (IRB approval, withdrawal of submissions). Source: [ai-scientist-nature](https://sakana.ai/ai-scientist-nature/).
- **FutureHouse** — "A research institute that pairs AI Scientists with exceptional human scientists to do science more efficiently than before." Robin (announced 2024) is the end-to-end demonstration. Source: [futurehouse.org/about](https://www.futurehouse.org/about), [Robin announcement](https://www.futurehouse.org/research-announcements/demonstrating-end-to-end-scientific-discovery-with-robin-a-multi-agent-system).
- **Anthropic — internal** — "Automated Weak-to-Strong Researcher" (alignment team, 2026) explicitly frames the division as: automate outcome-gradable problems, free humans for vaguer / riskier ones. Source: [alignment.anthropic.com — automated-w2s-researcher](https://alignment.anthropic.com/2026/automated-w2s-researcher/).

**What this vector does not address.** Whether researcher skill should develop as a goal in itself. The Anthropic W2S piece is candid that "supervising Claude requires the very coding skills that may atrophy from AI overuse" — the tension is named, not resolved. No camp member articulates a positive view of researcher growth as a design criterion.

---

### Vector 2 — Augmentation with architectural prescription

**One-line.** AI is positioned as a collaborator, but with explicit architectural rules about the human's place in the loop (verification, supervision, source-grounding, autonomy sliders).

**What research looks like in practice.** The researcher works in a tool environment with explicit human-AI loop boundaries. AI generates; the human verifies. Each AI action is auditable — citation transparency, reasoning logs visible to the user, outputs grounded only in the source corpus the user provided. Workflow design is a methodological decision: define success criteria up front, build in checkpoints, prefer tools that expose AI reasoning over those that do not, accept friction in exchange for verifiability.

**Tools and methodologies.** Elicit (literature workflow with supervision interfaces and reasoning logs), NotebookLM (source-grounded — AI cannot answer from outside the user's notebook), Anthropic's Claude in agent / projects modes with explicit checkpoint behavior, Karpathy's described workflow ("autonomy sliders," human-as-verifier).

**Players and evidence.**

- **Elicit** (formerly Ought) — "Supervise the process, not the output" is the explicit operating principle. Co-founder Jungwon Byun: "people are increasingly going to be put in the position of having to evaluate and be really explicit and mindful of what success looks like before then using AI tools to manifest that." Source: [latent.space — Supervise the Process of AI Research](https://www.latent.space/p/elicit).
- **Andrej Karpathy** — Software 3.0 keynote at Y Combinator AI Startup School, June 2025. "Autonomy sliders," "they are doing the generation, and we as humans are doing the verification." Iron Man suit analogy: augmentation that can be autonomous in some contexts but always requires oversight capacity. Source: [Software Is Changing (Again) transcript](https://singjupost.com/andrej-karpathy-software-is-changing-again/).
- **NotebookLM (Google)** — tagline "AI Research Tool and Thinking Partner." Source-grounding is the core architectural commitment: AI stays within the user-provided corpus. No deeper methodology manifesto. Source: [notebooklm.google](https://notebooklm.google/).
- **Google DeepMind** — Hassabis frames AI as "tool that could help the best scientists in the world make discoveries," lists the human's role as: select problems, interpret what AI does, decide what to deploy. Source: [IAS talk, May 2025](https://blog.biocomm.ai/2025/06/05/sir-demis-hassabis-on-the-future-of-knowledge-institute-for-advanced-study/). The co-scientist paper frames the system as a "collaborative partner": [arXiv 2502.18864](https://arxiv.org/abs/2502.18864).
- **Anthropic — public** — "How scientists are using Claude" (already in [reading-list.md](../reading-list.md)) and the AI for Science Program: [anthropic.com/news/ai-for-science-program](https://www.anthropic.com/news/ai-for-science-program). Augmentation language; researcher remains the actor. Compare with Anthropic's internal W2S piece (Vector 1) for the tension.

**What this vector does not address.** Skill formation as a positive design criterion. The architecture protects the human's role; it does not prescribe what the human should become better at.

---

### Vector 3 — Craft / skill preservation

**One-line.** AI use is a practice that can be done well or badly; the researcher is the constant; how the practice changes the researcher is the methodologically interesting question.

**What research (and knowledge work) looks like in practice.** AI is one of many instruments. Choosing how to use it is a methodological decision worth deliberating. Heavy emphasis on what the practitioner can do without AI (because that is the baseline that decays with overuse). Mollick's "always invite AI to the table" is paired with his explicit warning about skill atrophy. Willison treats his iterative LLM-coding workflow as a craft; context curation and testing are skills he names. Royal Society explicitly warns against researchers being incentivized to be "good at AI" rather than "good at science."

**Tools.** Tool-agnostic — the methodological move is reflective practice with whatever tool, not adoption of a specific one. Mollick uses commercial frontier models for his teaching; Willison uses Claude / GPT / open models documented on his blog. The unit of methodology is the practice, not the tool.

**Players and evidence.**

- **Ethan Mollick** — *Co-Intelligence* (book, April 2024) and Substack *One Useful Thing*. The "centaur / cyborg" framing and the "always invite AI to the table" rule, paired with the skill-atrophy warning ("less accurate answers than those who were not allowed to use AI"). Source: [Centaurs and Cyborgs on the Jagged Frontier](https://www.oneusefulthing.org/p/centaurs-and-cyborgs-on-the-jagged) (September 2023).
- **Simon Willison** — "Here's how I use LLMs to help me write code" (March 2025). LLMs as "over-confident pair programming assistant"; context management is the new skill; testing "is the one thing you absolutely cannot outsource to the machine." Source: [simonwillison.net — using-llms-for-code](https://simonwillison.net/2025/Mar/11/using-llms-for-code/).
- **The Royal Society** — "Science in the Age of AI" (May 2024). Warns against AI substituting for scientific judgment; calls for AI literacy investment and human ability to scrutinize / verify / replicate AI-assisted experiments. Source: [royalsociety.org — Science in the Age of AI executive summary](https://royalsociety.org/news-resources/projects/science-in-the-age-of-ai/executive-summary/).

**What this vector does not address.** None of its members has built a systematic methodology with foundation→evidence→guidelines structure. The position exists as essays, books, talks, and editorial warnings — not as a constructed methodology artifact. This is the vector the repo's own niche sits closest to; the construction itself appears to be open.

---

### Vector 4 — Governance / disclosure / cautionary

**One-line.** The frame is what AI must not do, what must be disclosed, and what infrastructure must precede AI integration — not how AI should be used.

**What research looks like in practice.** AI use is permitted but disclosed in Methods sections or cover letters. AI cannot be an author; humans are accountable. In Science, AI output cannot be used directly as manuscript text. Funders invest in data standards and workforce training before backing methodology prescriptions. Critics flag specific tasks (hypothesis generation, peer review) as inappropriate for current AI.

**Tools and infrastructure.** Editorial policies (Nature, Science, journal-specific guidelines), open-data standards (Bridge2AI), funding mechanisms (NSF AI Institutes, NAIRR), critique venues (Bender's *The AI Con*, Marcus's Substack).

**Players and evidence.**

- **Nature** — AI cannot be an author; all non-trivial AI use must be disclosed in Methods. Policy established 2023, current as of 2026. Source: [Nature editorial policies on AI](https://www.nature.com/nature-portfolio/editorial-policies/ai) (verified via [policy summary](https://manusights.com/blog/nature-ai-policy)).
- **Science** — slightly stricter: AI output cannot be used directly as manuscript text; disclosure in cover letter and methods/acknowledgments. Source: [Science journals editorial policies](https://www.science.org/content/page/science-journals-editorial-policies).
- **Emily Bender** — hypothesis generation requires human experience and bias-awareness LLMs lack; "best left to humans." *The AI Con* (Bender & Hanna, 2025) extends to research contexts. Reference: [Stochastic Parrots paper page](https://faculty.washington.edu/ebender/stochasticparrots.html).
- **Gary Marcus** — reliability skepticism (hallucinations, no world models) applied to high-stakes research; general critique rather than research-specific methodology prescription. Source: [Marcus on AI Substack](https://garymarcus.substack.com/).
- **NIH Bridge2AI** — data infrastructure and workforce training are positioned as prerequisites to trustworthy AI in biomedical research. Source: [commonfund.nih.gov/bridge2ai](https://commonfund.nih.gov/bridge2ai).
- **NSF AI Institutes** — "human-AI collaboration" is a programmatic theme; NAIRR provides compute and training access. Funding-programmatic, not methodology-prescriptive. Source: [nsf.gov/focus-areas/ai/institutes](https://www.nsf.gov/focus-areas/ai/institutes).

**What this vector does not address.** A positive methodology for how AI should be used. The frame is rules of the road, not a way of driving.

---

### Vector 5 — Silence

**One-line.** Several institutions that have natural authority to opine on research methodology with AI have not staked public positions.

**What this looks like in practice.** Researchers working in open-science / replication / preregistration cultures operate without explicit community guidance on AI tools. Existing open-science infrastructure (the Open Science Framework, TOP guidelines, preregistration templates) has not been updated to address AI-assisted analyses. Individual practice fills the gap, idiosyncratically.

**Players and evidence.**

- **Brian Nosek / Center for Open Science** — no public position found on AI in research methodology as of May 2026. The TOP 2025 update (September 2024) addresses analytic transparency and preregistration but does not mention AI tool disclosure or AI's effect on replication. Source: [COS blog — TOP 2025](https://www.cos.io/blog/new-preprint-introduces-major-update-to-the-top-guidelines).
- **Stanford HAI** — output is descriptive measurement (the AI Index report); no found prescription on how researchers should work with AI. Source: [hai.stanford.edu/research/ai-index-report](https://hai.stanford.edu/research/ai-index-report).
- **Allen Institute for AI (Ai2)** — augmentation framing inferred from product design (OpenScholar, ScholarQA, Asta, Paper Finder); no published methodology manifesto found. Source: [allenai.org/ai-for-science](https://allenai.org/ai-for-science).

**What absence here means.** Not necessarily that no position exists privately or is in draft; only that public canvassing did not find one. This is a step-0-level finding and should be re-verified before the foundation treats the silence as a durable fact. The metascience silence in particular (COS / Nosek) is the most consequential — the open-science community is the natural home for methodological norms on AI in research, and its absence leaves the question open.

---

## 4. Cross-cutting observations

**Convergence.** Three things every player who takes a stance agrees on: AI is changing what is possible in research; outputs must remain attributable to humans (governance camp's bedrock); speed gains are real (delegation camp's bedrock). Augmentation is the rhetorical default — almost every player uses augmentation language even when the architecture they describe is delegation.

**Divergence.** Where execution should sit (with AI agentically — Vector 1; with the human using AI as instrument — Vectors 2 and 3). Whether the human's role is durable (frontier labs imply temporary; craft camp implies permanent; governance camp implies regulated). Whether AI hypothesis generation is methodologically respectable (DeepMind and Sakana yes; Bender and Royal Society skeptical).

**What no player is claiming.** That AI use should be evaluated on whether it grows the researcher, rather than on whether it produces outputs. Skill formation appears as a *warning* (Mollick, Anthropic internal, Royal Society) — never as a *positive design criterion*. The repo's "empower, not replace" stance in its explicit positive form has no direct claimant among the twenty entities canvassed.

**The taxonomy is asymmetric.** Vectors 1 and 4 dominate by player count (frontier labs are well-resourced and loud; governance bodies are well-organized and have venues). Vector 2 is mid-sized. Vector 3 has the fewest players. Vector 5 is the most surprising.

## 5. Limitations of step 0

- **Twenty entities is a sample, not a census.** Things were missed. The canvass should be widened in later stages, especially in domains adjacent to the repo's question (HCI augmentation lineage, cognitive psychology of skill formation, history-of-science accounts of past tool transitions).
- **URLs were subagent-verified at time of fetch; nothing here is citation-grade until re-verified.** Any source that earns its way into the foundation or methodology needs to flow through `add-evidence` with its own check.
- **"No explicit position found" is a step-0 finding, not a durable absence.** Particularly for COS / Nosek, the silence should be re-checked at depth before the foundation leans on it.
- **Public positioning is what an entity *says* it does.** The gap between that and what working researchers actually do is what `evidence/interviews/`, `experiments/`, and `observations/` are for — step 0 does not substitute for them.
- **A snapshot from May 2026.** The frontier-lab positions in particular shift on a months-scale; treating these as durable would be a mistake.

## 6. What this surfaces for deeper investigation

In rough priority order, for the survey's Stage 3:

1. **Elicit's methodology writings in depth.** "Supervise the process, not the output" is the closest operational cousin to "empower, not replace." A literature-note-grade read of Stuhlmüller and Byun's writing, and of Elicit's blog over time, is high priority.
2. **The empirical literature on AI and skill formation.** The Anthropic coding-skills study (already in [reading-list.md](../reading-list.md)) is one data point. The broader literature — cognitive psychology of skill, related studies in education, chess, and other domains where AI tutors have been studied — almost certainly exists and is not yet in the foundation. This is the empirical anchor cluster V needs more of.
3. **The centaur / cyborg vocabulary's lineage.** Kasparov's original framing → Mollick's adaptation → current usage in research contexts. The repo currently uses neither term. Stage 3 should produce a decision: adopt, refine, or contest.
4. **Whether the metascience silence is real.** Re-check whether anyone in the COS / Nosek / Ioannidis / Royal Society / preregistration world has staked a position the canvass missed. If the silence holds, decide whether the repo should address it explicitly or expect it to be filled.
5. **The frontier-lab consensus on speed-as-the-primary-good.** This is the closest the field has to a foil for the repo's stance. The foundation could sharpen its argument by naming the contrasted position explicitly — "empower, not replace" reads differently when the position being contrasted is named.

## 7. Sources canvassed (full list)

URLs verified at time of subagent fetch, 2026-05-16. Not re-verified.

**Frontier labs and autonomous-research systems:**

- [Anthropic — AI for Science Program](https://www.anthropic.com/news/ai-for-science-program)
- [Anthropic — Automated Weak-to-Strong Researcher (alignment, 2026)](https://alignment.anthropic.com/2026/automated-w2s-researcher/)
- [OpenAI — Introducing Deep Research](https://openai.com/index/introducing-deep-research/)
- [TechCrunch — Altman on 2028 researcher (October 2025)](https://techcrunch.com/2025/10/28/sam-altman-says-openai-will-have-a-legitimate-ai-researcher-by-2028/)
- [Hassabis — IAS talk on the future of knowledge (May 2025)](https://blog.biocomm.ai/2025/06/05/sir-demis-hassabis-on-the-future-of-knowledge-institute-for-advanced-study/)
- [Hassabis — Fortune interview (February 2026)](https://fortune.com/2026/02/11/demis-hassabis-nobel-google-deepmind-predicts-ai-renaissance-radical-abundance/)
- [Google DeepMind — AI co-scientist paper (arXiv 2502.18864)](https://arxiv.org/abs/2502.18864)
- [FutureHouse — About](https://www.futurehouse.org/about)
- [FutureHouse — Robin announcement](https://www.futurehouse.org/research-announcements/demonstrating-end-to-end-scientific-discovery-with-robin-a-multi-agent-system)
- [Sakana — AI Scientist in Nature (March 2026)](https://sakana.ai/ai-scientist-nature/)
- [Beel et al. — Evaluating Sakana's AI Scientist (arXiv 2502.14297)](https://arxiv.org/abs/2502.14297)

**Augmentation tools and individual voices:**

- [Elicit — Supervise the Process of AI Research (Latent Space)](https://www.latent.space/p/elicit)
- [NotebookLM](https://notebooklm.google/)
- [ResearchRabbit — Boosting Research Productivity](https://www.researchrabbit.ai/articles/boosting-research-productivity-with-researchrabbit)
- [Perplexity — Introducing Deep Research](https://www.perplexity.ai/hub/blog/introducing-perplexity-deep-research)
- [Ethan Mollick — Centaurs and Cyborgs (September 2023)](https://www.oneusefulthing.org/p/centaurs-and-cyborgs-on-the-jagged)
- [Andrej Karpathy — Software Is Changing Again (June 2025)](https://singjupost.com/andrej-karpathy-software-is-changing-again/)
- [Simon Willison — How I use LLMs to help me write code (March 2025)](https://simonwillison.net/2025/Mar/11/using-llms-for-code/)

**Institutions, metascience, critics, venues:**

- [Stanford HAI — AI Index Report](https://hai.stanford.edu/research/ai-index-report)
- [Ai2 — AI for Science](https://allenai.org/ai-for-science)
- [Royal Society — Science in the Age of AI (May 2024)](https://royalsociety.org/news-resources/projects/science-in-the-age-of-ai/executive-summary/)
- [NSF AI Institutes](https://www.nsf.gov/focus-areas/ai/institutes)
- [NIH Bridge2AI](https://commonfund.nih.gov/bridge2ai)
- [Center for Open Science — TOP 2025 update (no AI provision)](https://www.cos.io/blog/new-preprint-introduces-major-update-to-the-top-guidelines)
- [Emily Bender — Stochastic Parrots page](https://faculty.washington.edu/ebender/stochasticparrots.html)
- [Gary Marcus — Marcus on AI Substack](https://garymarcus.substack.com/)
- [Nature — editorial policy on AI (summary)](https://manusights.com/blog/nature-ai-policy)
- [Science — journals editorial policies](https://www.science.org/content/page/science-journals-editorial-policies)
