# Step 0 landscape scan — round 2 expansion and format refinement (2026-05-17)

Second round on the step-0 public-positions scan, in response to maintainer feedback on the round-1 output: broader coverage of practicing scientists and heavy AI users (round 1 underweighted both), explicit inclusion of Alex Wissner-Gross / PSI (called out by name), and two format changes (uniqueness integrated into each vector's explanation; players appendix added).

Source doc updated in place: [`../evidence/survey-2026-05/step-0-landscape.md`](../evidence/survey-2026-05/step-0-landscape.md). Round 1 history visible in git.

## What was done

Three subagents ran in parallel, covering 27 entities not in round 1:

- **AI-side actors missed in round 1**: Alex Wissner-Gross / PSI (deep), Yann LeCun / AMI Labs, xAI, Microsoft AI / Suleyman, Apple ML Research, Mistral AI, Cohere.
- **Practicing scientists with public AI-methodology positions**: Terence Tao, Andrew Ng, Jeremy Howard, Eric Topol, George Church, Sébastien Bubeck, Patrick Collison, Lior Pachter, John Carmack.
- **Heavy AI users + research tools missed in round 1**: Matt Welsh, Sebastian Raschka, Cassie Kozyrkov, Cal Newport, Hadley Wickham, Patrick Mineault; Consensus, Scite, SciSpace, Causaly, Connected Papers, Litmaps, Iris.ai, Humata.ai, Genei.

Total now canvassed across both rounds: 47 entities. Format changes folded into the same doc.

## What changed in the inquiry's understanding

**The five-vector taxonomy held**, but each vector grew and a few sub-patterns sharpened.

- **Vector 1 (agentic delegation)** gained Wissner-Gross / PSI, Microsoft AI / Suleyman, SciSpace, and Welsh (as a role-metamorphosis variant). The major addition is a named pattern — **tactical augmentation, strategic replacement** — visible most clearly in PSI (GPD treats agents as "graduate students, not autopilots" while *Solve Everything* describes physics being "steamrolled by well-targeted generalist AIs") and Microsoft AI ("Humanist Superintelligence" + 12-18 month total-automation prediction held simultaneously). The pattern is implicit across the delegation vector but the two new entries make it explicit and namable. *Worth carrying into the foundation as a named foil for empower-not-replace.*

- **Vector 3 (craft / skill preservation)** grew substantially and is now the largest vector by player count. Practicing scientists (Tao, Topol, Howard, Church, Pachter, Mineault) reach craft conclusions independently of the AI-tools discourse. They display a consistent frame absent from the AI-lab voices: **what the researcher must preserve** — formal verification, comprehension loops, RCT evidence, mechanistic interpretability, capacity for dissent, metacognition. *Worth carrying into the foundation as a cross-cutting observation: the practicing-scientist camp thinks about methodology differently from the AI-lab camp, and the inquiry has more material to draw on from the former.*

- **Vector 4 (governance / cautionary)** gained an architectural-empirical sub-position: LeCun's architectural critique (current AI is on the wrong substrate for science) + Apple's "Illusion of Thinking" empirical demonstration. *Worth a literature-note-grade read together.*

- **Vector 5 (silence)** broadened: xAI, Mistral, Cohere on the AI-lab side; Humata, Genei, Iris.ai on the tool side; Collison at the individual level (institutional/funding contributor, no personal methodology essay). Confirms that opting out of methodology debates is a coherent corporate choice, not just oversight.

- **No new vectors needed.** Welsh's metamorphosis position fits as a delegation sub-case. LeCun's architectural critique sharpens but doesn't break Vector 4. Wissner-Gross's bifurcation is a tension within delegation, not a new camp.

## Findings most worth carrying into the foundation

In rough order of weight:

1. The **"tactical augmentation, strategic replacement"** pattern is now a named contrasted position. Naming it explicitly in `foundation/00-why-reimagine.md` (probably §1 or §4) would sharpen the empower-not-replace argument by giving the reader a concrete foil.
2. The **working-scientist vs AI-lab frame difference** — "what must the researcher preserve" vs "how to design the workflow" — is a useful observation about where the repo's substantive material is most likely to come from in stages 3-4 of the survey. Possibly worth a cross-cutting note in the foundation about what kinds of evidence sources the inquiry will favor.
3. The **pedagogical problem** (Mineault) — junior researchers cannot develop the metacognition to use AI well when AI hides its mistakes — is the most precise statement yet of a question the foundation already gestures at via A16 in [`foundation/01-ai-attributes.md`](../foundation/01-ai-attributes.md). Worth strengthening the A16 entry with this framing.
4. **Topol's clinical-RCT epistemology** is a potentially generative move: it imports a research field's gold-standard evidence layer into AI-methodology decisions. Worth investigating whether the same move works elsewhere — could become a methodology guideline.

## Still open

- Round 2 deepened most of the round-1 stage-3 candidates and added two new ones (LeCun + Apple as a paired literature-note; Topol's epistemology as a possible generalizable move). The full updated list is in §6 of the step-0 doc.
- Stage 1 (territories map) is still the next concrete step in the survey plan. Round 2's working-scientist findings give clearer hooks for which territories will matter most: cognitive psychology of skill formation (Mineault), formal verification (Tao), clinical-trial epistemology (Topol), mechanistic interpretability as scientific requirement (Church), AI's effect on community power dynamics (Pachter).
- The 47-entity sample is still not a census. Domains intentionally not yet canvassed: HCI augmentation lineage, history-of-science accounts of past tool transitions, cognitive psychology of skill, research-software-engineering literatures. These belong in the deeper survey, not in step 0.
