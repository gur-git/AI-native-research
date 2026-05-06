# Why reimagine research

This document does five things, in order: it lays out how research has historically worked and where its value comes from; it situates AI in the longer history of how technology has changed knowledge work; it explains why AI breaks a pattern that has held reliably for the previous tools; it shows why this forces a particular reimagining of research; and it proposes the mindset shift the rest of the methodology operationalizes.

The argument runs through a chain. Each section is meant to be a step that can be checked before the next. Skipping ahead is fine, but the argument is cleaner taken in order.

---

## 1. What research has been

Research, as a kind of knowledge work, has a structure most professional writing does not. Most knowledge work serves an audience that mostly trusts the producer; research serves an audience whose job it is *not* to trust. A claim in a paper is supposed to survive review, replication, and adversarial examination. The defining operation is the production and verification of claims that did not exist before.

Around that core operation, there is a wide periphery of supporting work — reading, summarizing, analyzing, drafting, plotting, testing, formatting. These are not the research itself; they are what makes the research possible. They take the bulk of a researcher's time. The relationship between core and periphery has been stable for a long time: the periphery is expensive in human hours but routine, the core is small in volume but where the value lives, and the routine work of the periphery is what trains the researcher in the judgment that the core requires.

The work has another property worth naming explicitly. A researcher's understanding of a problem deepens with practice. A second project in a domain is faster than the first, and the third faster than the second, not because the work itself is faster but because the researcher has grown. Research therefore has two outputs, not one: the artifact (papers, results, code) and the researcher (a person who can do harder work next time than they could last time). The second output compounds across years and is often more durable than any individual artifact. For early-career researchers in particular, the second output is most of why the first output matters.

The cost structure that has shaped how research is done flows from these properties. Production work in the periphery has been the binding constraint — drafts cost time, analyses cost time, lit reviews cost time. Judgment of one's own work has been comparatively cheap, because the person doing the judging was also the person who had just done the work and had context. Workflows, training, careers, and institutions optimized for this. Junior researchers' apprenticeship has largely been about getting faster and more accurate at periphery work, on the well-supported assumption that the core skills come from doing the periphery work attentively over years.

## 2. How technology has historically changed knowledge work

When new tools change the cost of some part of a workflow, the workflow reorganizes. This is general; it happens in research, in software, in writing, in any domain that uses tools. What is less general — and what is the relevant pattern for understanding AI — is the *shape* of the reorganization that has historically followed.

The pocket calculator displaced arithmetic. Before pocket calculators were common, doing a regression by hand was a multi-hour exercise; afterward, it was a button press. What replaced the lost skill was not nothing. Calculator-literacy became a real capability — knowing what to ask the calculator, knowing how to spot when the answer was off by an order of magnitude, knowing when to fall back to mental arithmetic for a sanity check. The skill set changed. The user was still skilled, just at different things, and the new skills compounded across a career the way the old ones did.

Compilers and high-level languages displaced direct work in machine code and assembly. Programmers used to write loops by hand-managing registers; now they write `for x in xs:`. The skill that compiled-out — register-level optimization — was real and is still real for the few who need it, but for nearly everyone it was traded for higher-level fluency: data structure choice, type system intuition, library knowledge, debugging in higher-level abstractions. Different shape, same pattern: the worker remained skilled.

GPS displaced dead-reckoning navigation. London cabbies, who used to grow their hippocampi memorizing the city, mostly use turn-by-turn directions now. What appeared in place of the lost skill was route-planning judgment — when to trust the routing, when to detour, how to recover when the GPS is wrong. Different skill, same pattern.

The pattern repeats across very different tools — spreadsheets, type systems, version control, search engines, statistical packages — reliably enough that it has become the standard reassurance the field reaches for when discussing any new tool: *technology changes the skill set, but the worker is still skilled, just at different things.* We have been right about it for a long time.

The pattern works because of a property of all those tools that we did not need to name. Every prior tool required *informationally substantial* input from its user. The user had to know what they wanted with enough specificity that operating the tool was itself an exercise of skill — and so the skill, once exercised, was the new reciprocal skill the tool produced. Calculator-literacy is the skill of knowing what to compute. Higher-level fluency is the skill of knowing what to express. Route-planning judgment is the skill of knowing what to navigate toward. The tool's quality came from the user's input quality, and so using the tool well *was* the new skill.

## 3. How AI is different

AI is the first tool in this pattern that does not work this way.

A natural-language request to an AI model is informationally thin. *"Write a literature review on X." "Summarize this paper." "Generate a hypothesis."* The user is not specifying very much — and the model produces output that is fluent enough to look complete. The asymmetry between what the user puts in and what comes out is a step-change from any prior tool, and it is, in fact, what makes AI valuable. The whole appeal is that the user does not have to articulate what they want at the level of detail prior tools required.

That asymmetry breaks the historical pattern. The skill the prior tools produced was the skill of putting in articulate input — of *knowing what to ask for* with enough specificity that operating the tool was itself an act of fluency. AI does not require this. "Prompt and accept" is not a compounding skill in the way calculator-operation was. A user can produce fluent output indefinitely without the input-side practice that built the prior generations of skills.

