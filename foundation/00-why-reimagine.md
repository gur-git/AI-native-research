# Why reimagine research

A note before the methodology: an explanation of why the inquiry is necessary at all. The argument here is that AI is not just a faster tool for existing knowledge work — it shifts the cost structure of that work in ways that force the work itself to reorganize. Research is one case among many. It is a particular case worth studying on its own because of structural properties research has that most knowledge work does not.

---

## 1. What is happening to knowledge work generally

For most of the history of professional knowledge work, the cost structure looked like this:

- **Producing a draft** of anything — a paragraph of prose, a paragraph of code, a chart, an analysis, a literature summary — was *expensive* in human time.
- **Judging a draft** — deciding whether it was right, useful, well-suited to its purpose — was *cheap* in comparison, because the person doing the judging was usually the person who had just produced the draft, and they had context.

So the binding constraint was production. Workflows, training, hiring, careers, institutions all optimized for it. A junior employee's job was to produce drafts; their value compounded as they became faster and more accurate at it.

In the last three years, this cost structure has been inverted in many domains. Fluent first drafts of text, code, summaries, analyses, charts, and translations are now produced by AI in seconds, at near-zero marginal cost. The remaining expensive operation is **judgment** — deciding whether the draft is right, whether it answers the actual question, whether it is missing something the requestor needed but did not specify.

The pattern repeats across surprisingly different domains:

- **Software engineering.** Writing a function used to be the work; now writing a function is a prompt away, and the work is verifying that what came back actually does what the system needs, without breaking anything else. The METR 2025 study captures the consequence: experienced developers using frontier AI tools were measurably 19% slower at completing real tasks while *believing* they were 20% faster, because the new bottleneck (verification, integration, correction) is less visible than the old one (typing).
- **Customer service.** Producing a coherent reply was the operation; the human's value was speed and tone. Most coherent-reply tasks are now resolved by AI without a human in the loop, and the residual human work is the difficult cases where judgment, escalation, or empathy is the actual deliverable.
- **Education.** Producing a tailored explanation of a topic at a student's level was costly enough that personalized instruction was a luxury. It is now cheap. The expensive work has shifted to assessing whether students actually learned, and to designing curricula that AI cannot trivially shortcut.
- **Legal research.** Finding relevant precedent and summarizing it was the bulk of a junior lawyer's time. AI does this faster than the lawyer, with caveats about hallucinated citations. The remaining hard work is judgment about which precedents matter, how they interact, and what argument they support.
- **Writing and journalism.** Producing a serviceable draft is fast. Producing a draft that is *true*, original, and worth a reader's time is slow — and is the part AI is most likely to misjudge if left to evaluate itself.

The pattern is general. Wherever the historical cost structure was "production expensive, judgment cheap," the new structure is "production cheap, judgment expensive." Domains that respond to this by trying to do the same things faster — by treating AI as a cheaper version of the old workflow — tend to produce more output of unverified quality. Domains that respond by reorganizing — by promoting judgment, verification, and selection to first-class operations — tend to produce work that is honestly better.

This is the broad phenomenon. AI does not speed up old workflows uniformly; it reweights which steps in those workflows matter.

## 2. Why research is a particular case

Research has structural properties that make it especially sensitive to this reweighting.

**Research's defining operation is the verification of novel claims.** Most knowledge work serves an audience that mostly trusts the producer; research serves an audience whose job it is *not* to trust. A claim in a paper is supposed to survive review, replication, and adversarial examination. The verification of novelty is exactly the operation AI is structurally bad at, for reasons cataloged in `01-ai-attributes.md`. So research feels the inversion sharply: the new bottleneck (judgment, verification, selection) is the part of research that always was hardest, and the new cheap part (drafting, summarizing, exploring known terrain) is the part research always could afford.

**Research has no clean unit-of-output.** Most knowledge work produces deliverables that are evaluated discretely — a ticket closed, a customer issue resolved, an article published. Research produces understanding, which accumulates across years and is judged retrospectively. This makes research particularly vulnerable to the perception gap: a researcher feeling "AI is making me 50% more productive" has no near-term mechanism to falsify that, and may be 30% less productive in practice. The METR finding, which is for software engineering, is about the most measurable knowledge work there is. In research, the gap between felt and real productivity is likely worse, not better, because the feedback loops are slower.

**Research depends on cumulative state across sessions, projects, careers.** A researcher's value compounds because their understanding of a problem deepens over months and years. AI sessions, by default, do not compound at all. A workflow that leans heavily on AI without specifically engineering the cumulative state can quietly lose the very thing that makes research possible — the slow, deepening grip on a problem.

**Research has higher stakes for fluent-but-empty output.** A bad draft of a customer email costs an apology. A bad draft of a research claim, fluent enough to pass internal review, can mislead a field for years. The Sakana AI Scientist evaluation found that the system produced manuscripts that "many reviewers might struggle to distinguish" from real work, while also producing 42% experiment failures from coding errors and "hallucinated numerical results." This is what happens when AI is allowed to do research-shaped output without the verification structures research demands.

**Research is more sensitive to direction than to speed.** Software engineering, journalism, customer service — these have well-specified targets, and the problem is mostly to hit them faster. Research is a process of choosing what target to hit, and the choice itself is the value. AI is excellent at producing plausible candidate directions and structurally bad at distinguishing genuinely promising ones from ones that merely sound novel. A research workflow that lets AI pick directions, even subtly, is one that drifts toward the well-trodden — which is exactly the work the researcher should not be doing.

For these reasons, the response to AI in research cannot be the same response as the response to AI in adjacent domains. Faster drafting helps. Faster lit scans help. Faster code helps. But these do not by themselves answer the new bottleneck — judgment, verification, selection, and cumulative state — and pretending they do produces work that is more, but not better.

## 3. Why now, and why this repo

The capability moved fast. Three years ago this conversation was speculative; today it is overdue. Universities and labs are largely *not* adapting their structure — they are adopting tools. The default trajectory is that researchers will continue to use AI as a faster version of the old workflow, will continue to produce more output of less-verified quality, and will continue to feel productive while being measurably less so.

There is a window in which a researcher who actually reorganizes their workflow — who treats verification and selection as primary, who maintains explicit cumulative state, who measures rather than feels — has a compounding advantage. The same window is one in which bad practices ossify across the field. AI-assisted papers without verification trails, hallucinated citations entering the literature, productivity claims that nobody checked: these are accumulating now. They are easier to push back on early than late.

This repo is one researcher's attempt to think through what an honest reorganization looks like, in public, while applying the result to a real research project. The aim is not to publish a framework. It is to record an inquiry — what was read, what was tried, what worked, what didn't, what was changed and why — so that another researcher reading along can borrow what is useful and discard what is not.

The structure of the inquiry: the diagnosis (this file and `01-ai-attributes.md`) is settled enough to write down. The methodology (`methodology/guidelines.md`) is mostly empty by design and grows from evidence (`evidence/`). The case studies (`case-studies/`) will hold the pilot research project once a domain is chosen. The log (`log/`) carries the chronicle.

The repo will be wrong about things. It will revise. It will retire guidelines. The point is that the revisions are visible.

---

*Last revised 2026-05-05. Initial draft.*
