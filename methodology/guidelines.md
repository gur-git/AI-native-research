# Methodology guidelines

Accumulated practices the inquiry proposes, is testing, or has adopted. Each guideline traces to the foundation attribute(s) it addresses, the evidence that motivated it, and an explicit *skill implication* — the capacity the practice is meant to develop or preserve in the researcher. The skill-implication field is not optional; a guideline that cannot say what skill it builds is one that risks substituting for skill, and the methodology's central principle (`foundation/00-why-reimagine.md` §7: empower, not replace) cannot tolerate that.

G1–G15 are first-pass drafts derived from the foundation as written through 2026-05-06; later guidelines arrive as evidence accumulates (G16–G19, from the first professor interview and the first pilot audit, 2026-06-10). All are at status `proposed`; none rest on systematic evidence yet. Promotion to `testing` requires deliberate trial; promotion to `adopted` requires evidence that the trial worked. Use the [`add-guideline`](../.claude/skills/add-guideline/SKILL.md) skill for additions and the [`update-foundation`](../.claude/skills/update-foundation/SKILL.md) skill when status changes.

---

## Schema

Every guideline takes this shape:

```markdown
## G{N}: <Name>

**Status:** proposed | testing | adopted | retired (last reviewed YYYY-MM-DD)
**Addresses attribute(s):** N, N
**Evidence trail:** [file](../evidence/...), [file](../evidence/...)
**Skill implication:** <what capacity does this practice develop, preserve, or risk substituting?>

### Practice

<step-level description of what the researcher actually does>

### What success looks like

<observable outcome — how you know this guideline is helping>

### Known costs

<honest accounting of friction, time, attention this guideline asks for>

### Notes

<edge cases, related guidelines, things already learned not to do>
```

Numbers are sequential and never reused, even when guidelines are retired.

---

## Active guidelines

### G1: Apply the empower-vs-replace question at the level of the research job, not at every AI use

**Status:** proposed (last reviewed 2026-05-17)
**Addresses attribute(s):** A16, A17 (cluster V)
**Evidence trail:** Derived from `../GOAL.md` §The commitment and `foundation/00-why-reimagine.md` §7, the central commitment of the inquiry.
**Skill implication:** Develops two metacognitive capacities. *First*, recognizing which AI uses cross into the territory where the empower/replace question matters — uses whose output would be the substantive contribution at the level the research job is judged on. *Second*, applying the question well at that level. This is the load-bearing skill of the entire methodology; without it, all other guidelines drift toward replacement under the gradient.

#### Practice

The question to ask is at the level of the whole research job, not every keystroke: *will my capacity to do the research job — at the framing at which the job is judged — be greater as a result of how I use AI here, or smaller?* Routine syntax, formatting, unit conversions, and similar low-level operations can be handled by AI without invoking the test; these are not the choices the methodology is built to police.

The threshold for applying the question is whether AI's output would be the substantive contribution of the moment. When yes, pause and ask. The answer is rarely "yes" or "no" — it is usually "yes if I do X, no if I just accept the output." Note the X. Coarse heuristics that help when the question feels uncertain: *did I learn something I didn't know? Could I reproduce this without AI in six months? Am I skipping a practice I would benefit from doing?*

The pause does not have to be elaborate. It needs to be habitual at the right level. The point is to make the empower/replace question visible at the choices that matter, not after the choices have compounded into atrophy.

#### What success looks like

Over time, the researcher can articulate two things: which kinds of AI uses cross the threshold in their work, and which of those threshold-crossing uses have reliably been empowering versus replacing. The articulation should be specific to the kind of work — "AI for literature scans empowers me when I cross-check claims against sources; replaces me when I summarize without reading."

#### Known costs

The threshold judgment itself adds friction at the beginning, until the researcher's pattern-recognition for "this is a substantive-contribution moment" becomes habitual. Misjudgments in both directions are common: pausing on micro-tasks (over-applies), and not pausing on substantive moments because they didn't feel substantive at the time (under-applies). Both decrease with practice. The threshold also shifts as AI improves: what counts as substantive contribution today may be routine in two years, and the practice has to track that drift.

#### Notes

This is the meta-guideline. Other guidelines below are specific operationalizations of empower-not-replace in particular contexts. Open question Q10 in `foundation/03-open-questions.md` tracks the operational difficulty of applying this guideline reliably — both the threshold judgment and the empower/replace judgment at that threshold.

---

