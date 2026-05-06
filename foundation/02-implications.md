# Implications for methodology (gesture, not commitment)

The diagnosis in [`00-why-reimagine.md`](00-why-reimagine.md) and [`01-ai-attributes.md`](01-ai-attributes.md) points toward a research workflow that looks structurally different from current practice. This file gestures at what the difference might be. It is explicitly **not** the methodology. The methodology lives in [`../methodology/guidelines.md`](../methodology/guidelines.md) and is built up from evidence over time.

The point of this file is to keep the diagnosis from sitting alone — to show what kinds of practices the foundation seems to call for. Every gesture here is a hypothesis the methodology will eventually test, not a finding.

---

## The meta-frame: empower, not replace

Before any individual gesture, one principle frames all of them. The diagnosis in `00` §5 names the choice the methodology exists to make: AI used in ways that grow the researcher (empower), versus AI used to produce outputs the researcher could not have produced themselves and now will not learn to produce (replace).

Every gesture in this file, and every guideline in the methodology, should be evaluable against the question: *will the researcher be more capable as a result of this practice, or less?* Practices that look efficient but quietly substitute for skill development are not improvements over the default — they are the default. Practices earn their place in the methodology by passing the empower/replace test, not by being clever.

This meta-frame is what distinguishes the four cluster-level directions below from a generic "AI productivity" framework. The same observation about cheap idea generation could lead to "use AI to generate more ideas" (replacement, in the sense of substituting AI's volume for the researcher's developing taste) or to "use AI's cheap idea generation to feed the researcher's selection practice and develop their taste over time" (empowerment). The directions below try to consistently take the second option.

---

## The five directions the diagnosis pulls toward

### From cluster I (asymmetric competence)

If idea generation is now nearly free and selection is the binding constraint, the unit of research may need to shift from *project* to *portfolio*. The relevant skill is no longer only "produce one good idea and execute it" — it is also "run several threads, prune them on signals the researcher learns to read, develop the survivors." The empowering version of this is one where the researcher's taste develops through repeated direction-and-outcome practice. The replacing version is one where AI ranks the threads and the researcher rubber-stamps the ranking. The methodology has to bias toward the first.

### From cluster II (subtle, fluent, biased failures)

If verification cannot be entrusted to the same system that generates, then verification has to be promoted from "the last step" to a structural commitment that shapes earlier steps. A workflow that decides what would convincingly verify *before* designing the experiment is different from one that designs the experiment first and figures out verification later. Verification is also the part of the workflow most likely to develop the researcher when done well — formalizing claims, looking for missing controls, replicating others' work all build skills that whole-task outsourcing erases.

### From cluster III (no accumulation)

If AI does not carry state across sessions, the human's role becomes the carrier of cumulative state, and that state has to live somewhere external — version-controlled, re-loadable, designed for re-grounding new sessions. This is not a tooling problem; it is a craft. The shape of the external state, and the discipline of maintaining it, is itself a methodology to be developed. Maintaining external state is itself a skill that compounds: the more practiced the researcher is at deciding what to log and at what grain, the more useful their log becomes — both to AI sessions and to their future self.

### From cluster IV (we can't trust our perception)

If felt productivity does not match measured productivity, the methodology has to include some form of measurement, however crude. A researcher who cannot describe whether AI helped or hurt them last week, with at least some grounding in observation, is operating on vibes. The honest minimum is personal calibration data — likely an n=1 self-experiment that accumulates over a year. The act of building this data is itself a developing capacity; over time it becomes the researcher's instrument for noticing their own drift, which is exactly the capacity A16 (output without reciprocal skill development) makes precarious.

### From cluster V (AI changes the user)

If AI is the first tool that produces output without requiring reciprocal skill development, and if research tasks resist clean decomposition, then the methodology's first job is to make the empower/replace question visible at every choice. Specific gestures:

- **Refuse whole-task outsourcing on tasks that resist decomposition** — even when partial outsourcing is awkward and slower. The slower path is the one that develops the researcher; the awkwardness is the price of that development.
- **Track the second output (researcher development) as deliberately as the first (the deliverable).** A researcher's growing capacity is invisible by default; deliberate tracking — what was harder a month ago, what looks easy now, what skills are atrophying — is the only way to keep it from being lost.
- **Use AI as terrain map rather than as agent.** Ask AI to map the known thoroughly so the human can see where the map ends. Ask AI to produce the obvious objections so the human can notice the non-obvious ones. The human stays in the navigation; AI provides the map.

These are the gestures the empower-not-replace mindset most directly implies. They are also the gestures most absent from existing AI-for-research practice.

---

## What this file is not

- Not a list of guidelines. Guidelines live in [`../methodology/guidelines.md`](../methodology/guidelines.md), have status (`proposed`, `testing`, `adopted`, `retired`), and require evidence trails. The gestures here are inputs to that process, not outputs of it.
- Not the methodology. The methodology is something this repo grows over time, not something it asserts upfront.
- Not exhaustive. The diagnosis may pull in directions that have not been articulated yet, and the methodology may surface practices these gestures do not anticipate.

The honest position: the five directions above are where the inquiry expects to find its first guidelines, but that expectation should be tested, not assumed. The methodology will refine, retire, and add directions as evidence accumulates.

---

*Last revised 2026-05-06. Reframed around empower-not-replace as the meta-frame for all directions. Cluster V (AI changes the user) added as a fifth direction. Original four-direction draft from 2026-05-05 is preserved in `log/`.*
