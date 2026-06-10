# The methodology

This document is the bridge between the repo's theoretical backbone and the practical artifact researchers use. It states, as of its last revision, how this inquiry currently believes AI-native research should be done: the principles, the working posture, the process, and the practices — each traced to the foundation and to evidence, each carrying a status. The **starter repo** (the template workspace a researcher actually works in) is the executable view of this document; where the starter and this document disagree, this document is the source and the starter has drifted.

**Status of the whole:** everything here is `proposed` — a working answer under live test by the pilot, not a validated result. The practice registry below tracks each practice individually. The central revision this document carries (the gate-carried posture, 2026-06-10) is a falsifiable bet, tracked as open question Q13 ([foundation/03-open-questions.md](foundation/03-open-questions.md)).

---

## 1 · Principles

Derived from the foundation; stated here compactly, with the reasoning at the links.

1. **Research has two outputs: the artifact and the researcher.** The second is built through the work itself and is invisible until it's missing. AI is the first tool that produces output without insisting on the user's growth, which puts the second output silently at risk ([GOAL.md](GOAL.md) §What changed about research; [foundation/00-why-reimagine.md](foundation/00-why-reimagine.md)).
2. **Empower, not replace — judged at the whole-job level.** The question is never "did the researcher do this themselves?" but "is the researcher's capacity to do the job, at the level it is judged on, growing or shrinking because of how AI is used here?" Low-level skills are fine to lose; the line moves as AI improves ([GOAL.md](GOAL.md) §The commitment).
3. **AI's competence is asymmetric and its failures are fluent.** Breadth, transfer, parallelism, and idea-volume are nearly free (attributes A1–A4); confidence does not track correctness, self-validation is the default, agreement is the trained disposition, and hallucination concentrates exactly at the research frontier (A5–A9). Selection and verification are therefore the scarce human work ([foundation/01-ai-attributes.md](foundation/01-ai-attributes.md)).
4. **Nothing accumulates and nobody's perception is reliable.** Sessions forget (A10–A12); felt productivity and felt understanding are measurably miscalibrated (A13–A15). State lives in owned, version-controlled files; development is measured by records, not impressions.
5. **Every practice must trace.** A practice that cannot name the attribute it answers, the evidence behind it, and the skill it develops or protects does not enter the registry. Practices are retired when evidence turns against them; the retirement is kept visible.

## 2 · The posture: AI as a junior colleague

*(proposed; evidence: [pilot team meeting](evidence/interviews/2026-06-10-pilot-team-meeting.md), [pilot workspace audit](evidence/observations/2026-06-10-pilot-workspace-audit.md); revises the earlier advise-don't-author posture — see the registry, G5.)*

The agent works like a junior colleague: it does the heavy lifting — searching, gathering, drafting, building, formatting, writing every document in the workspace — and is never fully trusted. The researcher contributes through conversation: framing, choosing, judging, articulating, deciding. Nothing in the methodology requires the researcher to author a document.

What the posture does **not** relax:

- **Decisions stay the researcher's.** Direction, commitments, what counts as done — the agent advises, surfaces trade-offs, and may disagree on record; it does not decide ("what should I do next" is never the agent's to answer).
- **Trust stays conditional.** Anything load-bearing the agent produced gets verified from a source independent of the agent (G3) before the work stands on it.
- **The second output stays a tracked deliverable** — carried by gates (below) instead of by authorship.

The bet, stated honestly: that verified understanding plus decision practice can build what doing-the-work used to build. The original foundation argument says the apprenticeship lives in the peripheral work itself; this posture wagers that the apprenticeship can be carried by articulation and judgment instead. Q13 tracks it; the pilot tests it. If gate records pass while external signals of the researcher's development stagnate, this posture — not the principle — is what gets revised.

## 3 · Gates

*(proposed; evidence: [professor interview](evidence/interviews/2026-06-10-professor-classical-research-steps.md) — the classical explain-back instrument; [pilot audit](evidence/observations/2026-06-10-pilot-workspace-audit.md) — the teach→quiz loop that survived the posture relaxation and caught a real gap.)*

