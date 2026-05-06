# Methodology guidelines

Accumulated practices the inquiry proposes, is testing, or has adopted. Each guideline traces to the foundation attribute(s) it addresses, the evidence that motivated it, and an explicit *skill implication* — the capacity the practice is meant to develop or preserve in the researcher. The skill-implication field is not optional; a guideline that cannot say what skill it builds is one that risks substituting for skill, and the methodology's central principle (`foundation/00-why-reimagine.md` §5: empower, not replace) cannot tolerate that.

The guidelines below are first-pass drafts derived from the foundation as written through 2026-05-06. None of them are based on systematic evidence yet; all start at status `proposed`. Promotion to `testing` requires deliberate trial; promotion to `adopted` requires evidence that the trial worked. Use the [`add-guideline`](../.claude/skills/add-guideline/SKILL.md) skill for additions and the [`update-foundation`](../.claude/skills/update-foundation/SKILL.md) skill when status changes.

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

### G1: Treat empower-vs-replace as a question to ask at every AI use

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A16, A17 (cluster V)
**Evidence trail:** Derived from `foundation/00-why-reimagine.md` §5, the central mindset of the inquiry.
**Skill implication:** Develops the metacognitive capacity to notice when AI use is substituting for skill development versus supporting it. This is the load-bearing skill of the entire methodology; without it, all other guidelines drift toward replacement under the gradient.

#### Practice

Before any non-trivial AI use, pause for one question: *will I be more capable as a result of this, or less?* The answer is rarely "yes" or "no" — it is usually "yes if I do X, no if I just accept the output." Note the X. Coarse heuristics that help when the question feels uncertain: *did I learn something I didn't know? Could I reproduce this without AI in six months? Am I skipping a practice I would benefit from doing?*

The pause does not have to be elaborate. It needs to be habitual. The point is to make the empower/replace question visible at the moment of choice, not after the choice has compounded into atrophy.

#### What success looks like

Over time, the researcher can articulate which kinds of AI uses they have reliably found empowering and which they have found replacing. The articulation should be specific to the kind of work — "AI for literature scans empowers me when I cross-check claims against sources; replaces me when I summarize without reading."

#### Known costs

The pause adds friction. For some uses (formatting a citation, a quick syntactic question), the friction is more than the question is worth. The methodology has to allow the researcher's judgment to skip the pause where it does not serve. Rule of thumb: pause when the AI's output would be the substantive deliverable of the moment.

#### Notes

This is the meta-guideline. Other guidelines below are specific operationalizations of empower-not-replace in particular contexts.

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

The Tao reference is about math specifically; the practice generalizes because the underlying attribute (session forgetting) is general. This is open question Q3 in `foundation/04-open-questions.md` — whether the discipline scales without becoming its own friction.

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
**Evidence trail:** `foundation/02-innovation.md`; reading-list entries on Campbell BVSR, March, Stanley, Sarasvathy.
**Skill implication:** Develops the metacognitive capacity to recognize, in the moment, which kind of operation a task is — recombination of known elements, or innovation that requires variation outside the known distribution. This recognition is itself a research skill that AI cannot supply; the practice of asking the question at every task is what builds it.

#### Practice

Before starting any non-trivial task, classify it: *is this recombination work (assembling known elements into a fluent output) or innovation work (producing something the trained distribution does not contain)?* For recombination, AI is well-suited as a parallel production engine; verification (G3) is the dominant concern. For innovation, AI is a partial-fit substrate at best; the dominant concerns are protected depth, exposure to negative space, and developing taste through retrospective selection.

The classification is not always clean — some tasks have both at fine grain. When in doubt, treat as innovation; the cost of over-classifying is friction, the cost of under-classifying is letting AI substitute for the part of the work that develops the researcher.

#### What success looks like

The researcher can articulate, for any given working session, what kind of operation they were doing and what role AI played. Sessions without this articulation are sessions where AI's role drifted by default.

#### Known costs

The classification step adds metacognitive overhead. It is also imperfect — researchers will misclassify. Both are tolerable.

#### Notes

This guideline is the methodology's operationalization of `foundation/02-innovation.md` §2. It has obvious overlap with G1 (the empower question is sharper for innovation work), and the two should usually be applied together.

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

Open question Q12 in `foundation/04-open-questions.md` flags that this guideline may not generalize across all research domains. Some tasks may genuinely decompose; the guideline is most load-bearing where they do not.

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
**Evidence trail:** Derived from cluster II (self-validation default, sycophancy) and the verification-first direction in `foundation/03-implications.md`.
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
**Addresses attribute(s):** Cluster I, related to A4; addresses Q7 in `04-open-questions.md`.
**Evidence trail:** `foundation/02-innovation.md` §4 (selective-retention practice); reading-list entries on Campbell BVSR.
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
**Evidence trail:** `evidence/reading-list.md` — March (1991) on the drift toward exploitation. `foundation/02-innovation.md` §4.
**Skill implication:** Preserves the practice of working on questions whose payoff is uncertain and distant — the practice that the gradient toward AI-cheap exploitation actively erodes. Without deliberate maintenance, the researcher loses both the taste for exploration and the patience for it.

#### Practice

Allocate explicit time — say, one day a week, or one half-day — to exploration work that is not aimed at any current deliverable. The exploration share is protected, not residual; it does not get eaten by deadlines. AI is allowed in this time but its role is constrained to substrate (G13), not agent.

The amount and cadence will need calibration. The point is to make the exploration share visible and maintained rather than implicit and slowly disappearing.

#### What success looks like

The researcher can name, at any moment, what fraction of their working time is going to exploration vs. exploitation. The exploration share does not shrink quarter over quarter without a deliberate decision.

#### Known costs

Protected time is real opportunity cost. Deadlines and deliverables genuinely compete for the same hours. The methodology is asking the researcher to make a choice that the system around them does not reward.

#### Notes

Open question Q8 in `foundation/04-open-questions.md` is whether this discipline holds against the gradient. Without measurement (G7), it likely does not.

---

### G13: Use AI as terrain map, not as agent

**Status:** proposed (last reviewed 2026-05-06)
**Addresses attribute(s):** A1, A2, A8 (cluster I, II); related to A16, A17 (cluster V).
**Evidence trail:** `foundation/02-innovation.md` §4 ("use AI as substrate, not as agent"); `foundation/03-implications.md` (cluster V direction).
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

This is the methodology's operationalization of the Wissner-Gross GPD framing for individual researchers. Open question Q5 in `foundation/04-open-questions.md` flags the open question of whether this is practical at solo scale.

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

## Retired guidelines

*(none yet)*

---

*Last revised 2026-05-06. Initial population of 15 guidelines drawn from the foundation as written through 2026-05-06. All start at status `proposed`. None are based on systematic evidence yet; promotion requires deliberate trial and observed signal.*
