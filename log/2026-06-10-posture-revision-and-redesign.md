# 2026-06-10 — The posture revision and the redesign: gates, modes, the starter, and one document

The largest revision since the foundation was written, made in a single deliberate session: a long maintainer conversation (conversation mode, by design) over the day's pilot evidence, concluded by decisions, then executed. The evidence behind it: the [pilot team meeting](../evidence/interviews/2026-06-10-pilot-team-meeting.md) (recorded first, per discipline), the morning's [pilot workspace audit](../evidence/observations/2026-06-10-pilot-workspace-audit.md), and the [professor interview](../evidence/interviews/2026-06-10-professor-classical-research-steps.md).

## The posture revision (and G5's retirement)

The pilot researcher will work through chat and will not author documents; he framed the relationship he wants as *a junior colleague you never fully trust but happily let do the heavy lifting*. The maintainer's judgment, recorded here: requiring busy-work the researcher doesn't believe in is self-defeating — researchers will reject the methodology or quietly reshape it (both observed in the pilot within two days). The school-homework analogy guided the reframe: the answer to AI is not banning it from the work but moving the *assessment* — you stop grading the essay and start grading the oral defense.

The methodology's operationalization therefore moved from **authorship rules to gates**: AI does the heavy lifting; the researcher's contribution flows through conversation; progress and the second output are carried by interview-conversations at closures and commitments. Decision ownership and independent verification are explicitly *not* relaxed. The full statement is [`METHODOLOGY.md`](../METHODOLOGY.md) §2–3.

**G5 (refuse whole-task outsourcing) is the registry's first retirement.** Post-mortem: G5 translated "preserve capacity" into "do the work yourself," which read as make-work to the first real user and was rejected wholesale — taking the posture down with it, while the verification gate (the thing actually carrying the second output) survived on its own merits. The diagnosis it served (A17, A16) stands; the response was wrong. Replaced by G20 (gate-carried apprenticeship). The bet this rests on is opened as **Q13**: if gate records pass while external signals of researcher development stagnate, the gates — not the principle — get revised next.

## Design decisions (maintainer's, from the conversation)

- **Gates** are interviews that produce value for the work, not tests — with a goal-gradient (early-stage gates legitimately lean test-like because articulation is the goal there). The agent closes by default when the conversation stops producing value, may vote to prolong; the researcher overrides on record, never argued. (G20, G16 reframed.)
- **Modes** — work / conversation — join skills in the user-facing vocabulary, introduced at onboarding, invocable by name. (G21.)
- **Two-repo split.** This repo is the inquiry; the **starter** (a GitHub template repo) is the researcher-facing product: README + CLAUDE.md + state cursor + context store + FRICTION/ + eight skills (onboard, gate, learn, paper, gather, ideate, session, update). User-surface = what the researcher sees (README, chat, skill *names*); everything else is visibly machinery. Day-one self-sufficiency: everything the researcher needs is in the README or said proactively by the agent.
- **Onboarding** is an interview (replacing the written intake the pilot deleted): identity, goals, where the work stands, the interaction contract with our defaults proposed and adjustments recorded, skills selected from the shipped library. (G22.)
- **Workspace shape:** `state.md` cursor + `context/` store (profile / knowledge / records); researcher-written ledgers retired — their function moved to gate-generated records plus a periodic review conversation (G6/G7/G11 reframed). Provenance carried inline (G15 reframed to the pilot's actual practice).
- **Sync channels:** downstream, [`updates/`](../updates/) in this repo — agent-addressed update documents, per-item adoption conversations, deliberate re-pin ([0001](../updates/0001-gates-posture-and-starter.md) covers this whole revision for workspaces pinned at fc00c47); upstream, the workspace's `FRICTION/` folder, agent-drafted + researcher notes, read by maintainers by arrangement (pull, not push) during the early-user phase.
- **One document.** The `methodology/` folder retired into a root [`METHODOLOGY.md`](../METHODOLOGY.md): principles, posture, process, gates, modes, the practice registry (G-numbers preserved; statuses live), and the starter mapping. `guidelines.md`, `ai-native-research-process.md`, `agent-operating-guide.md`, and `HANDOFF.md` retired (texts in git history, committed beforehand). The starter is the executable view; nothing normative lives only there.
- **Open questions made live:** the agent proactively offers to open/close questions during any work here; `add-evidence` gained a `related_questions` field, `inquiry-status` now reports evidence-per-question, `update-foundation` carries the open/close mechanics.

## Registry changes

**Retired:** G5 (post-mortem above). **Reframed:** G2 (cursor/store), G6/G7/G11 (records + review conversation), G10 (fetch-before-rely absorbed), G15 (inline provenance), G16 (interview vocabulary). **New, all `proposed`:** G20 (interview gates), G21 (named modes), G22 (onboarding contract). **Kept:** G1, G3, G4, G8, G9, G12, G13, G14, G17 ("authors" now explicitly = owns through conversation), G18, G19. Evidence for the new entries: the three 2026-06-10 evidence files.

## Flagged, not done

- **GOAL.md revisions** (posture wording, the "private while the pilot runs" line vs. the public pilot, stale counts) — proposed as text to the maintainer, applied only on approval.
- **The starter's GitHub template repo** — built locally at `ai-native-research-starter/`; creating the GitHub repo, ticking "Template repository," and setting the real `pinned_commit` are the maintainer's actions.
- **Professor consent** before publication (unchanged from the morning's flag).
- The pilot's own posture reconciliation now has its path: update 0001 walked by the pilot's agent.
