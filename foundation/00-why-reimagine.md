# Why reimagine research

This is the front door of the inquiry. It does four jobs: it lays out what most thoughtful researchers already see about AI's impact, takes that view one step further into something less obvious, names why the situation is urgent, and proposes the mindset shift the rest of the methodology will operationalize. The mindset, in one phrase: **empower, not replace.**

The reader who finishes this document should leave with two things: the argument that something needs to be done, and a clear pointer to what kind of something it is.

---

## 1. Where you probably already are

If you are reading this, you have likely noticed some version of the following.

AI has become competent at producing fluent first drafts of nearly everything researchers produce around their core work — literature summaries, code, charts, data analyses, prose. Tasks that used to take a day take minutes. Tasks that used to require weeks of specialist effort can be approximated in an afternoon by a non-specialist.

You have also probably noticed that the speed-up is not unconditionally good. Fluent output is not the same as correct output. AI-generated literature reviews cite papers that exist, papers that don't, and papers whose claims do not match what the AI says they claim. AI-generated code runs in some senses and breaks in others. AI-generated analyses look serious and sometimes are.

You may have noticed your own work shifting around AI. Tasks you would have done by hand a year ago, you now hand off without thinking about it. The handoff usually feels efficient. Sometimes you notice, after, that you cannot quite reconstruct what the AI did, or that you cannot quite explain why the result is the result. Sometimes you do not notice.

You have probably heard the two loud reactions to all of this. One is that AI is a transformative tool researchers should adopt aggressively or be left behind. The other is that AI produces convincing-looking work without substance and that adopting it carelessly will degrade research as a craft. Both reactions are responding to something real. Neither, on its own, is a methodology.

This is the floor. None of it is news. This document is for the reader who recognizes the situation and wants to think about what comes next.

## 2. What you may not have followed through on yet

Every prior knowledge-work technology required a reciprocal skill from its user. The calculator displaced arithmetic and produced calculator-literacy. The compiler displaced assembly programming and produced fluency in higher-level languages. GPS displaced dead-reckoning navigation and produced route-planning judgment. Each tool changed which skills mattered, but the user developed *some* compensating capability. The new skills compounded the way the old ones did. Workers were fine.

This is the standard reassurance the field reaches for when discussing any new tool: *technology changes the skill set, but the worker is still skilled, just at different things.* It has been reliable enough that we use it almost without thinking.

AI is the first tool that breaks the pattern. "Prompt and accept" is not a skill that compounds the way calculator-operation did. A user can produce output that looks like progress, indefinitely, without growing. The output is genuine in the sense that it exists; the growth is genuine in the sense that it does not happen.

This is the structural fact the rest of the document rests on. **AI is the first tool that can substitute for skill without requiring reciprocal skill development.** It is not "a faster way to do the same things." It is a way to produce results without becoming the kind of person who could produce them. The historical reassurance about technology and skills does not apply to it specifically, and acting as if it does is one of the field's most consequential mistakes.

Three things follow.

**The temptation to outsource is a trap, not a tradeoff.** With prior tools, outsourcing a task you used to do by hand was a clean trade — old capacity given up, new capacity gained, the new capacity compounded. AI offers the first outsourcing where the trade is asymmetric: you give up the practice that built your old capacity, and you gain nothing that compounds. The standard "use AI for the routine, keep yourself on the hard parts" framing assumes a trade AI does not actually make. The methodology's job is not to balance the trade. It is to preserve the practice the trade would erase.

**Tasks resist the clean cut the temptation requires.** The natural defense — *let AI do the routine bits, keep me on the hard ones* — assumes the routine and the hard separate cleanly. They do not, in research. The fine-grained interleaving of well-trodden technique and original move is most of what makes a task research rather than execution. Doing partial outsourcing — your part, then reviewing AI's part, then integrating — is more work than either alternative. The gradient pulls toward whole-task outsourcing because partial outsourcing is awkward. The methodology has to address tasks that do not decompose, not tasks that do.

**Output is one optimization target; the user is another.** Most knowledge work has only one output that matters — the deliverable. A worker who finishes a task with the deliverable in hand has done their job. But AI's offer to the user changes the user, in ways that take longer to feel and that compound across tasks. A workflow that ships strong outputs and quietly hollows out the worker has succeeded on one axis and failed on another, and the second failure is invisible until much later.

