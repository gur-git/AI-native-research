# Open questions

Questions the foundation does not yet have a settled view on. Each entry includes what would resolve it.

When evidence resolves a question, it gets moved to a "resolved" section at the bottom (kept for the record), and the foundation gets updated via `update-foundation`. New questions are added when the inquiry surfaces them.

---

## Open

### Q1: Which attributes really are structural, and which are temporary?

The current tagging in `01-ai-attributes.md` is the inquiry's best read as of the foundation's first draft. Several attributes are tagged `ambiguous` because the answer depends on how AI capabilities evolve. The honest position is that the tagging is a working hypothesis, not a finding.

**What would resolve this:** observation across model generations. Specifically, tracking whether a given attribute remains a binding constraint across, say, three frontier-model releases. A `temporary` attribute that is still binding three releases later should be retagged `structural`.

### Q2: Does the cluster I framing — "selection is the new bottleneck" — actually match how researchers experience their work?

The framing is plausible from the technology side, but it is not yet grounded in observation of researchers actually doing AI-native work. It might be that selection is *one* new bottleneck among several, or that the bottleneck shifts depending on the phase of a project.

**What would resolve this:** interviews with researchers who have done at least 6 months of serious AI-assisted work, asking specifically about where their bottlenecks now sit and whether they feel different from their pre-AI bottlenecks.

### Q3: Is "external cognition" — version-controlled, re-loadable project state — actually a discipline that scales, or does it become its own friction?

The argument is that a researcher's cumulative state must live in files, because AI sessions don't carry it. But maintaining that state has a cost. It might be that the cost is high enough that researchers in practice abandon it, even when it would help.

**What would resolve this:** structured self-experiments where a researcher maintains an external state file for one project and not for a comparable one, with honest reporting of friction and benefit. n=1 to start, then potentially extended.

### Q4: Does the methodology generalize across research domains, or are the structural attributes dominated in practice by domain-specific failure modes?

The four-cluster framing in `01-ai-attributes.md` is meant to be domain-agnostic. But it is possible that, in practice, the dominant failure modes in (say) experimental biology are different enough from those in theoretical physics that the methodology needs domain-specific instantiations.

**What would resolve this:** comparing observations and interviews across at least three distinct research domains. If the same patterns recur, the methodology generalizes. If different domains hit different walls, the foundation needs a more careful treatment of domain dependence.

### Q5: Is replication-as-verification practical for individual researchers, or does it remain a system-scale capability (à la PSI / GPD)?

Wissner-Gross's GPD suggests that AI can replicate published work end-to-end as a verification primitive. But that demonstration was at LBNL with significant infrastructure. Whether an individual researcher can adopt "replicate a recent paper" as a regular practice is open.

**What would resolve this:** a structured trial — pick three recent papers in a known area, attempt AI-assisted replication, log what happens, what breaks, what it cost.

### Q6: Can AI produce variation that is genuinely blind in Campbell's sense, or is its bias toward the trained distribution a structural ceiling?

The current foundation position (`04-innovation.md`) is that AI's "novelty" is biased toward the trained distribution — fluent recombination, not blindness in BVSR's sense. Stanley's Open-Endedness research at OpenAI is the active line attempting to address this. The answer is not settled.

**What would resolve this:** observation across model generations of whether outputs framed as "novel" cluster near training-distribution modes, or genuinely escape them. Likely requires testing with frontier models specifically trained or prompted for open-ended search, not general-purpose chat models. Stanley's published work is the place to track progress.

### Q7: What does selective retention look like for an individual researcher with no team?

The classic accounts of taste (Campbell, March, Sarasvathy implicitly) assume a research-group culture — postdocs, advisors, peer review at the bench — that produces the social pressure that performs selective retention. Most early-career researchers do not have full access to this culture, and AI does not substitute for it. How an individual researcher develops and exercises taste in this regime is open.

**What would resolve this:** observation of researchers (the maintainer included) who maintain explicit direction-and-outcome logs over a year or more, with retrospective analysis of which directions paid off and what signals at the time predicted that. This is a long-horizon question; partial answers will accumulate before a full one is possible.

### Q8: How does the methodology resist March's drift toward exploitation when AI specifically makes exploitation cheaper?

March's warning is that organizations follow gradients, and AI sharpens the gradient toward exploitation. A methodology that does not deliberately maintain the exploration share will drift, even if the researcher believes it is doing innovative work. Whether the response is cultural (peer commitment, public exploration logs) or technical (workflow design, time allocation) or both is open.

**What would resolve this:** structured self-experiments where the researcher tracks the share of working time spent on exploitation vs exploration, with deliberate interventions (e.g., enforced exploration days) and honest measurement of whether the interventions hold against the gradient.

### Q9: Is the methodology biased toward defense?

The foundation as written is heavily focused on what can go wrong with AI in research — failure modes, perception gaps, verification needs. The generative side — what kinds of research become newly feasible because AI exists — is underdeveloped. Whether this is the right balance, or an artifact of the source material's defensive posture, is open.

**What would resolve this:** observation of what kinds of research projects the maintainer (or other researchers) actually start in this regime that would not have been feasible before, and whether the foundation's framing suppresses or supports them. Likely requires the pilot research project to surface this question concretely.

---

## Resolved

*(none yet)*
