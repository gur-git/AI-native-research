# Innovation added as a distinct operation in the foundation (2026-05-05)

The foundation gained a new dimension today. Recording the shift, the reasoning, and what changed.

## What prompted it

In conversation, the maintainer pushed back on the framing in `00-why-reimagine.md` that treats "production" as a single operation whose cost has fallen. Their point: producing a draft is at least two qualitatively different operations — recombination of known elements, and innovation that extends or escapes the known distribution. Innovation is "more than randomness applied to recombination" and deserves its own treatment. As the conversation developed, it became clear the topic was substantial enough for a dedicated foundation document, *and* needed acknowledgment in the central diagnostic claim of `00`.

## What was read

Four lines of innovation literature were surveyed at the abstract-and-overview level:

- **Campbell's BVSR (Blind Variation and Selective Retention).** The 1960 foundational claim that creative thought operates through blind variation followed by retrospective selection, with Simonton's 2011/2022 typological refinements (rational/irrational/blind, only blind associated with knowledge production).
- **March (1991) — Exploration vs. Exploitation.** The warning that organizations following short-term gradients drift toward exploitation and become "effective in the short run but self-destructive in the long run." Directly relevant because AI sharpens the exploitation gradient.
- **Lehman & Stanley (2011) — Novelty Search.** "As soon as you create an objective, you ruin your ability to reach it." Active line of AI research (Stanley now leads OpenAI's Open-Endedness team) attempting to address whether AI can produce blind variation.
- **Sarasvathy — Effectuation.** The means-driven vs. goal-driven distinction in entrepreneurship; same structural claim about emergent direction in different vocabulary.

The four converge on: innovation = (variation not directed by the goal) + (selection that is retrospective and aggregate). All four are now in [`evidence/reading-list.md`](../evidence/reading-list.md).

## Maintainer's synthesis (developed in conversation)

Innovation is "smart diversification" — diversification that is effective in aggregate even when individual variants fail. Taste is necessary because innovation must eventually progress a cause; otherwise it is blind in the wrong sense (random walk). But taste must be applied retrospectively to a wide enough set of variants, because goal-directed search converges to dead-ends. The other "qualities" of innovation (committed depth, negative-space recognition, recognition-over-generation) are best framed as *techniques for producing smart diversification*, not as separate qualities.

This synthesis is captured in `04-innovation.md` section 2, and informs section 4's gestures at methodological consequences.

## What changed in the foundation

### Foundation update

- **`foundation/00-why-reimagine.md`** — Section 2 added: "But production is not a single operation." Splits production into recombination (where the cost-structure inversion in section 1 holds) and innovation (where it does not hold cleanly). Old section 2 (research as particular case) renumbered to section 3, with a new paragraph noting that research is innovation-heavy in a way most knowledge work is not. Old section 3 renumbered to section 4. Last-revised footnote updated.
- **`foundation/04-innovation.md`** — New document. The deeper standalone treatment. Six sections: literature review, the inquiry's working synthesis, AI's role in innovation, methodological consequences (gestures), open questions, status with caveats. Longer than 00 and 01 because both literature and synthesis need air.
- **`foundation/README.md`** — Updated to describe 04 and the recombination/innovation distinction in 00.
- **`foundation/03-open-questions.md`** — Four new open questions added (Q6–Q9): can AI produce blind variation, what does selective retention look like for solo researchers, how to resist March's drift, and is the methodology biased toward defense.

### Reading list

- **`evidence/reading-list.md`** — New section "Innovation literature" with four entries (Campbell BVSR, March exploration/exploitation, Lehman & Stanley novelty search, Sarasvathy effectuation). Each entry annotates what the source contributed to the foundation, in the same shape as existing entries.

## Why this matters for the inquiry

The pre-update foundation was correct about recombination work and silent about innovation. The methodology that would have grown from it — verification-first, selection-heavy, portfolio over single-thread — is a methodology for the recombination half of research. Research is, at its core, an innovation discipline. A methodology that addresses only recombination is one that improves the routine work and fails to engage the part of research that matters most.

The post-update foundation acknowledges this asymmetry and creates a place (`04-innovation.md`) where the innovation half can be developed alongside, with its own evidence trail, its own open questions, and — eventually — its own guidelines.

## What is still open

This is the inquiry's first substantive treatment of innovation, and the literature has been read at the abstract-and-overview level rather than fully digested. Particular caveats:

- The four-line reading is selective. Boden, Kauffman, Simon, Polanyi, Schumpeter all have relevant work that has not been engaged.
- The mapping from innovation literature to AI methodology is the inquiry's own work, not established. Whether AI's bias toward the trained distribution maps cleanly onto Campbell's "rational variation" is a claim to be tested, not a finding.
- Q9 specifically — "is the methodology biased toward defense?" — is the most uncomfortable question of the four added today, and the most likely to drive substantive further revision.

## Files touched today (this log entry's scope)

- `foundation/00-why-reimagine.md` (edit)
- `foundation/04-innovation.md` (new)
- `foundation/README.md` (edit)
- `foundation/03-open-questions.md` (edit, four questions added)
- `evidence/reading-list.md` (edit, innovation literature section added)
