# Innovation document moved from foundation to evidence (2026-05-06)

A focused refactor following maintainer feedback. Recording the move and the substance preservation.

## What prompted it

The maintainer asked whether the innovation document fit naturally in the foundation folder. It did not. The other foundation files are normative — short, declarative claims and arguments. The innovation document was structurally different: a long literature synthesis (Campbell BVSR, March, Stanley, Sarasvathy) followed by application to AI. Its register did not match the rest of the foundation, and its substance partially duplicated what was already in `00-why-reimagine.md` §3 and `01-ai-attributes.md` cluster I.

The cleaner split: foundation contains normative claims (compactly stated); evidence contains the literature synthesis those claims rest on.

## What changed

### File move

- `foundation/02-innovation.md` → `evidence/literature-notes/innovation-as-different-operation.md` (with `git mv` to preserve history). A header was added to the file explaining its new role and pointing to where the foundation-level claims live.

### Foundation renumbering

With innovation no longer at slot 02, the rest of the foundation contracted:

- `foundation/03-implications.md` → `foundation/02-implications.md`
- `foundation/04-open-questions.md` → `foundation/03-open-questions.md`

Foundation now has four files (00-03) instead of five (00-04).

### Substance preservation in the foundation

The maintainer's instruction was that the ideas about innovation's uniqueness and nature must remain present in the foundation, not just in the literature note. Specific updates:

- **`foundation/00-why-reimagine.md` §3** was expanded from a one-paragraph compact statement to roughly four paragraphs covering: (a) the recombination/innovation distinction, (b) the convergent claim from the innovation literature that innovation = blind variation + retrospective selection, (c) the synthesis under the maintainer's framing of "smart diversification," (d) the consequence that AI is structurally a parallel exploitation engine more than a parallel exploration engine, biased toward its trained distribution rather than producing Campbell-blind variation, and (e) that AI cannot do retrospective selection because it lacks taste, so AI is at most a partial-fit collaborator for innovation work — useful as substrate but not as agent. The deeper literature synthesis is referenced as evidence.

- **`foundation/01-ai-attributes.md` A1** (breadth without depth) gained a paragraph on the deeper version of the claim: AI does not natively produce variation that is *blind* in Campbell's technical sense, which makes it a parallel exploitation engine more than a parallel exploration engine.

- **`foundation/01-ai-attributes.md` A4** (cheap idea generation) gained a nuance paragraph clarifying that cheap idea generation is not the same as cheap *innovation* — the volume of AI variation is high but the variation tends to cluster around existing modes, so the selection bottleneck and the innovation bottleneck are related but distinct.

- The open question `Q6` (can AI produce blind variation) was updated to point to the new locations of the foundation position rather than the old `02-innovation.md`.

### Cross-reference updates

All internal cross-references updated for the renumbering and move. Files touched: `foundation/00`, `foundation/01`, `foundation/02-implications.md`, `foundation/03-open-questions.md`, `foundation/README.md`, `methodology/guidelines.md`, `.claude/skills/update-foundation/SKILL.md`, `README.md` (top-level), `evidence/README.md`, `evidence/reading-list.md`. The literature note itself uses `../../foundation/...` paths for its outbound references.

### README updates

- `foundation/README.md` rewritten with a four-file reading table and an explicit "where the innovation deep-dive lives now" section explaining the move.
- `evidence/README.md` gained an entry for `literature-notes/` describing what it is for.
- `evidence/reading-list.md`'s "Innovation literature" section updated to point to the literature note as the synthesis location.
- Top-level `README.md` updated to reflect four foundation documents instead of five and to point at the literature note.

## What is preserved, in summary

The reader who lands on the foundation now finds:

- In `00-why-reimagine.md` §3: the claim that innovation is qualitatively different from recombination, the structural framework for it (variation + selection, with variation that is not goal-directed), the working synthesis (smart diversification), the AI-specific consequence (parallel exploitation engine, not exploration engine), and the partial-fit conclusion.
- In `01-ai-attributes.md` A1: the deeper version of breadth-without-depth, framed in terms of Campbell's blind variation.
- In `01-ai-attributes.md` A4: the nuance that cheap idea generation is not cheap innovation.
- In `03-open-questions.md` Q6, Q7, Q8: the innovation-specific open questions — whether AI can produce blind variation, what selective retention looks like solo, how to resist March's drift.

What lives only in the literature note is the detailed synthesis of the four lines of work — the sentences explaining what BVSR is, what March's empirical finding was, how Stanley's novelty search relates, what Sarasvathy's effectuation pattern is. That material is supportive, not normative, and belongs in evidence.

## Net effect

Foundation reads as a coherent set of claims at the same register. The literature synthesis is preserved as evidence and discoverable through the foundation's pointers and the evidence README. The substance the maintainer wanted preserved — the uniqueness of innovation, its structure, AI's specific mismatch to it — is present in the foundation in compact form, with the longer treatment one click away.

## Files touched

```
foundation/00-why-reimagine.md           (§3 expanded; cross-refs updated; footer revised)
foundation/01-ai-attributes.md           (A1 deepened; A4 nuance added; cross-refs updated)
foundation/02-implications.md            (renamed from 03; cross-refs updated)
foundation/03-open-questions.md          (renamed from 04; Q6 reference updated)
foundation/README.md                     (rewritten for four-file structure)
evidence/literature-notes/innovation-as-different-operation.md  (moved from foundation/02-innovation.md; header added; cross-refs updated)
evidence/README.md                       (added literature-notes/ entry)
evidence/reading-list.md                 (Innovation literature section updated)
methodology/guidelines.md                (cross-refs updated)
.claude/skills/update-foundation/SKILL.md (file list updated)
README.md                                (top-level; foundation count, reading order, reference to lit note)
log/2026-05-06-innovation-doc-moved-to-evidence.md  (this entry)
```