These three points are not separate concerns. They are one structural problem from three angles: **AI's offer changes the user, and changes them in directions the methodology is not currently built to notice.**

## 3. Why research is the case that matters most

What is true of knowledge work generally is sharper for research, for four reasons.

**Research's defining operation is the production of claims that did not exist before.** The thing research produces is novelty that survives review and replication. Most other knowledge work applies known patterns to new instances; research, at its core, is new patterns. AI's structural bias toward its trained distribution — its tendency to produce fluent recombinations of established work — is most useful for the parts of research that look most like other knowledge work, and least useful for the parts that are research-specific. A workflow that lets AI do "the work" tends to drift toward the parts that are not research.

**Production is at least two operations, not one, and they respond to AI differently.** Producing a literature summary, a routine analysis, or a draft of a familiar argument is *recombination* of existing material — assembling known elements from a known distribution. AI does this well; the cost-structure inversion described in §2 mostly holds.

Producing a new framing, a method that did not exist, a hypothesis nobody has stated is *innovation*. The literature on innovation — Campbell's Blind Variation and Selective Retention (BVSR), March's exploration vs exploitation, Stanley's novelty search, Sarasvathy's effectuation — converges on a structure for it that the recombination framing cannot capture. Innovation, across all four lines of work, is the joint operation of two things: **variation that is *not* directed by the goal**, combined with **selection that is retrospective and aggregate**. The variation is "blind" in Campbell's technical sense — its utility cannot be known at the time of generation, which is precisely why it can produce something the searcher would not otherwise find. The selection happens after the fact, on a portfolio of variants of which most fail. The two together are what the maintainer's own framing called *smart diversification*: diversification that is effective in aggregate even when individual variants are not.

The relevance to AI is sharp. AI's "novelty," the variants it produces in volume, is not blind in this sense. AI is biased toward its trained distribution; its variation clusters around the modes the model has seen most often. Stanley's framing — *as soon as you create an objective, you ruin your ability to reach it* — applies directly: AI is implicitly optimizing for plausible-looking output, which is an objective, which biases generation toward existing modes. So AI is structurally **a parallel exploitation engine more than a parallel exploration engine**. Its cost reduction applies cleanly to recombination and does not apply cleanly to innovation. AI also cannot do the retrospective-selection half — selection requires taste, which AI lacks. So AI is at most a partial-fit collaborator for innovation work: useful as a substrate that maps the known terrain (literature scans, routine variants, obvious objections) so the human's attention is free for blind variation and for taste, not as the agent of innovation itself.

A methodology that does not distinguish recombination from innovation will be correct about routine work and silently wrong about the part of research that matters most. The deeper synthesis of the innovation literature is in [`../evidence/literature-notes/innovation-as-different-operation.md`](../evidence/literature-notes/innovation-as-different-operation.md).

**Research has the researcher's growing competence as a primary output.** Most knowledge work optimizes for the deliverable. Research has two outputs: the work, and the worker — the researcher who finishes a project more capable, more discriminating, with deeper taste, than they started. For an early-career researcher in particular, the second output is often more durable and more consequential than any individual paper. AI workflows are uniquely positioned to fail at the second output because of the structural fact in §2: outsourcing tasks does not develop the researcher. A methodology that ships fluent papers but leaves the researcher unchanged has failed at half its job.

**Research has higher stakes for fluent-but-empty output.** A bad draft of a customer email costs an apology. A bad draft of a research claim, fluent enough to pass internal review, can mislead a field for years. The Sakana AI Scientist evaluation found that the system produced manuscripts "many reviewers might struggle to distinguish" from real work, while also producing 42% experiment failures from coding errors and "hallucinated numerical results." This is what happens when AI is allowed to produce research-shaped output without verification structures research demands. The cost falls on more than just the producer.

For these reasons, the response to AI in research cannot be the response to AI in adjacent domains. Faster lit scans help. Faster code helps. Faster drafting helps. But these alone do not address the structural problem — and pretending they do produces work that is more, but not better, and researchers who are productive but not progressing.

## 4. Why now

The capability moved fast. Three years ago this conversation was speculative; today it is overdue. The default trajectory the field is on is the dangerous one.

Adoption is happening, with or without deliberate methodology. Researchers are using AI individually, fast, in whatever way feels efficient in the moment. Universities and labs are largely not adapting their structure — they are adopting tools. The default at the institutional level is "let people figure it out." The default at the individual level is the one §2 just described — outsource what looks routine, lose the practice that built the capacity, do not notice until the lost capacity is needed.

