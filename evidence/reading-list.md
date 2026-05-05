# Reading list

Annotated list of sources that shaped the foundation. The annotations describe what each source contributed — not a summary of the source. New entries are added as the inquiry encounters work that adds a non-trivial fact or framing.

---

## Primary

### Tao on Dwarkesh Patel — *How the world's top mathematician uses AI* (March 2026)

- [Dwarkesh's writeup](https://www.dwarkesh.com/p/terence-tao)
- [Podcast notes](https://podcastnotes.org/the-lunar-society-with-dwarkesh-patel/terence-tao-how-the-worlds-top-mathematician-uses-ai-dwarkesh-podcast/)
- [YouTube](https://www.youtube.com/watch?v=Q8Fkpi18QXU)

The single most useful source for this inquiry. Contributed:

- The "AI cannot make partial progress" framing — the climbing-handhold metaphor, and the corollary that each new session forgets everything. Foundational for cluster III.
- The 1–2% per-problem success rate against the visible Erdős wins — the cleanest articulation of publication bias in AI-for-research narratives.
- The "richer and broader, not deeper" observation — the cleanest statement of cluster I.
- The Lean / formal-verification framing of atomic checking — a verification primitive that does not depend on the generator. Foundational for the verification-first direction in `02-what-this-implies.md`.
- The serendipity-loss caution — that over-optimization can starve research of the inputs it needs.

### Beel, Kan, Baumgart — *Evaluating Sakana's AI Scientist* (arXiv 2502.14297, Feb 2025)

- [arXiv abstract](https://arxiv.org/abs/2502.14297)

Contributed:

- The 42% experiment-failure rate from coding errors — concrete number for "AI generates faster than it verifies."
- The "median 5 citations, mostly outdated" finding — concrete failure of AI-generated literature reviews.
- The "system cannot critically assess its own results" finding — empirical anchor for cluster II's self-validation attribute (A6).
- The framing of "papers that look like research without being research" — useful counter-example throughout.

### METR — *Measuring the Impact of Early-2025 AI on Experienced Open-Source Developer Productivity* (July 2025)

- [METR blog post](https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/)
- [Paper (arXiv 2507.09089)](https://arxiv.org/abs/2507.09089)

Contributed:

- The 19%-slower measurement against the 20%-faster perception — the entire empirical basis for cluster IV (perception gap).
- The methodology of randomized controlled trial on real tasks — model for what serious self-experimentation could look like in this repo's case studies.
- The follow-up update (Feb 2026) showing that for a subset of developers in a later study the effect may have shifted — useful as a reminder that A14 (capability ceiling moves) applies to the evidence base too.

---

## Cross-references — system-level builders

These sources are read primarily to know what this repo is *not* trying to be (system-scale agentic research), and secondarily to extract specific contributions.

### Wissner-Gross / Physical Superintelligence (PSI) / GPD (2026)

- [Physical Superintelligence (substack)](https://theinnermostloop.substack.com/p/physical-superintelligence)
- [Welcome to May 3, 2026 (GPD / LBNL replication, Erdős 1196)](https://theinnermostloop.substack.com/p/welcome-to-may-3-2026)

Contributed:

- The framing of replication as a verification primitive — LBNL's "flawless" replication of a 2023 condensed-matter paper using GPD. Independent of the generator; falls neither to self-validation nor to formal-verification's domain limits.
- The Erdős 1196 → ESS-conjecture chain as a partial counterexample to "AI cannot make partial progress" — and the reframing that the human is the carrier of cumulative state.

### FutureHouse — *Robin* end-to-end demonstration

- [Demonstrating end-to-end scientific discovery with Robin](https://www.futurehouse.org/research-announcements/demonstrating-end-to-end-scientific-discovery-with-robin-a-multi-agent-system)

Contributed:

- The clean factoring of Crow / Falcon / Owl / Phoenix / Finch agents — useful as an example of decomposition by capability, even though this repo is not building agents.
- The ripasudil-for-AMD result — concrete data point for AI hypothesis generation feeding into a real experimental result.
- The clear separation of "AI did the intellectual framework, humans did the wet lab" — useful framing.

### Google — *AI co-scientist*

- [Accelerating scientific breakthroughs with an AI co-scientist](https://research.google/blog/accelerating-scientific-breakthroughs-with-an-ai-co-scientist/)
- [Towards an AI co-scientist (arXiv 2502.18864)](https://arxiv.org/abs/2502.18864)

Contributed:

- The generate-debate-evolve hypothesis architecture — useful instance of the "produce many, select" pattern that cluster I implies.
- The Imperial antimicrobial-resistance reproduction — data point that cross-domain hypothesis generation (A2) is no longer hypothetical.

### OpenAI — *Deep Research*

- [Introducing deep research](https://openai.com/index/introducing-deep-research/)

Contributed:

- The capability profile (multi-step web research, structured citation) — useful baseline for what AI literature work can do today.
- The documented failures (outdated data, deference to less-reliable sources for corroboration) — empirical support for A8.

### Anthropic — *How scientists are using Claude*

- [How scientists are using Claude to accelerate research and discovery](https://www.anthropic.com/news/accelerating-scientific-research)

Contributed:

- The Biomni / Cheeseman / Lundberg case studies — concrete examples of researchers compressing month-scale workflows into hour-scale ones.
- The Cheeseman lab emphasis on confidence levels in findings — a methodological practice worth treating as evidence for a future guideline.
- The "encode the methodology as a skill" framing — relevant to how this repo's own skills are designed.

---

## Format note

When adding to this list, write what the source contributed in *terms the foundation can use*. "Interesting paper on AI" is not annotation. "This source documents X failure mode and gives a concrete percentage" is annotation.

A source belongs in this list when the foundation or methodology cites it or could cite it. A source that has not contributed to either does not belong here yet; if it is interesting reading material, keep it elsewhere until it has earned a citation.
