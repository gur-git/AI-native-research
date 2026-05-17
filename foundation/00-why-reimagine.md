# Why reimagine research

## 1. How it used to go

A graduate student in 1985 needs a calculation. They sit down with a calculator. They have to know what they want to compute. They have to know what the answer should look like. They have to recognize when the result can't be right — when they entered something wrong, when the answer is off by a factor of ten. And on; the list of things they bring runs long. The calculator does the arithmetic. The student does everything else.

A programmer in 2000 writes in C++ instead of assembly. They no longer hand-tune registers. But they have to choose data structures. They have to reason about types. They have to understand the libraries they pull in. The list is just as long. The compiler does the optimization. The programmer does everything else.

This pattern has held every time a new tool arrived in knowledge work. The tool took over a skill. A new skill took its place — knowing what to ask the tool for, knowing when its answer was wrong, knowing what to do with what it gave you. The skills changed. The user remained skilled.

The pattern held because of a property of those tools we never had to name. **Each one required real skill from the user to do its job at all — skill of whatever kind the tool demanded.** Operating the tool was itself an exercise of skill. So using the tool well *was* the new skill. The output was only as good as the user behind the tool. We never articulated this property because no tool had ever lacked it.

## 2. How it goes now

A graduate student in 2026 needs a literature review. They open a chat window. They type: *"Write a literature review on X."*

Three minutes later they have something that reads like a literature review. It cites real papers. It is organized into themes. It is fluent. With minor edits it could be turned in.

The student barely had to know what they wanted. They put in a sentence; they got back a draft.

This is the first tool we have ever had that does not need much from the user before it produces something. That asymmetry — sentence in, draft out — is what makes AI useful. The whole point is that you no longer have to bring the kind of competence prior tools required.

It is also what breaks the pattern.

## 3. The break in the pattern

Every prior tool made a clean trade. It took a skill from the user and required a different one in return. The user kept growing because the tool insisted on it.

A real skill set is forming around AI, too — and it is not just prompt craft. It includes the judgment of what to delegate and what to keep, the verification work of telling plausible output from correct output, the recognition of how a particular model fails and where it drifts, the workflow design that keeps the model in the lanes where it works, the taste and domain feel that lets you evaluate what came back. The set is still being mapped; this is illustration, not enumeration. A researcher who develops it gets two things at once: a compensating capacity of the kind prior tools always gave back, *and* materially better results from AI than the unskilled user gets.

But — and this is the structural break — AI does not *require* any of it. The user can produce passable output indefinitely without developing the new skill set at all. The calculator wouldn't compute if you didn't know what to type. The compiler wouldn't optimize if you didn't write the code. AI will give you something usable from one underspecified sentence — usable enough to feel like progress, but qualitatively below what the same prompt would have produced in skilled hands.

This is the structural claim everything else rests on:

> AI is the first tool that can substitute for skill without requiring reciprocal skill development.

The skill is real, available, and rewarding — and it is what separates AI slop from work a researcher should be willing to put their name on. It is also optional in a way no prior tool's compensating skill was. The unskilled researcher gets a worse output *and* gets no growth; the skilled one gets a better output *and* gets growth. The default path is the worse one on both axes, which is a property of how the technology works and not coincidentally the source of its value.

A note on trajectory. As AI capabilities improve, the floor of what an unskilled user can produce will rise — but so will the ceiling of what a skilled user can produce, and the skill set itself will shift as AI shifts. Having the appropriate skill set, whatever its current shape, remains beneficial. The scenario in which the floor catches the ceiling — where even the basic skills of articulating what one wants and recognizing when the output is right stop mattering — would correspond to a regime in which AI works without human involvement at all. This repo does not address that regime.

The methodological response cannot be to wait for AI to require skill from its users. It will not. The response has to be to reorganize how we work — to build into our workflows the practice that the technology no longer extracts from us by default. That reorganization is what this repo means by *reimagining research*.

## 4. Why this hits research hardest

Most knowledge work has one job: produce the deliverable. The report ships, the code merges, the deck lands. Whether the worker grew is somebody else's problem.

Research has two.

There is the artifact — the paper, the dataset, the proof, the code. There is also the researcher — a person who can do harder work next time than they could last time.

The second output is not a side effect. For an early-career researcher in particular, it is most of why the first one matters.

And the second output is built almost entirely by the routine peripheral work that surrounds any research project — reading, analyzing, drafting, testing. The periphery is expensive in human hours. It is also where discriminating judgment forms. **The apprenticeship is not separate from doing the work. The routine work *is* the apprenticeship.**

Now look back at the graduate student with the literature review.

Twenty years ago, that review would have taken weeks. Weeks of confusion, of misreading, of slowly starting to see why this paper matters and why that one is overcited. The review would have been the deliverable. The capacity to read a field is what they would actually have been building.

In 2026 the review takes three minutes. The deliverable is the same, on the surface. The capacity is not built.

There is a second reason research is hit hardest. Most knowledge work applies known patterns to new instances. Research is largely about producing new patterns. AI helps cleanly with the recombination work that surrounds research — summary, restatement, search — and helps poorly with the production of new framings, methods, or hypotheses themselves. The parts AI does well are the parts that double as training. The parts AI does poorly are the parts the researcher most needs to grow into. Outsource the first and you lose the practice that would have built capacity for the second. The deeper treatment of why these two operations are different is in [`../evidence/literature-notes/innovation-as-different-operation.md`](../evidence/literature-notes/innovation-as-different-operation.md).

## 5. The trap, and why the gradient pulls toward it