A **gate** is an interview-conversation at a point where something is about to be relied on — a concept about to be built upon, a paper about to inform a design, a direction about to be committed to, a result about to be claimed. Gates are how progress is verified and how the second output is built and measured, given a researcher who works through chat.

The protocol:

- **An interview, not a test.** The agent asks questions whose answers the work genuinely needs — derivations about to become design choices, "what breaks if…" probes about to become constraints. The gate's output is a contribution to the research (a sharper formulation, a surfaced edge case, a gap that becomes a question), never just a verdict. A gap found is a finding, not a flunk; if the gap traces to a flawed artifact (an unclear note), the artifact gets fixed too.
- **The goal-gradient.** Early in a project the dominant goal *is* becoming knowledgeable, so gates legitimately lean test-like — articulating the answer is itself how the knowledge becomes whole. Later, the same primitive leans toward design-probing and decision-defense. The gate serves whatever the current goal is.
- **Closure.** The agent closes the gate by default, when the conversation has stopped producing value — when the next question would only test rather than build. The agent may vote to stay longer if it judges there is more to gain. The researcher can override and close at any time, as a last resort: the override is recorded in one line and never argued.
- **Honesty rules (hard lines, agent-enforced).** No generous passes — a record with no failures indicates a soft grader (A7), not mastery. Nothing is marked understood, closed, or done except through a gate. A gate that surfaced unresolved gaps cannot conclude "solid." Where the subject is at the research frontier, the agent's own corrections are suspect (A5, A8) and must be grounded in a source the researcher can open.
- **Stamps and records.** Gate outcomes stamp the artifacts they verify (a knowledge note without a stamp is visibly just AI output) and leave a transcript in the workspace records. Those records are the raw material for tracking the second output (registry, G6) and for testing Q13.

## 4 · Modes

*(proposed; evidence: pilot team meeting — chat-first preference; the mode definitions are design, marked as such.)*

The agent has named modes, introduced to the researcher at onboarding and invocable by name — part of the user-facing vocabulary, like skills:

- **Work mode** (default): the agent builds, edits, gathers, maintains the workspace.
- **Conversation mode**: read-only; short, conversational replies; nothing in the repo changes. Triggers: every gate runs in it by definition; every researcher-reserved decision drops the agent into it (stop producing, start talking); and thinking-out-loud signals — the researcher exploring, venting, asking "what do you think." Exit is explicit (the researcher releases it), and the agent's first act after release is to summarize what the conversation concluded — which becomes the input for any edits and doubles as the gate record.

## 5 · The process