This is the structural fact this entire document rests on. **AI is the first tool that can substitute for skill without requiring reciprocal skill development.** Not "a faster way to do the same things," not "a tool with a different skill set," but a way to produce results without becoming the kind of person who could produce them. The output is genuine in the sense that it exists; the growth is genuine in the sense that it does not happen.

This is not a current limitation that will be designed away. It is a property of how the technology works. Improvements to AI have, so far, widened the asymmetry rather than closing it — each generation produces more fluent output from less articulate input, not the other way around. The methodological response is not to wait for AI to require skill from its users; it is to design workflows that develop the user's skill *despite* AI not requiring it.

Three things follow.

**The temptation to outsource is a trap, not a tradeoff.** With prior tools, outsourcing a task you used to do by hand was a clean trade — old capacity given up, new capacity gained, the new capacity compounded. AI offers the first outsourcing where the trade is asymmetric: the practice that built the old capacity is given up, and nothing that compounds is gained. The standard "use AI for the routine, focus on the hard parts" framing assumes a trade AI does not actually make. The methodology's job is not to balance the trade. It is to preserve the practice the trade would erase.

**Tasks resist the clean cut the temptation requires.** The natural defense — *let AI do the routine bits, keep me on the hard ones* — assumes the routine and the hard separate cleanly. They do not, in research. The fine-grained interleaving of well-trodden technique and original move is most of what makes a task research rather than execution. Doing partial outsourcing — your part, then reviewing AI's part, then integrating — is more work than either alternative. The gradient pulls toward whole-task outsourcing because partial outsourcing is awkward. The methodology has to address tasks that do not decompose, not tasks that do.

**The deliverable is one optimization target; the worker is another.** Most knowledge work has only one output that matters. Research, as §1 noted, has two. AI's offer to the user changes the user, in ways that take longer to feel and that compound across tasks. A workflow that ships strong outputs and quietly hollows out the worker has succeeded on one axis and failed on another, and the second failure is invisible until much later.

## 4. Why this forces reimagining research specifically

What is true of knowledge work generally is sharper for research, because of the properties §1 named.

**Research's defining operation is the production of claims that did not exist before.** Most knowledge work applies known patterns to new instances; research, at its core, is new patterns. AI's structural bias toward its trained distribution — its tendency to produce fluent recombinations of established work — is most useful for the parts of research that look most like other knowledge work, and least useful for the parts that are research-specific. A workflow that lets AI do "the work" tends to drift toward the parts that are not research.

**Production decomposes into recombination and innovation, and they respond to AI differently.** Producing a literature summary, a routine analysis, or a draft of a familiar argument is *recombination* — assembling known elements from a known distribution. AI does this well; the cost-structure shift §3 described applies cleanly here. Producing a new framing, a method that did not exist, a hypothesis nobody has stated is *innovation*. The literature on innovation — Campbell's Blind Variation and Selective Retention, March's exploration vs exploitation, Stanley's novelty search, Sarasvathy's effectuation — converges on a structure for it that the recombination framing cannot capture. Innovation is the joint operation of two things: variation that is *not* directed by the goal, and selection that is retrospective and aggregate. The variation is "blind" in Campbell's technical sense — its utility cannot be known at generation time, which is precisely why it can produce something the searcher would not otherwise find. The selection happens after the fact, on a portfolio of variants of which most fail. Together these amount to what one might call *smart diversification:* diversification that is effective in aggregate even when individual variants are not.

AI's "novelty" is not blind in this sense. AI is biased toward its trained distribution; its variation clusters around modes the model has seen most often. Stanley's framing applies directly: *as soon as you create an objective, you ruin your ability to reach it.* AI is implicitly optimizing for plausible-looking output, which is an objective, which biases generation toward existing modes. So AI is structurally **a parallel exploitation engine more than a parallel exploration engine**. Its cost reduction applies cleanly to recombination and does not apply cleanly to innovation. AI also cannot do the retrospective-selection half — selection requires taste, which AI lacks. So AI is at most a partial-fit collaborator for innovation work: useful as a substrate that maps the known terrain so the human's attention is free for blind variation and for taste, not as the agent of innovation itself. The deeper synthesis of the innovation literature is in [`../evidence/literature-notes/innovation-as-different-operation.md`](../evidence/literature-notes/innovation-as-different-operation.md).

**Research has the researcher's growing competence as a primary output.** This is the property §1 named. Most knowledge work optimizes for the deliverable; research has two outputs. AI workflows are uniquely positioned to fail at the second output because of §3: outsourcing tasks does not develop the researcher. A methodology that ships fluent papers but leaves the researcher unchanged has failed at half its job, and the failure is exactly the one the historical pattern of skill-shifting tools would not have produced.

**Research has higher stakes for fluent-but-empty output.** A bad draft of a customer email costs an apology. A bad draft of a research claim, fluent enough to pass internal review, can mislead a field for years. The Sakana AI Scientist evaluation found that the system produced manuscripts "many reviewers might struggle to distinguish" from real work, while also producing 42% experiment failures from coding errors and "hallucinated numerical results." This is what happens when AI is allowed to produce research-shaped output without the verification structures research demands. The cost falls on more than just the producer.