The gradient is in the wrong direction. AI makes outsourcing cheaper and easier; outsourcing produces output that looks like progress; the user feels productive; the metrics that would catch the failure (skill drift, taste atrophy, drift toward exploitation work) operate on timescales of years rather than weeks. Inertia is not neutral. Waiting is a vote for the default.

Bad practices ossify. AI-assisted papers without verification trails, hallucinated citations entering the literature, productivity claims that nobody checked: these are accumulating now. Each one is harder to push back on than it was a month ago. The field is forming its norms in this period, mostly by default.

This is the urgency. There is a window in which a researcher who reorganizes their workflow deliberately — who uses AI in ways that grow them, who maintains practice in tasks that do not decompose, who treats verification as a primary operation rather than a finishing step — has a compounding advantage. The same window is one in which the field's defaults are being set. Setting them well requires people who are doing the work well in the open.

## 5. The mindset shift: empower, not replace

The choice is not whether to use AI. That choice has been made. The choice is whether to use AI in ways that empower the researcher or in ways that replace them.

**Empower** means: AI is used in service of building the researcher's capacity, not as a substitute for it. Every use is evaluable against the question — *will I be more capable as a result of this, or less?*

**Replace** means: AI is used to produce outputs the researcher could not have produced themselves and now will not learn to produce. The output exists; the capacity to produce it does not develop and may atrophy.

The two are not always easy to distinguish in the moment. The same AI prompt can be empowering or replacing depending on what the researcher does with the output, what they would have done without it, whether they engage critically with what comes back, whether the practice they are skipping is one they need to keep. The methodology will not provide a clean rule. What it can provide is a framing that makes the question visible at every choice, and a set of practices that bias the answer in the right direction.

This framing does not solve the problem. It names the problem so the methodology can address it instead of optimizing for output and hoping the researcher's capacity takes care of itself. The five directions in [`02-implications.md`](02-implications.md) are first attempts at what empowerment looks like in practice. The methodology in [`../methodology/guidelines.md`](../methodology/guidelines.md) accumulates concrete guidelines, each evaluable against the empower/replace question.

Empower-not-replace is not a slogan to repeat. It is a question the researcher asks at every step where AI is used, and a question the methodology has to make easy to ask.

## 6. What this repo is

The aim is not to publish a finished framework. It is to record an inquiry — what was read, what was tried, what worked, what didn't, what was changed and why — in a form another researcher can read along with and borrow from.

The structure: the diagnosis lives in [`foundation/`](.) — this document, [`01-ai-attributes.md`](01-ai-attributes.md) (the catalog), [`02-implications.md`](02-implications.md) (gestures toward methodology), [`03-open-questions.md`](03-open-questions.md) (what is still open). The deeper literature synthesis on innovation that §3 above draws on lives in [`../evidence/literature-notes/innovation-as-different-operation.md`](../evidence/literature-notes/innovation-as-different-operation.md). The methodology lives in [`../methodology/guidelines.md`](../methodology/guidelines.md), grows from evidence, and starts with the initial guidelines drawn from this foundation. The evidence lives in [`../evidence/`](../evidence/). The chronicle of how the inquiry has changed lives in [`../log/`](../log/). Real research projects, when applied, will live in [`../case-studies/`](../case-studies/).

The methodology will never be finished. AI is changing. What works changes with it. A foundation that treats "under construction" as a phase ending in some future v1.0 will be wrong by the time v1.0 ships. The repo's structure is the inquiry. The first imperfect version beats the perfect-but-future version, every time.

The repo is not currently accepting external contributions. It is deliberately one researcher's working artifact, in public, while the foundation is being developed and the pilot research domain is being chosen. Reach out through the contact in [`../CONTRIBUTING.md`](../CONTRIBUTING.md) if you have substance to offer — an interview, a structured experiment, a contradiction that bears on the foundation.

The repo will be wrong about things. It will revise. It will retire guidelines. The point is that the revisions are visible.

---

*Last revised 2026-05-06. Section 3's recombination/innovation paragraph expanded to absorb the substance previously living in `02-innovation.md` (now moved to `../evidence/literature-notes/`). Substantial §1–§6 rewrite earlier the same day established empower-not-replace as the central mindset and the structural skill-substitution claim as the load-bearing diagnostic.*
