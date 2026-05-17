# GOAL.md introduced; repo aligned to the charter (2026-05-17)

A new top-level document, `GOAL.md`, was drafted and accepted as the repo's primary document — the charter against which the rest of the repo aligns. The foundation, methodology, READMEs, and operating principles were then revised so that everything points to the charter and reflects its current framing. This entry records the full scope.

## What prompted it

Two threads converged. (a) Methodology infrastructure from the maintainer's other repo (a `progress` skill + cross-machine usage tracking) was being merged onto this machine; the question of whether to import that skill led to a wider conversation about how autonomous work should advance the repo, and to the realization that `/progress`'s divergence-convergence pattern (designed for the maintainer's research-engine repo) did not fit this repo's evidence-driven rhythm. (b) Out of that, the right artifact for this repo was identified as a skill-agnostic charter: `GOAL.md`, the primary document of the repo, with everything else aligning to it rather than the other way around.

Drafting `GOAL.md` surfaced two conceptual refinements that the existing foundation expressed less precisely:

- **AI slop vs. valuable outcomes.** The prior phrasing in `foundation/00-why-reimagine.md` §3 — "the output is real whether you develop the skill or not; the growth is not" — was misleading. It can be read as: unskilled use produces output equivalent to skilled use. The repo's actual position is that unskilled use produces *passable but qualitatively worse* output. The skill is what separates AI slop from work a researcher should be willing to put their name on. The optionality break is doubly bad: the unskilled researcher gets a worse output *and* gets no growth; the skilled one gets a better output *and* gets growth.
- **Whole-job framing of empower-not-replace.** The principle had been written as a question to ask "at every AI use." That framing creates a false expectation: it would forbid letting AI handle routine code syntax, citation formatting, or unit conversions, which is not what the methodology actually wants. The right framing applies the question at the level of the research job — the level it is actually judged on — not at every keystroke. Lower-level skills are a different category; their replacement is what frees attention for the work that compounds. The boundary between "fine to replace" and "must preserve" moves upward as AI improves, but the principle is stable.

Also surfaced as a trajectory caveat the foundation already had in parenthetical form: as AI improves, both floor and ceiling rise, the skill set itself shifts, and skill remains beneficial across the trajectory. The convergence scenario — where the floor catches the ceiling and even basic articulation/recognition skills stop mattering — would correspond to AI working without human involvement at all, and is explicitly out of scope for this repo.

## What changed

### New: `GOAL.md`

A new top-level document. Seven sections: Purpose, What changed about research, The call to action, The commitment, How the repo operates and why, What advancing the inquiry looks like, Status. Skill-agnostic (no Claude / autonomous-work vocabulary). Compressed; the foundation documents are the substantiated long-form.

### `foundation/00-why-reimagine.md` — substantive update

- **§3 (The break in the pattern)** — rewrote the paragraphs from "But — and this is the structural break" through the trajectory parenthetical. Substituted "passable" for "serviceable" to align with the AI-slop framing; added "usable enough to feel like progress, but qualitatively below what the same prompt would have produced in skilled hands." Replaced the problematic "output is real whether you develop the skill or not; the growth is not" line with: *the unskilled researcher gets a worse output and gets no growth; the skilled one gets a better output and gets growth. The default path is the worse one on both axes.* Expanded the trajectory caveat from a parenthetical into a full paragraph.
- **§7 (The response: empower, not replace)** — added the whole-job framing throughout. New paragraph stating the principle applies at the level of the whole job, not every micro-task; identifies what's preserved (framing questions, designing investigations, recognizing too-good results, taste, verification habits) vs. what's comfortably replaced (routine syntax, formatting, mechanical operations). Reframed the central question as: *will my capacity to do the research job, at the framing at which the job is judged, be greater as a result of this, or smaller?* Added the boundary-moves-with-AI clause.
- **§8 (What this repo is)** — added pointer to `../GOAL.md` as the compressed charter.

### `foundation/01-ai-attributes.md` — references updated

- **A16 (Output without reciprocal skill development)** — closing sentence updated to point to `../GOAL.md` §The commitment and §7 of `00-why-reimagine.md` (was §5; foundation/00's section numbering had shifted in the May 6 walk-through rewrite but the reference had not). Also reframed the methodological response from "make skill development a tracked output" to "make skill development *at the level the research job is judged on* a tracked output," consistent with the whole-job framing.
- **Cluster V intro** — corrected reference from `00` §2 to `00` §3 (post-rewrite, the structural break is in §3 not §2).

### `foundation/02-implications.md` — meta-frame reframed

- The "meta-frame: empower, not replace" section was reframed around the whole-job version of the question. Updated reference from `00` §5 to `../GOAL.md` and `00` §7. Added the explicit statement that the question is asked at the whole-job level, not every micro-task; routine operations are a different category. Added the boundary-moves-with-AI clause at the end.

### `foundation/03-open-questions.md` — Q10 sharpened

- Q10's title was "How does a researcher distinguish empowerment from replacement in the moment?" The whole-job framing partially answers this by saying not every AI use needs the test — only those whose output would be the substantive contribution of the moment. But two operational questions remain: how does the researcher reliably identify which uses cross that threshold, and how do they apply the empower/replace question well at that threshold? Q10 was rewritten to reflect both. The "what would resolve this" was also updated to specify observation across working sessions for *both* the threshold judgment and the empower/replace judgment at that threshold, with the explicit note that the threshold itself drifts upward as AI improves.

### `foundation/README.md` — charter pointer added

- Added explicit reference to `../GOAL.md` as the compressed charter. Updated the "if you have N minutes" reading guidance to include the five-minute charter read before the ten-minute foundation read.

### `methodology/guidelines.md` — G1 rewritten

- **G1** title changed from "Treat empower-vs-replace as a question to ask at every AI use" to "Apply the empower-vs-replace question at the level of the research job, not at every AI use." Practice section rewritten to specify the whole-job framing, the threshold of substantive contribution, and to clarify that routine operations are not the choices the methodology is built to police. Skill implication expanded to name *two* metacognitive capacities (recognizing the threshold + applying the question at it). Known costs updated to discuss threshold-judgment misjudgments in both directions and the upward drift of the threshold as AI improves. Reference updated from `foundation/00` §5 to `../GOAL.md` §The commitment + `foundation/00` §7. Last-reviewed date updated to 2026-05-17. Notes section now points to Q10 in `foundation/03-open-questions.md`.
- Guidelines G2–G15 left unchanged. They are operational practices whose content is compatible with the whole-job framing without rewording.

### `methodology/README.md` — guiding principle refined

- "Does this practice grow the researcher, or does it substitute for them?" → "Does this practice grow the researcher's capacity to do the research job at the level it is actually judged on, or does it substitute for that capacity?" Added the whole-job clause and the routine-operations exception. Added the boundary-moves-with-AI clause. Updated reference from `foundation/00-why-reimagine.md` §5 to `../GOAL.md` + `foundation/00-why-reimagine.md` §7.

### `README.md` (top-level) — central claim refined; charter added to navigation

- Central-claim paragraph: "useful output" → "passable output," with added clauses about the qualitative gap in skilled hands and the doubly-beneficial framing for skilled use. Empower-not-replace paragraph rewritten to add the whole-job framing and the routine-operations exception. Charter pointer added before the foundation pointer.
- "What's here" — `GOAL.md` added as the first item, ahead of `foundation/`.
- "Read first" — ladder restructured to five-minute charter read → ten-minute foundation/00 → thirty-minute walk → full picture.

### `CLAUDE.md` (top-level) — charter pointer added; discipline refined

- "What this repo is" — added explicit statement that `GOAL.md` is the charter, that CLAUDE.md serves the charter, and that conflicts are resolved in the charter's favor.
- **Discipline → "Empower over replace"** — rewritten to add the whole-job framing, the routine-operations exception, and to update references from `foundation/00-why-reimagine.md` §5 to `GOAL.md` §The commitment + `foundation/00-why-reimagine.md` §7.

## Files touched today

```
GOAL.md (new)
README.md
CLAUDE.md
foundation/README.md
foundation/00-why-reimagine.md
foundation/01-ai-attributes.md
foundation/02-implications.md
foundation/03-open-questions.md
methodology/README.md
methodology/guidelines.md
log/2026-05-17-goal-document-and-alignment.md (this entry)
```

## What is still open after today

- **The `CLAUDE.md` Status section is mildly stale** — it says "Five foundation documents (`00`–`04`)" but there are four (`00`–`03`) after the innovation deep-dive moved to `evidence/literature-notes/` on 2026-05-06. Not corrected today because it is unrelated to the GOAL-alignment work; flagged for a separate housekeeping pass.
- **G1's revision is itself proposed**, like the rest of the methodology. The change is conceptual cleanup rather than evidence-driven; it sharpens what G1 was already trying to say, but Q10 (now rewritten) flags that G1's reliable application in practice remains open.
- **The maintainer's other infrastructure** (cross-machine budget tracking, the `progress` skill from the research-engine repo) was installed at the user level on this machine alongside this work. That infrastructure is orthogonal to the repo's content and operates through `~/.claude/`, not the repo. The repo does not adopt `/progress`; if autonomous iteration is wanted in the future, the natural pattern is the built-in `/goal <condition>` orchestrating this repo's own four maintenance skills.