Faster lit scans help. Faster code helps. Faster drafting helps. None of these answer the structural problem. A response to AI in research that is built only on what is true of AI in adjacent domains will produce work that is more, but not better — and researchers who are productive but not progressing.

## 5. Why now

The capability moved fast. Three years ago this conversation was speculative; today it is overdue. The default trajectory the field is on is the dangerous one.

Adoption is happening, with or without deliberate methodology. Researchers are using AI individually, fast, in whatever way feels efficient in the moment. Universities and labs are largely not adapting their structure — they are adopting tools. The default at the institutional level is "let people figure it out." The default at the individual level is the one §3 just described — outsource what looks routine, lose the practice that built the capacity, do not notice until the lost capacity is needed.

The gradient is in the wrong direction. AI makes outsourcing cheaper and easier; outsourcing produces output that looks like progress; the user feels productive; the metrics that would catch the failure (skill drift, taste atrophy, drift toward exploitation work) operate on timescales of years rather than weeks. Inertia is not neutral. Waiting is a vote for the default.

Bad practices ossify. AI-assisted papers without verification trails, hallucinated citations entering the literature, productivity claims that nobody checked: these are accumulating now. Each one is harder to push back on than it was a month ago. The field is forming its norms in this period, mostly by default.

There is a window in which a researcher who reorganizes their workflow deliberately — who uses AI in ways that grow them, who maintains practice in tasks that do not decompose, who treats verification as a primary operation rather than a finishing step — has a compounding advantage. The same window is one in which the field's defaults are being set. Setting them well requires people who are doing the work well in the open.

## 6. The mindset shift: empower, not replace

The choice is not whether to use AI. That choice has been made. The choice is whether to use AI in ways that empower the researcher or in ways that replace them.

**Empower** means: AI is used in service of building the researcher's capacity, not as a substitute for it. Every use is evaluable against the question — *will I be more capable as a result of this, or less?*

**Replace** means: AI is used to produce outputs the researcher could not have produced themselves and now will not learn to produce. The output exists; the capacity to produce it does not develop and may atrophy.

The two are not always easy to distinguish in the moment. The same AI prompt can be empowering or replacing depending on what the researcher does with the output, what they would have done without it, whether they engage critically with what comes back, whether the practice they are skipping is one they need to keep. The methodology will not provide a clean rule. What it can provide is a framing that makes the question visible at every choice, and a set of practices that bias the answer in the right direction.

This framing does not solve the problem. It names the problem so the methodology can address it instead of optimizing for output and hoping the researcher's capacity takes care of itself. The five directions in [`02-implications.md`](02-implications.md) are first attempts at what empowerment looks like in practice. The methodology in [`../methodology/guidelines.md`](../methodology/guidelines.md) accumulates concrete guidelines, each evaluable against the empower/replace question.

Empower-not-replace is not a slogan to repeat. It is a question the researcher asks at every step where AI is used, and a question the methodology has to make easy to ask.

## 7. What this repo is

The aim is not to publish a finished framework. It is to record an inquiry — what was read, what was tried, what worked, what didn't, what was changed and why — in a form another researcher can read along with and borrow from.

The structure: the diagnosis lives in [`foundation/`](.) — this document, [`01-ai-attributes.md`](01-ai-attributes.md) (the catalog), [`02-implications.md`](02-implications.md) (gestures toward methodology), [`03-open-questions.md`](03-open-questions.md) (what is still open). The deeper literature synthesis on innovation that §4 above draws on lives in [`../evidence/literature-notes/innovation-as-different-operation.md`](../evidence/literature-notes/innovation-as-different-operation.md). The methodology lives in [`../methodology/guidelines.md`](../methodology/guidelines.md), grows from evidence, and starts with the initial guidelines drawn from this foundation. The evidence lives in [`../evidence/`](../evidence/). The chronicle of how the inquiry has changed lives in [`../log/`](../log/). Real research projects, when applied, will live in [`../case-studies/`](../case-studies/).

The methodology will never be finished. AI is changing. What works changes with it. A foundation that treats "under construction" as a phase ending in some future v1.0 will be wrong by the time v1.0 ships. The repo's structure is the inquiry. The first imperfect version beats the perfect-but-future version, every time.

The repo is not currently accepting external contributions. It is deliberately one researcher's working artifact, in public, while the foundation is being developed and the pilot research domain is being chosen. Reach out through the contact in [`../CONTRIBUTING.md`](../CONTRIBUTING.md) if you have substance to offer — an interview, a structured experiment, a contradiction that bears on the foundation.

The repo will be wrong about things. It will revise. It will retire guidelines. The point is that the revisions are visible.

---

*Last revised 2026-05-06. Substantial rewrite to a walk-through structure: how research has worked, how technology has historically changed knowledge work, why AI is structurally different from prior tools, why this forces reimagining research specifically, why now, and the mindset shift the rest of the methodology operationalizes.*
