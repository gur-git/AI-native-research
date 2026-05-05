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

---

## Resolved

*(none yet)*
