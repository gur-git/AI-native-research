---
name: gate
description: Run an interview-conversation that verifies something about to be relied on — a knowledge note ready to close, a decision about to be committed, a result about to be claimed. The only mechanism that marks anything understood, closed, or done. Triggers when the researcher asks ("gate X"), when another skill hands off at a closure point, or when the agent offers one at a natural closure.
---

# gate

A gate is where the workspace's trust comes from: a passed gate stamps an artifact; nothing gets marked understood, closed, or done by any other route. It is an **interview, not an exam** — its output is a contribution to the research (a sharper formulation, a surfaced edge case, a gap that becomes a question), never just a verdict. It also carries the second output: the researcher's own development, measured by records, not impressions.

## 1 · Open

- Enter **conversation mode** and say so. The gate is read-only talk until the outcome step.
- Name what is being gated and why now (what the work is about to rely on).
- First gate ever in this workspace: explain the mechanism briefly — what a gate is, what a stamp means, that the researcher can close it at any time.

## 2 · Design the questions

Ask questions the work genuinely needs answered next — not questions the existing notes could answer by pattern-matching. Include:

- at least one **work-it-out** question (a derivation, application, or construction the researcher carries through themselves), and
- at least one **why / what-breaks-if…** probe (the answer becomes a constraint or a defense).

**The goal-gradient.** Early in a project, gates on knowledge legitimately lean test-like: articulating the answer is itself how the knowledge becomes whole, because becoming knowledgeable *is* the current goal — say this to the researcher the first time it applies. Later, the same primitive probes designs, selections, and claims: the answers become the design's constraints and the claim's defenses.

## 3 · Conduct

- Ask one question at a time. Let the researcher commit to an answer before revealing anything — no hints, partial answers, or leading follow-ups before they have answered.
- Respond honestly to each answer: correct / partial / wrong, with the correction. Where the subject is at the research frontier, your own paraphrase is not a source — ground every correction in a source the researcher can open.
- **A gap found is a finding, not a flunk.** Work it through in the conversation. If it traces to a flawed artifact (e.g., an unclear note), fix the artifact after the gate and note the revisit in the outcome.

## 4 · Close

- **You close by default** when the conversation has stopped producing value — when the next question would only test rather than build.
- You may vote to stay longer; say plainly what you think is still to be gained.
- **The researcher may override and close at any time.** Record one line in `context/records/` — "closed by researcher; agent saw more to gain: <what>" — and move on without argument.

## 5 · Outcome

- The gate ran in conversation mode; the writes below happen only after the researcher releases it. On release, first summarize what the gate concluded — that summary is the input for the stamp and the record.
- **Genuine pass** (core questions answered with working understanding): stamp the artifact's inline status line — `gate-stamped YYYY-MM-DD` — and write `context/records/YYYY-MM-DD-<slug>.md`: what was gated, a transcript summary (questions, answers, corrections, findings), and the outcome.
- **Unresolved gaps**: no stamp, and never conclude "solid." Write the same record, listing what to revisit; the artifact's status line stays `agent-drafted`.
- Either way, record gaps found and artifacts revised — these records are the raw material for the periodic development-review conversation.

## Hard lines

- No generous passes. A record with no failures means a soft grader, not mastery; if every answer is passing, the questions were too easy — say so in the record.
- Never close a gate over unresolved gaps; never stamp anything by any route other than this skill.
- At the frontier, never correct from your own paraphrase alone — openable source or the correction is marked unverified.
- Never argue an override; record it and proceed.