### G2: Maintain external project state in version-controlled files

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A10, A11 (cluster III)
**Evidence trail:** `evidence/reading-list.md` — Tao on Dwarkesh ("AI has forgotten everything it just did").
**Skill implication:** Develops the craft of deciding what to log and at what grain — a skill that compounds because the logs become more useful as the researcher gets better at writing them. The state file is also what allows the human to remain the carrier of cumulative state, which is the methodology's response to AI's session forgetting.

#### Practice

Maintain a markdown file per project containing the current question, constraints, assumptions, decided directions, dead ends, and open threads. Update it at the start and end of working sessions. Re-load relevant parts of it into AI sessions as context. Treat the file as the project's source of truth, not the chat history.

#### What success looks like

A new AI session, given the project state file, can be productively grounded in five minutes. The researcher's own re-orientation after a week away takes minutes, not hours. The file accumulates rather than fragments.

#### Known costs

Maintenance overhead. The file goes stale if the discipline lapses, and stale files are worse than no files because they mislead. Probably 10–20 minutes per working day in the steady state.

#### Notes

The Tao reference is about math specifically; the practice generalizes because the underlying attribute (session forgetting) is general. This is open question Q3 in `foundation/03-open-questions.md` — whether the discipline scales without becoming its own friction.

---

### G3: Verify AI output from a different source than the one that generated it

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A6, A8, A9 (cluster II)
**Evidence trail:** `evidence/reading-list.md` — Beel/Kan/Baumgart Sakana evaluation (42% experiment failure, hallucinated numerical results, system "cannot critically assess its own results"); Tao on Lean as atomic verification; Wissner-Gross GPD on replication.
**Skill implication:** Develops three distinct verification skills depending on which mode is used: formalization (when verifying with formal tools like Lean or type systems), replication (when re-deriving a third party's published result), and critical reading (when human-reviewing). All three compound; none of them develop if the researcher accepts AI output without verification.

#### Practice

For any AI output the researcher will rely on substantively, choose at least one verification mode whose source is independent from the generation:

- **Formal tools.** Push the result through a checker that does not know it came from AI — a type system, a deterministic simulator, a formal proof checker.
- **Third-party replication.** For an AI-derived result, attempt to re-derive it from independent ground (a different paper, a different dataset, a different tool).
- **Human review.** A colleague who has not seen the AI session reads the output cold; or, in solo work, the researcher returns to the output a day later with a deliberately critical posture.

Choose the mode appropriate to the stakes and the domain. The choice is itself a practice that develops with use.

#### What success looks like

The researcher can name, for each substantive AI-assisted output in their work, which verification mode was applied. Outputs without a verification trail do not ship.

#### Known costs

Verification often costs more than the AI-assisted generation itself. This is the point of the verifiability gap (A9). The methodology accepts this cost as the price of trusting the output.

#### Notes

This guideline is what makes the cluster II diagnosis actionable. Without it, AI's "cannot critically assess its own results" remains diagnosis without prescription.

---

### G4: Distinguish recombination work from innovation work; apply different practices to each

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A1, A4 (cluster I)
**Evidence trail:** `evidence/literature-notes/innovation-as-different-operation.md`; reading-list entries on Campbell BVSR, March, Stanley, Sarasvathy.
**Skill implication:** Develops the metacognitive capacity to recognize, in the moment, which kind of operation a task is — recombination of known elements, or innovation that requires variation outside the known distribution. This recognition is itself a research skill that AI cannot supply; the practice of asking the question at every task is what builds it.

#### Practice

Before starting any non-trivial task, classify it: *is this recombination work (assembling known elements into a fluent output) or innovation work (producing something the trained distribution does not contain)?* For recombination, AI is well-suited as a parallel production engine; verification (G3) is the dominant concern. For innovation, AI is a partial-fit substrate at best; the dominant concerns are protected depth, exposure to negative space, and developing taste through retrospective selection.

The classification is not always clean — some tasks have both at fine grain. When in doubt, treat as innovation; the cost of over-classifying is friction, the cost of under-classifying is letting AI substitute for the part of the work that develops the researcher.

#### What success looks like

The researcher can articulate, for any given working session, what kind of operation they were doing and what role AI played. Sessions without this articulation are sessions where AI's role drifted by default.

#### Known costs

The classification step adds metacognitive overhead. It is also imperfect — researchers will misclassify. Both are tolerable.

#### Notes

This guideline is the methodology's operationalization of `evidence/literature-notes/innovation-as-different-operation.md` §2. It has obvious overlap with G1 (the empower question is sharper for innovation work), and the two should usually be applied together.

---

### G5: For tasks that resist clean decomposition, refuse whole-task outsourcing

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A17 (cluster V)
**Evidence trail:** Derived from `foundation/00-why-reimagine.md` §2 and `foundation/01-ai-attributes.md` A17.
**Skill implication:** Preserves the practice of staying involved at fine grain in tasks where the routine and the original interleave. This is the practice that keeps the researcher's capacity intact when working on tasks that the natural gradient pulls toward whole-task outsourcing.

#### Practice

When a task does not separate cleanly into "AI part" and "human part," do not let AI do the whole task. Stay involved at fine grain — write some, prompt for some, integrate, iterate. Accept the awkwardness of partial outsourcing as the price of preserved skill. The practice is not heroism; it is choosing slower-and-developing over faster-and-hollowing as a default.

In practice this often means writing the structure or the load-bearing pieces yourself, then using AI for filling, polish, or specific subordinate moves. The exact division depends on the task. The method is to never let the question "should I just have AI do all of this?" be answered by default.

#### What success looks like

A month of work shows several tasks where the researcher can describe what they did themselves, what AI did, and what the integration looked like. Tasks where the answer is "AI did all of it, I reviewed" are flagged as candidates for skill drift.

#### Known costs

This guideline costs measurable productivity in the short term. Whole-task outsourcing is, in the moment, faster. The methodology accepts this trade because the slower path is the one that preserves the researcher's capacity, and the productivity loss only looks like loss if the second output (researcher growth) is not being measured.

#### Notes

Open question Q12 in `foundation/03-open-questions.md` flags that this guideline may not generalize across all research domains. Some tasks may genuinely decompose; the guideline is most load-bearing where they do not.

---

### G6: Track the second output (researcher development) deliberately

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A13, A16 (cluster IV, V)
**Evidence trail:** Derived from `foundation/00-why-reimagine.md` §3 (research has two outputs).
**Skill implication:** Develops the meta-skill of noticing one's own developing or atrophying capacities. Without this practice, the second output is invisible and so unmanageable; with it, drift can be caught and addressed.

#### Practice

Maintain a separate log file (one per project, or one for the researcher across projects) tracking developing or atrophying capacities. Entries are short and dated: *"What was hard a month ago that feels easy now? What did I do this week that I would not have been able to do six months ago? What did I delegate to AI that I might have lost the ability to do myself?"*

Review the log monthly. Use it to surface skills that need deliberate practice (because they are atrophying under AI use) or skills that have developed enough to take on harder work.

#### What success looks like

The researcher can describe, with examples, the trajectory of their own capacity over a quarter or longer. Atrophying skills are caught early enough that deliberate re-practice can recover them. Developed skills are recognized and pressed into harder work.

#### Known costs

The log requires honesty about what the researcher cannot do. This is a different muscle from logging accomplishments; it tends to feel uncomfortable. The cost in time is small (15 minutes a week) but the cost in honesty is real.

#### Notes

Open question Q11 flags that the right practice for this is genuinely unclear. The log described here is one candidate; periodic skills audits and structured replication of past work are others. Promotion to `testing` should specify which candidate is being trialed.

---

### G7: Maintain a calibration log of personal AI-vs-no-AI productivity

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A13, A15 (cluster IV)
**Evidence trail:** `evidence/reading-list.md` — METR 2025 RCT (39-point gap between felt and measured productivity).
**Skill implication:** Develops the researcher's ability to honestly measure rather than feel. This is a discipline that cuts against the grain of how knowledge work is normally evaluated. The data accumulated also becomes evidence the methodology can use across years.

#### Practice

For tasks where it is possible to estimate, log: *task description, expected time, actual time, AI-assisted or not, retrospective sense of whether AI helped, hurt, or made no difference, and any specific notes on what AI did or didn't do well.* The log entries are short — one or two lines.

Review monthly. Look for patterns: tasks where AI consistently helps, tasks where the researcher consistently feels AI helped while the data shows otherwise, tasks where AI made no difference.

#### What success looks like

After several months, the researcher can answer "does AI help me with X?" with personal data, not vibes. The data is messy and n=1, but it is real.

#### Known costs

The discipline is hard to maintain. Logging takes attention away from the work being logged. The point at which the log becomes more friction than signal is real and worth watching for.

#### Notes

The METR finding is the cautionary anchor for this practice. Without personal calibration, the researcher is operating on intuitions that have a known 39-point error.

---

### G8: Score AI-generated candidates against your own ranking before AI evaluates

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A4, A5, A7 (cluster I, II)
**Evidence trail:** Derived from cluster I (cheap idea generation, selection as new bottleneck) and cluster II (sycophancy, confidence/correctness decoupling).
**Skill implication:** Develops the researcher's selection skill — the taste that distinguishes promising candidates from candidates that merely sound novel. Selection is the skill the new bottleneck demands; AI cannot supply it; the only way it develops is through deliberate practice.

#### Practice

When AI is used to generate a set of candidate ideas, hypotheses, framings, or directions, do this in order: (a) read the candidates without AI's commentary; (b) rank them yourself, with brief reasons; (c) only then ask AI to evaluate or rank them; (d) compare your ranking to AI's; (e) reconcile differences deliberately, not by deferring to AI.

Step (e) is where the practice does its work. AI's ranking will be biased by what looks fluent and confident; the researcher's ranking will be biased by their priors. Neither is correct on its own. Reconciliation builds the discrimination AI cannot provide.

#### What success looks like

The researcher has a record of cases where their ranking diverged from AI's, and how those divergences played out — sometimes the researcher was right, sometimes AI was, sometimes neither. The pattern of divergences is itself useful information about where the researcher's taste is reliable and where it needs work.

#### Known costs

Adds time at every multi-candidate AI use. Worth the cost when the choice among candidates is the substantive part of the work; not worth it for low-stakes selections.

#### Notes

This guideline is most useful for innovation work (G4). For recombination work, AI's ranking is often fine.

---

### G9: Pre-mortem prompt before any experimental design

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A6, A7 (cluster II)
**Evidence trail:** Derived from cluster II (self-validation default, sycophancy) and the verification-first direction in `foundation/02-implications.md`.
**Skill implication:** Develops the researcher's adversarial-thinking skill — the practice of attacking one's own design before defending it. AI's default disposition is validation; the explicit attack-prompt is the practice that builds the falsification habit.

#### Practice

Before designing any experiment or formalizing any hypothesis, run an explicit pre-mortem prompt with AI: *"What would falsify this? What control is missing? What would a hostile reviewer say? What are three different ways the result could be wrong?"* Use AI to attack rather than to support. Take the attacks seriously; revise the design before, not after, running it.

The prompt is deliberately structured to override sycophancy — by asking explicitly for attack, the researcher gets a different (and usually more useful) response than they would from a neutral or supportive prompt.

#### What success looks like

The researcher's experimental designs catch missing controls and hidden assumptions before execution. Failures from the kind of methodological flaw the Sakana evaluation documents become rare.

#### Known costs

The pre-mortem adds a step before any design work. It also produces uncomfortable lists — design flaws are often things the researcher would have preferred not to notice.

#### Notes

Pairs naturally with G3 (verification from a different source). The pre-mortem is verification at the design stage; G3 is verification at the output stage.

---

### G10: Treat AI literature reviews as starting graphs, not finished reviews

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A8 (cluster II)
**Evidence trail:** `evidence/reading-list.md` — Sakana evaluation (median 5 citations, mostly outdated, novelty misclassification); Deep Research failures (outdated data, deferring to less reliable sources).
**Skill implication:** Develops critical reading of the literature graph — the skill of distinguishing claims that survive source-checking from claims that look good in a summary but do not hold up. This is one of the skills A16 most directly puts at risk.

#### Practice

When using AI for literature work, treat the output as a starting graph that needs walking, not a finished review. For each substantive claim with a citation: visit the source, read enough to confirm the claim is what AI said it was, mark the citation in the working notes as `green` (claim confirmed against source), `yellow` (source exists but the AI's paraphrase is approximate), or `red` (citation could not be verified or is wrong). Yellow and red claims do not become foundation in further work without re-derivation.

#### What success looks like

Citations entering the researcher's actual work are nearly all green. The researcher catches AI hallucinations regularly enough that they no longer trust paraphrases without source-checking — and the source-checking habit becomes second nature.

#### Known costs

Source-walking is most of the value of a literature review. It is also most of the time. The practice of using AI to find candidate sources, then walking them by hand, is roughly the same effort as a careful pre-AI literature review — the savings are in coverage, not in reading time.

#### Notes

The point of this guideline is to prevent A8 (hallucination at the frontier) from contaminating the foundation of the researcher's own work.

---

### G11: Maintain a direction-and-outcome log to develop taste over time

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** Cluster I, related to A4; addresses Q7 in `foundation/03-open-questions.md`.
**Evidence trail:** `evidence/literature-notes/innovation-as-different-operation.md` §4 (selective-retention practice); reading-list entries on Campbell BVSR.
**Skill implication:** Develops taste — judgment about which directions are interesting, where "interesting" means load-bearing for things not yet known. Taste is the half of the BVSR operation AI cannot supply, and is the most consequential long-horizon skill of a researcher.

#### Practice

Maintain a separate log (per project, or for the researcher across projects) recording direction-choices and their outcomes. Each entry: *date, what direction was chosen, what was rejected, the reasoning at the time, and (later) what came of it.* Review quarterly: which choices paid off? Which signals at the time predicted that? Which intuitions held up; which were wrong?

This log is not a research log of experiments and results. It is specifically about *direction-choice* — the taste-exercising moments that BVSR's selective retention names.

#### What success looks like

After a year, the researcher can articulate, with examples, what kinds of direction-signals reliably predict good outcomes for them. The articulation may differ from the field's stated wisdom; that is fine and possibly the point.

#### Known costs

The log requires retrospective updating, which means the researcher has to remember to revisit it. Quarterly review is the rough cadence; weekly is too often, yearly is too rare.

#### Notes

This guideline is the methodology's response to open question Q7 — what selective retention looks like for an individual researcher. The log is one candidate practice; if it does not work, others (peer review of direction-choices, mentor conversations, public commitment) can be tried.

---

### G12: Resist the exploitation gradient; deliberately maintain exploration share

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A4 (cluster I); related to A1.
**Evidence trail:** `evidence/reading-list.md` — March (1991) on the drift toward exploitation. `evidence/literature-notes/innovation-as-different-operation.md` §4.
**Skill implication:** Preserves the practice of working on questions whose payoff is uncertain and distant — the practice that the gradient toward AI-cheap exploitation actively erodes. Without deliberate maintenance, the researcher loses both the taste for exploration and the patience for it.

#### Practice

Allocate explicit time — say, one day a week, or one half-day — to exploration work that is not aimed at any current deliverable. The exploration share is protected, not residual; it does not get eaten by deadlines. AI is allowed in this time but its role is constrained to substrate (G13), not agent.

The amount and cadence will need calibration. The point is to make the exploration share visible and maintained rather than implicit and slowly disappearing.

#### What success looks like

The researcher can name, at any moment, what fraction of their working time is going to exploration vs. exploitation. The exploration share does not shrink quarter over quarter without a deliberate decision.

#### Known costs

Protected time is real opportunity cost. Deadlines and deliverables genuinely compete for the same hours. The methodology is asking the researcher to make a choice that the system around them does not reward.

#### Notes

Open question Q8 in `foundation/03-open-questions.md` is whether this discipline holds against the gradient. Without measurement (G7), it likely does not.

---

### G13: Use AI as terrain map, not as agent

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A1, A2, A8 (cluster I, II); related to A16, A17 (cluster V).
**Evidence trail:** `evidence/literature-notes/innovation-as-different-operation.md` §4 ("use AI as substrate, not as agent"); `foundation/02-implications.md` (cluster V direction).
**Skill implication:** Preserves the navigation skill — the researcher's choice of which way to go in the work. Outsourcing navigation to AI is the most consequential form of replacement. Using AI to map the terrain instead, while staying in the navigation, develops both the navigation and the map-reading.

#### Practice

Frame AI's role as mapping the known thoroughly so the researcher can see where the map ends, not as choosing the next move. Concretely:

- Ask AI to summarize the existing literature so the researcher can locate the gaps.
- Ask AI to produce the obvious objections so the researcher can notice the non-obvious ones.
- Ask AI to enumerate the standard approaches so the researcher can choose which one (or none).
- Ask AI for the routine variants so the researcher's attention is free for the non-routine moves.

The pattern: AI provides the territory; the researcher provides the navigation. Avoid the inverse — do not ask AI which way to go, then route through the answer with light edits.

#### What success looks like

The researcher's working sessions show AI in support roles (mapping, enumerating, summarizing, attacking) and the researcher in driver roles (choosing, framing, deciding, integrating). Reversed roles are flagged and corrected.

#### Known costs

The pattern requires the researcher to do the navigation work, which is the harder and slower work. The terrain-map framing is a reminder, not a limit; AI will produce navigation if asked, and the discipline is to not ask.

#### Notes

This is most load-bearing for innovation work (G4). For routine recombination, AI as agent is sometimes fine — but G1 should still apply (is this empowering or replacing?).

---

### G14: Replicate a recent paper as a verification primitive

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A6, A9 (cluster II)
**Evidence trail:** `evidence/reading-list.md` — Wissner-Gross PSI/GPD (LBNL flawless replication of 2023 condensed-matter paper).
**Skill implication:** Develops the replication skill — the ability to take a paper's claims and reproduce them from independent ground. This skill is itself a form of verification (G3) and a form of literature engagement that source-walking alone does not produce.

#### Practice

Periodically — one paper per quarter is a starting cadence — pick a recent paper in the researcher's area and attempt AI-assisted replication of its main result. Log what worked, what broke, what AI did well, what required human intervention. The point is not to publish the replication; it is to keep the practice of reproducing others' work alive, and to test whether AI tooling makes replication accessible at the individual scale.

#### What success looks like

After a year, the researcher has 3–4 replication trials logged, with honest accounting of what AI made possible and what it didn't. The trials accumulate as a personal verification capability.

#### Known costs

A serious replication takes days to a few weeks. This is real time. The methodology proposes this anyway because the replication skill is structurally different from the skills typical research workflows develop, and is one of the few verification primitives that does not depend on the generator (G3, third-party replication mode).

#### Notes

This is the methodology's operationalization of the Wissner-Gross GPD framing for individual researchers. Open question Q5 in `foundation/03-open-questions.md` flags the open question of whether this is practical at solo scale.

---

### G15: Standardize logging of model, prompt, parameters, and date for reproducibility

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A12 (cluster III)
**Evidence trail:** Derived from A12 (inconsistency across runs).
**Skill implication:** Develops the discipline of treating AI output as a recorded artifact rather than ephemeral chat. This is more a record-keeping habit than a skill in the deeper sense, but it scales the researcher's ability to engage with their own past work and the field's reproducibility norms.

#### Practice

For any AI output that will be relied on substantively, record alongside the output: model name and version, the full prompt (or a link to it), any non-default parameters (temperature, etc.), and the date. A simple convention is sufficient — a `.aimeta.md` or `.aicontrib.md` file alongside the artifact, or a section in the artifact's commit message.

#### What success looks like

The researcher can reproduce, or attempt to reproduce, any past AI-assisted result. Reviewers and collaborators can audit the AI contribution to any artifact.

#### Known costs

Small but real overhead per AI use. The cost is dominated by the discipline of doing it consistently, not by the amount of work each instance requires.

#### Notes

This is the simplest guideline in the list. It is also the one most likely to lapse without explicit habit formation. Tools that automate it (e.g., templates, hooks) help, but the underlying discipline has to come first.

---

### G16: Gate knowledge-building with an explain-back check

**Status:** proposed (last reviewed 2026-06-10)
**Addresses attribute(s):** A13, A16 (cluster IV, V); A5, A7, A8 shape the practice's caveats
**Evidence trail:** [2026-06-10 professor interview](../evidence/interviews/2026-06-10-professor-classical-research-steps.md), [2026-06-10 pilot workspace audit](../evidence/observations/2026-06-10-pilot-workspace-audit.md)
**Skill implication:** Develops field fluency at the level the professor's account names — knowing the field well enough to make insightful observations and hold meaningful conversations — and the articulation skill of explaining a concept precisely. It also produces a *measured* (not felt) record of the second output: each passed or failed explain-back is a data point about the researcher's actual understanding, which neither the researcher's own sense (A13) nor AI's fluency (A16) supplies.

#### Practice

On a regular cadence (weekly is the classical default), and at the close of any unit of knowledge-building the researcher will rely on: the researcher explains the concept to the agent in their own words, without the source notes open. The agent probes with understanding-questions rather than recall-questions — at least one "work it out" derivation or application, at least one "why / what breaks if…" question, nothing answerable by pattern-matching the researcher's own notes — withholds the answers until the researcher commits to theirs, then grades honestly: correct / partial / wrong, with the correction and where it comes from. Two integrity rules, taken from the pilot's working version: a generous pass defeats the purpose, and understanding is never marked verified by any route other than a passed check.

Where the concept sits at the frontier (recent, niche), the grader is itself suspect (A8, A5): corrections there must be grounded in a source the researcher can open, not in the grader's paraphrase. A failed check is also signal about the learning artifact — if the miss traces to an unclear note, fix the note too.

The classical form of this check was a scarce resource: a professor's weekly attention. The AI-native adaptation makes the prober always available, which moves the cadence from "weekly, with the professor" to "at every closure the researcher cares about" — and frees the scarce professor-time for the checks only a human expert can run (G19).

#### What success looks like

Field knowledge the researcher relies on carries a trail of passed checks. Failed checks happen and are logged — a record with no failures indicates a generous grader (A7), not mastery. Over months, the record gives the researcher (and any mentor) a measured trajectory of the second output. The pilot's first recorded instance: a steady-state derivation that failed on first attempt and passed on re-attempt after a targeted hint — a real gap that fluent note-reading had not surfaced (one caught gap across two quiz events; signal, not validation).

#### Known costs

A check per closed concept adds real time to knowledge-building. The deeper cost is honesty under sycophancy pressure: the agent's grading drifts generous by default (A7), and the researcher is the one who has to demand strictness from their own grader.

#### Notes

Two convergent sources point at this practice: the supervising professor's classical mentoring instrument (a student explains a new concept weekly; he corrects inaccuracies; he reports it as an effective progress tracker) and the pilot's teach→quiz gate, which the team kept even after relaxing the methodology's authoring posture. The convergence is not full independence — the professor supervises that same pilot team, and both sources are recorded via the maintainer — so this counts as one practice seen from two angles, not two independent confirmations. It is a candidate answer to Q11 (how to track researcher development) and pairs with G6 — the check record is exactly the kind of entry the capability log wants. Authorship of the record, to keep the G6 ownership rule intact: the agent reports the grade and may transcribe the Q&A alongside the learning artifact (a transcript, not a self-assessment); the dated pass/fail entry in the capability log itself is written by the researcher, never the agent. Direction matters: G3 verifies *AI output* from an independent source; this guideline verifies *the researcher's understanding*, with the agent as prober and grader. The pilot's version cited G3 for legitimacy because no guideline owned the practice; this one now owns it.

---

### G17: Converge the survey into a researcher-authored five-part research proposition

**Status:** proposed (last reviewed 2026-06-10)
**Addresses attribute(s):** A4, A7 (cluster I, II); A8 governs one part
**Evidence trail:** [2026-06-10 professor interview](../evidence/interviews/2026-06-10-professor-classical-research-steps.md)
**Skill implication:** Develops problem formulation — the framing skill the charter names among those the research job is judged on. Writing the system model and problem formulation oneself is where the researcher's grasp of *what exactly is being asked* gets built; accepting an AI draft of them is where it silently doesn't.

#### Practice

When the survey-then-focus motion approaches commitment, converge it into a written research proposition with five parts (the classical structure, per the professor's account): (1) motivation and background; (2) system model; (3) problem formulation; (4) existing approaches; (5) the proposition itself — what the research will do and how it will contribute.

Division of labor: AI maps terrain for (1) and (4) under the terrain-map discipline (G13), with every claim in (4) source-walked per G10 — existing-approaches summaries are where frontier hallucination (A8) does the most damage, and a contribution claim built on a hallucinated gap collapses at review. The researcher authors (2), (3), and (5), phrasing included — accepting AI's phrasing of the problem is the anchoring trap (A7) the Context phase already warns about, applied at the highest-stakes artifact. Before adopting the proposition, attack it per G9: what would falsify it? what would a hostile reviewer say? is (5) genuinely distinguishable from the approaches in (4)? Version-control the proposition in the project state (G2); successive revisions of it are themselves a direction-and-outcome trail (G11).

#### What success looks like

The transition from surveying to executing happens through an explicit artifact rather than by drift. The researcher can hand the proposition to a skeptical expert (G19) and defend each part. Revisions are deliberate and logged, not silent.

#### Known costs

Writing the proposition is slower than letting direction accrete implicitly — that is the point, but the time is real. The five-part structure comes from one field culture (EE / signal processing); other fields may need a different decomposition, and the structure should bend to the field rather than the reverse.

#### Notes

This gives the phase 2→3 transition (survey-then-focus → design) a concrete exit artifact, which the process sketch previously lacked. Single-source evidence (one professor's account, relayed secondhand); the structure is offered as a starting shape, not a standard.

---

### G18: Build a minimum viable version early; iterate against reality

**Status:** proposed (last reviewed 2026-06-10)
**Addresses attribute(s):** A1, A3 (cluster I); A9, A17 bound it
**Evidence trail:** [2026-06-10 professor interview](../evidence/interviews/2026-06-10-professor-classical-research-steps.md) (the step itself; the AI-regime rationale is the maintainer's extension, marked as such there)
**Skill implication:** Develops end-to-end system thinking and the craft of designing iterations against observed behavior rather than against plans. Preserved against a named risk: delegating the whole build is exactly the whole-task outsourcing G5 refuses — the MVP is a vehicle for the researcher's contact with reality, not a deliverable to order from the agent.

#### Practice

Once a research proposition exists (G17), bias toward building the smallest end-to-end version of the research artifact that can confront reality — a toy model, a minimal pipeline on a small dataset, a sketched proof of a special case — rather than specifying the full study up front. The classical argument for waterfall planning — building is expensive, so plan exhaustively first — weakens in the AI regime: the recombination parts of a build (boilerplate, plumbing, standard baselines) are cheap to delegate (A3 carries the cost claim; A1 is what makes those parts "known elements" AI assembles reliably).

Three disciplines bound the practice. Classify before delegating (G4): the load-bearing modeling choices — what is simplified away and why, what the MVP must demonstrate to count — stay the researcher's; an MVP whose simplifications the researcher cannot defend is a demo, not research. Decide up front what the MVP would have to show to support or falsify the proposition — G9 applied at MVP scale. And carry the A9 caveat: cheap building multiplies candidate outputs while the verification bill stays unchanged; an unverified MVP result is a candidate, not a finding.

#### What success looks like

The proposition meets reality within weeks, not months. Wrong directions die cheaply on MVP evidence, and the death is logged (G11). For each MVP, the researcher can name what they built and decided themselves versus what was delegated.

#### Known costs

MVPs tempt scope drift in both directions: polishing the toy instead of answering the question, and trusting toy-scale results beyond their reach. The agile cadence also pulls the A9 verification load earlier in the project rather than reducing it.

#### Notes

The MVP is also what makes early expert review (G19) concrete — experts react more usefully to a running thing than to an abstract plan. Single-source evidence plus a maintainer inference; domain generality untested (Q12 applies — "build small first" means different things in theory, wet-lab, and fieldwork).

---

### G19: Put the work in front of expert humans early, and in parallel

**Status:** proposed (last reviewed 2026-06-10)
**Addresses attribute(s):** A6, A8 (cluster II); A7
**Evidence trail:** [2026-06-10 professor interview](../evidence/interviews/2026-06-10-professor-classical-research-steps.md). The [pilot workspace audit](../evidence/observations/2026-06-10-pilot-workspace-audit.md) corroborates the *existence of the mentor channel* (the pilot reserves its research-question commitment to a decision made with the supervising mentor); the early-and-parallel shape of this guideline rests on the interview alone
**Skill implication:** Develops presenting work-in-progress, defending it under live questioning, and converting expert critique into design changes — the respond-to-review skills, exercised early and repeatedly instead of once at submission time. Also maintains the mentorship channel the apprenticeship classically runs on, which AI does not substitute for.

#### Practice

From the first MVP (G18) onward, and in parallel with continuing the research — not as a stop-and-wait stage — put the work in front of expert humans and gather their reactions: the supervising mentor, domain experts, a colleague who has not seen the AI sessions. In an AI-saturated workflow this is a structural necessity, not a courtesy: AI critiques share the generator's blind spots to some degree (A6), and AI is weakest exactly at the frontier where the work is novel (A8) — the expert human is the critic whose independence is categorical and whose strength peaks where AI's fails.

AI assists the periphery: adapting the material to the audience (A2), surfacing which objections map to known weaknesses. The researcher presents and defends in their own person — an AI-drafted defense of a position the researcher has not reasoned to is the respond-to-review replacement failure, arrived at early. Log what the experts said against what AI critiques had said (G11): the divergence is a running measure of what AI review misses in this domain.

#### What success looks like

Expert feedback arrives early enough to redirect the work cheaply. The record shows expert objections no AI critique had surfaced — and occasionally the reverse, which is calibration data too (G7).

#### Known costs

Expert attention is scarce and asking for it has social cost; the practice spends real relationship capital and must be paced accordingly. Preparing work to be shown is overhead beyond doing the work.

#### Notes

Extends G3's "human review" verification mode from outputs to direction: G3 verifies a result; this keeps the *project* under independent expert pressure. It is a partial answer to Q7 (where selective retention comes from for a researcher without a full research-group culture — the mentor channel is part of it) and gives the process sketch's collaboration gap its first concrete mechanism.

---

## Retired guidelines

*(none yet)*

---

*Last revised 2026-06-10. Initial population of 15 guidelines drawn from the foundation as written through 2026-05-06; G16–G19 added 2026-06-10 from the first evidence of the pilot phase (a professor interview on the classical research steps, adapted AI-natively, and the first pilot workspace audit). All at status `proposed`. None are based on systematic evidence yet; promotion requires deliberate trial and observed signal.*
