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

The current foundation position (`02-innovation.md`) is that AI's "novelty" is biased toward the trained distribution — fluent recombination, not blindness in BVSR's sense. Stanley's Open-Endedness research at OpenAI is the active line attempting to address this. The answer is not settled.

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

### Q10: How does a researcher distinguish empowerment from replacement in the moment?

The mindset shift in `00-why-reimagine.md` §5 — empower, not replace — is the methodology's central principle. But the boundary between empowering use of AI and replacing use of AI is not always obvious in the moment of choice. The same prompt can be empowering or replacing depending on what the researcher does with the output, what they would have done without it, and which practices they are skipping. Without a clearer way to recognize the difference at the point of choice, the methodology asks researchers to apply a principle they cannot reliably apply.

**What would resolve this:** observation across many real working sessions, with the researcher noting in real time whether each AI use felt empowering or replacing, and reviewing those notes weeks later to see whether the in-the-moment judgment held up. Patterns may emerge that can be operationalized into recognizable signals. Until they do, the methodology has to lean on coarse heuristics (e.g., "did I learn something I didn't know?", "could I reproduce this without AI in six months?").

### Q11: How should the methodology track researcher development?

`00-why-reimagine.md` §3 names the researcher's growing competence as a primary output of research, and `01-ai-attributes.md` A16 explains why AI specifically endangers it. But measuring development is hard. Skills compound on long timescales; atrophy is invisible until needed; the researcher is a poor judge of their own current capability (cluster IV). The methodology has to track the second output, but how is open.

**What would resolve this:** experiment with several candidate practices — periodic skills audits ("can I still do X by hand?"), capability journals (what was hard a month ago, what is easy now), structured replication of past work (re-doing one's own work without AI to see what skills remain) — and observe which produce useful signal without consuming so much attention that they undermine the development they aim to track.

### Q12: Does empower-not-replace generalize across research domains?

The framing assumes research tasks resist clean decomposition (A17) and that researcher development is a primary output. Both are likely true across most research, but the *strength* of each may vary. Some experimental domains may have task structures that genuinely separate cleanly (e.g., AI generates protocols, the human runs the experiment). Some pure-theory domains may have research where development happens almost entirely outside AI-touched work. The mindset's universality is open.

**What would resolve this:** comparing observations across at least three distinct research domains. If the empower/replace question lands the same way in physics, biology, and computer science, the framing generalizes. If different domains have categorically different relationships to the question, the methodology may need domain-specific instantiations.

---

## Resolved

*(none yet)*