The natural defense is: *"Use AI for the routine, focus on the hard parts."* In research this assumes the routine and the hard separate cleanly. They rarely do. The fine-grained interleaving of well-trodden technique and original move is most of what makes a task research rather than execution. There is no clean cut.

Even where partial outsourcing is possible — your part, then reviewing AI's part, then integrating — it is more work than either alternative. So the gradient pulls toward whole-task outsourcing because it is the only configuration that is not awkward.

Prior tools made a fair trade — old capacity given up, new compounding capacity gained. AI offers the first deal where the trade is not fair. You give up the practice that built the old capacity, and nothing that compounds takes its place. In principle the hours freed could be reinvested in skill-building. In practice the gradient runs the other way: outsourcing is easy, the output looks like progress, you feel productive, and the metrics that would catch the failure operate on timescales of years.

You can ship strong papers and quietly hollow out as a researcher. You will not notice. By the time you need a capacity that did not develop, you will not remember when you stopped building it.

## 6. Why now

Three years ago this conversation was speculative. Today it is overdue.

Adoption is happening with or without methodology. Researchers are using AI individually, fast, in whatever way feels efficient. Most institutional responses so far have been to adopt the tools, not adapt around them. The default at the institutional level is *"let people figure it out."* The default at the individual level is the trap §5 just named.

Inertia is not neutral. Waiting is a vote for the default.

There is a window. A researcher who reorganizes deliberately — who uses AI in ways that grow them rather than substitute for them — has a compounding advantage in that window. The same window is the one in which the field's defaults are being set. Setting them well requires people doing the work well in the open.

## 7. The response: empower, not replace

The methodological response has to actively preserve and develop the skill AI does not require — at the level the research job is actually judged on.

The choice is no longer whether to use AI. That choice has been made. The choice is whether to use it in ways that empower the researcher or in ways that replace them.

The principle applies at the level of the whole job, not at the level of every micro-task. A researcher who lets AI handle a piece of routine code syntax, a citation format, or a unit conversion has lost a skill — and most of the time that loss is fine. Skills below the level at which research value is created are skills the methodology is comfortable seeing replaced; the replacement is what frees attention for the work that compounds.

What the methodology insists on preserving is the skill set required to do the research job at the level it is actually judged on: framing the question well, designing investigations that would convincingly verify, recognizing when a result is too good, knowing which threads to develop and which to drop, building the taste and the verification habits that make the work trustworthy.

**Empower** means: AI is used in ways that let a researcher do more or better research than they could have otherwise, while continuing to build the capacity that lets them keep doing so — including the capacity to use AI itself well, which is part of what producing valuable research now requires. Every use that crosses the threshold of substantive contribution is evaluable against the question — *will my capacity to do the research job, at the framing at which the job is judged, be greater as a result of this, or smaller?*

**Replace** means: AI is used to produce, at the level the job is judged on, outputs the researcher could not have produced themselves and now will not learn to produce. The output exists. The capacity does not develop, and may atrophy.

The two are not always easy to distinguish in the moment. The same AI prompt can be either, depending on what the researcher does with the output, what they would have done without it, whether they engage critically with what comes back, and whether the practice they are skipping is one they need to keep. The methodology cannot provide a clean rule. It can provide a framing that makes the question visible at the choices that matter — the choices where AI's output would be the substantive contribution of the moment — and a set of practices that bias the answer in the right direction.

The boundary between skills that may be safely replaced and skills that must be preserved is not fixed. As AI improves, it moves upward: capacities that today are central to the job may become routine enough that their replacement is fine, and the preserved skill set shifts to meet the new frontier. The principle is stable. The line it draws moves with the technology.

Empower-not-replace is not a slogan. It is a question the researcher asks at the level of the work as a whole, and a question the methodology has to make easy to ask and possible to answer.

## 8. What this repo is

The compressed charter — the why and how, stated for the repo as a whole — is in [`../GOAL.md`](../GOAL.md). This document is the substantiated long-form of that charter's argument.

The aim is not to publish a finished framework. It is to record an inquiry — what was read, what was tried, what worked, what didn't, what was changed and why — in a form another researcher can read along with and borrow from.

The diagnosis lives in this directory: this document, [`01-ai-attributes.md`](01-ai-attributes.md) (the catalog of AI's specific properties researchers must reckon with), [`02-implications.md`](02-implications.md) (gestures toward methodology), [`03-open-questions.md`](03-open-questions.md). The methodology lives in [`../methodology/guidelines.md`](../methodology/guidelines.md) and grows from evidence over time. The evidence, including the deeper literature synthesis the §4 argument draws on, is in [`../evidence/`](../evidence/). The chronicle of how the inquiry has changed is in [`../log/`](../log/).

The methodology will never be finished. AI keeps changing; what works changes with it. The first imperfect version is more useful than the perfect-but-future one. The repo will be wrong about things; it will revise; it will retire guidelines. The point is that the revisions are visible.

The repo is not currently accepting external contributions. It is one researcher's working artifact, in public, while the foundation is being developed and the pilot research domain is being chosen. Reach out through the contact in [`../CONTRIBUTING.md`](../CONTRIBUTING.md) if you have substance to offer — an interview, a structured experiment, a contradiction that bears on the foundation.

---

*Last revised 2026-05-06. Walk-through structure: how it used to go (calculator, compiler), how it goes now (the literature review in three minutes), the break in the pattern, why research is hit hardest (two outputs, plus AI's asymmetric coverage of recombination vs. innovation), the trap and its gradient, urgency, and the empower-not-replace response.*