*(proposed; the arc composes the registry's practices into an order. The decomposition is a reasoned overlay — phases recur and interleave; entry is flexible (a mid-project researcher starts where they are). Evidence for the early-phase structure: the professor interview; the rest derives from the foundation as before.)*

0. **Onboard.** The first session is an interview (in conversation mode, and says so): who the researcher is and what they want from the research; where the work currently stands; the interaction contract — the methodology's defaults proposed, the researcher's adjustments recorded; which skills fit their stage. The agent introduces the workspace, the modes, and the gates. Output: a seeded profile, a seeded state file, a recorded contract. *(G22)*
1. **Learn the field.** The agent maps terrain — sources, structure, the questions a concept must answer — and drafts the knowledge notes; the researcher builds understanding through conversation over them; **gates close each unit** (early-phase, test-leaning — that is the goal being served). Knowledge the work will rely on carries a stamp. *(G13, G10, G16/G20, G4)*
2. **Focus.** Divergence wide and cheap (with fresh outside scanning, not reframes-only), then selection against the researcher's own ranking first — the agent withholds its ranking until the researcher has committed theirs, then the two are reconciled deliberately; divergences are the signal. The phase exits through a **research proposition** — motivation/background, system model, problem formulation, existing approaches, the proposition — owned by the researcher through conversation, attacked before adopted. Commitment is a researcher-reserved decision, made with the mentor where one exists. *(G8, G13, G17, G9, G19)*
3. **Design and build the MVP.** Verification decided before building (what would falsify this; what would a hostile reviewer say). Bias toward the smallest end-to-end artifact that can confront reality — the build is cheap now; the simplifications that define it are load-bearing choices and stay the researcher's, defended at a gate. *(G9, G18, G4)*
4. **Execute and iterate.** The agent produces; the researcher steers, judges, and owns the moves where a parameter choice becomes a claim about the world. Cheap building multiplies candidates; the verification bill does not shrink (A9). *(G3, G15)*
5. **Verify.** Independent-source verification for anything that will be relied on or asserted: fetched-and-read sources for every load-bearing citation (an unresolvable reference stops the work), replication where stakes warrant it, expert human eyes — the one critic whose independence from the generator is categorical (A6) and whose strength peaks at the frontier where AI's fails (A8). Experts see the work early and in parallel, not at the end. *(G3, G10, G14, G19)*
6. **Share and respond.** The claim, its framing, and its defense are the researcher's, exercised in their own person; the agent adapts formats and surfaces which objections map to known weaknesses. *(G1, G9)*

Cross-cutting, every phase: state carried in the workspace cursor and store (G2); the exploration share protected against the exploitation gradient (G12); periodic review conversations over the gate records (G6); the empower/replace question made visible at the moments that matter (G1).

## 6 · The workspace

*(proposed; implemented by the starter. The cursor/store split and the death of researcher-written ledgers: 2026-06-10 design decisions from the pilot evidence.)*

- **`state.md` — the cursor.** Where the research is *right now*: current question, decided directions, dead ends, open threads, next step. Small, rewritten freely, loaded every session, points into the store. The session ritual (load at start, update at end, re-ground on drift) answers session forgetting (A10).
- **`context/` — the store.** Accumulates. `profile.md`: who the researcher is, their goals, the interaction contract. `knowledge/`: the research substance — concept notes, paper notes, terrain maps — agent-written, gate-stamped. `records/`: what gates leave behind — transcripts, stamps, overrides, decision records. Nothing here asks the researcher to write; everything here lets them verify and remember.
- **`FRICTION/` — the upstream channel.** The agent drafts dated entries in the background (what chafed, what was ignored, what was overridden) — about the methodology, never the research, readable out of context. The researcher may add notes of their own. The methodology's maintainers read these by arrangement (pull, not push) in the early-user phase.
- **Provenance** is carried inline: authorship/status headers on artifacts (agent-drafted vs. researcher-owned, gate-stamped or not) rather than separate metadata files — the form the pilot actually used (G15, reframed).

## 7 · Practice registry

The revisable layer. Numbers are stable and never reused; statuses move only on evidence. Full prior texts of G1–G19 survive in git history (`methodology/guidelines.md`, retired 2026-06-10); entries below are the current form. Attribute numbers refer to [foundation/01-ai-attributes.md](foundation/01-ai-attributes.md); evidence links are the trail.

| # | Practice | Status | Disposition 2026-06-10 |
|---|----------|--------|------------------------|
| G1 | **Ask empower-vs-replace at the whole-job level.** The controlling question — *is my capacity at the level the job is judged on growing or shrinking?* — asked at gates and decisions, not keystrokes. (A16, A17) | proposed | Kept; the question now lives at the gates. |
| G2 | **Carry state in owned, version-controlled files.** Split: `state.md` cursor + `context/` store; session ritual at start/end. (A10, A11) | proposed | Reframed (cursor/store split); the pilot's heaviest-used practice. |
| G3 | **Verify from a source independent of the generator.** Formal checks, fetched primary sources, replication, or a human who hasn't seen the session — before anything load-bearing stands. (A6, A8, A9) | proposed | Kept; carries more load than ever under the junior-colleague posture. |
| G4 | **Classify the task: recombination or innovation.** Sets delegation freedom and gate strictness; when in doubt, treat as innovation. (A1, A4) | proposed | Kept. |
| G5 | **Refuse whole-task outsourcing on non-decomposable tasks.** (A17) | **retired** | Retired 2026-06-10. The pilot would not work this way ([meeting](evidence/interviews/2026-06-10-pilot-team-meeting.md), [audit](evidence/observations/2026-06-10-pilot-workspace-audit.md)); authorship rules read as busy-work and drove rejection of the posture wholesale. Replaced by gate-carried apprenticeship (G20) — a bet tracked at Q13. Post-mortem in the [log](log/2026-06-10-posture-revision-and-redesign.md). |
| G6 | **Track the second output through gate records.** Gates generate the records; a periodic review *conversation* (not a researcher-written log) walks them: what was delegated and might be atrophying, what got easier, where overrides cluster. (A13, A16) | proposed | Reframed from researcher-written capability log — the pilot wrote no ledger entries in a month. |
| G7 | **Calibrate felt against measured.** The felt-vs-actual signals (time, helpfulness, understanding) are captured in records as work happens and reviewed in the G6 conversation. (A13, A15) | proposed | Reframed from a researcher-maintained ledger, same reason as G6. |
| G8 | **Rank before the agent ranks.** On any candidate set, the researcher commits a ranking (in conversation — a sentence each suffices) before seeing the agent's; divergences reconciled deliberately. (A4, A5, A7) | proposed | Kept; chat-native already. |
| G9 | **Attack before adopting.** Pre-mortem prompts (*what would falsify this? what control is missing? what would a hostile reviewer say?*) before designs, propositions, and claims are committed. (A6, A7) | proposed | Kept. |
| G10 | **Treat AI literature output as a starting graph; fetch before relying.** Every load-bearing citation resolves to a fetched, read source or the work stops (no deep-read of an unfetched paper); the researcher engages the load-bearing sources at the relevant gates. (A8) | proposed | Reframed: the pilot's verify-before-cite STOP rule absorbed; the researcher's source contact moves to the gates. |
| G11 | **Record direction decisions and their outcomes.** Commitment gates leave decision records (chosen, rejected, why); outcomes are attached as they arrive; reviewed in the G6 conversation to develop taste. (A4; Q7) | proposed | Reframed from a researcher-written log into gate records. |
| G12 | **Protect the exploration share.** A deliberate fraction of effort goes to work aimed at no current deliverable; the agent notices when everything lately is refinement of one thread and says so. (A4) | proposed | Kept. |
| G13 | **AI maps terrain; the researcher navigates.** The agent lays out options, costs, adjacencies — and never answers "which way should I go." (A1, A2, A8) | proposed | Kept; under the new posture this is the sharpest remaining line. |
| G14 | **Replicate a recent paper periodically.** A verification primitive and a depth practice; cadence quarterly as a starting point. (A6, A9) | proposed | Kept, untested (Q5). |
| G15 | **Carry provenance inline.** Authorship/status headers (agent-drafted vs. researcher-owned, gate stamps, dates) on artifacts; model+date noted for relied-on syntheses. (A12) | proposed | Reframed to the form the pilot actually practiced. |
| G16 | **Gate knowledge with explain-back interviews.** The researcher explains, notes shut; the agent probes with understanding-questions and corrects from openable sources; only a genuine pass closes a concept. (A13, A16; A5, A7, A8 shape the caveats) | proposed | Reframed into interview vocabulary (a found gap is a finding); the specific knowledge-phase form of G20. Two convergent (not independent) sources: the professor's classical instrument, the pilot's quiz. |
| G17 | **Converge focus into a five-part research proposition.** Motivation/background, system model, problem formulation, existing approaches, the proposition — owned by the researcher through conversation (the agent transcribes; the phrasing decisions are the researcher's), attacked before adopted, version-controlled. (A4, A7, A8) | proposed | Kept; "authors" now explicitly means *owns through conversation*. |
| G18 | **Build a minimum viable version early; iterate against reality.** Build cost collapsed for recombination parts (A3, with A1 supplying the known elements); the defining simplifications stay the researcher's; the verification bill does not shrink (A9). | proposed | Kept. |
| G19 | **Expert human review, early and in parallel.** From the first MVP onward; the mentor and domain experts see work-in-progress; the researcher presents and defends in person; expert-vs-AI-critique divergence is logged. (A6, A8) | proposed | Kept. |
| G20 | **Gate progress with interview-conversations.** The general protocol of §3: gates at closures and commitments; value-producing interviews; agent closes when value runs out, may vote to prolong; researcher overrides on record; honesty rules agent-enforced. (A5, A6, A7, A13, A16) | proposed | New 2026-06-10; evidence: professor interview + pilot audit + pilot meeting. The load-bearing practice of the revised posture; Q13 tests it. |
| G21 | **Name the modes; let the researcher steer them.** Work mode and conversation mode, introduced at onboarding, invocable by name; conversation mode for gates, reserved decisions, and thinking-out-loud; exit by explicit release, followed by a summary of what was concluded. (A7, A17) | proposed | New 2026-06-10; evidence: pilot meeting (chat-first preference). |
| G22 | **Onboard through an interview that sets the contract.** First session: who the researcher is, their goals, where the work stands, how they want to work — defaults proposed, adjustments recorded in the profile; the workspace, modes, skills, and gates introduced proactively. (A16; the interface evidence) | proposed | New 2026-06-10; replaces the written intake the pilot deleted. |

## 8 · The starter mapping

The starter repo is the executable view of this document. What implements what:

| Starter element | Implements |
|---|---|
| `README.md` | The discoverability contract: everything the researcher must know is either here (what this is; the modes and skills by name; "tell your agent to start") or said proactively by the agent. |
| `CLAUDE.md` | The posture (§2), modes (§4), gate protocol and hard lines (§3), session ritual (G2), provenance (G15), the proactive-explanation duty, and the pin back to this repo + the `updates/` path. |
| `state.md` | G2 (cursor). |
| `context/profile.md` | G22's output: who, goals, the interaction contract. |
| `context/knowledge/` | G10, G13, G15, G16 (stamped notes). |
| `context/records/` | G6, G7, G11, G20 (transcripts, stamps, overrides, decisions). |
| `FRICTION/` | The upstream channel (§6). |
| skill `onboard` | G22, G21. |
| skill `gate` | G20, G16 (and the stamp/record mechanics). |
| skill `learn` | G13, G10, G15 — terrain-map and draft a concept, teach it in conversation, hand off to `gate`. |
| skill `paper` | G10, G9 — structured deep-read with fetch-before-write; relevance judged by the researcher at a gate. |
| skill `gather` | G10, G13 — cited web research, per-claim confidence, landscape-not-verdict. |
| skill `ideate` | G8, G13, G17, G12 — divergence with fresh scanning, researcher-first ranking, toward the proposition. |
| skill `session` | G2, G6, G12 — session-end ritual: cursor update, records proposals, friction drafting, drift notices. |
| skill `update` | The downstream channel: reads this repo's `updates/` against the pin, converses item-by-item, applies adoptions, records skips, moves the pin deliberately. |

The sync channels: **downstream**, versioned update documents in this repo's [`updates/`](updates/) — written for the agent (what changed, why, what to ask your researcher) — consumed by the `update` skill; **upstream**, the workspace's `FRICTION/`, read by the maintainers by arrangement during the early-user phase.

## 9 · Revision protocol

- Statuses move only on evidence: `proposed` → `testing` (a deliberate trial is running and named) → `adopted` (the trial's evidence supports it) → `retired` (evidence against, or superseded — kept in the registry with a post-mortem pointer).
- Every revision of this document writes a log entry and, when it changes researcher-facing behavior, an update document in `updates/`.
- New evidence is checked against the open questions ([foundation/03-open-questions.md](foundation/03-open-questions.md)) when recorded — opening and closing questions is part of the work, prompted by the repo's own skills, decided by the maintainer.
- The interface itself (starter form, onboarding shape, gate feel) is an object of study (Q9, Q10, Q13); friction from real use is the primary evidence stream for it.

---

*Created 2026-06-10, merging and superseding `methodology/guidelines.md` (G1–G19 texts preserved in git history), `methodology/ai-native-research-process.md`, and `methodology/agent-operating-guide.md`. The posture revision and its reasoning: [log/2026-06-10-posture-revision-and-redesign.md](log/2026-06-10-posture-revision-and-redesign.md).*
