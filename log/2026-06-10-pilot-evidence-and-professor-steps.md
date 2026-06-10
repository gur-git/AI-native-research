# 2026-06-10 — First pilot-phase evidence: the professor's classical steps, and the first background audit of the pilot workspace

The pilot phase produced its first two pieces of evidence today, and they produced the methodology's first post-foundation guidelines (G16–G19). Two standing channels opened: occasional conversations with the pilot team's supervising professor about how research is classically conducted (raw material to adapt AI-natively, not copy), and periodic maintainer-side background audits of the pilot's public workspace. A conversation with the pilot team is scheduled for later today; its notes will be recorded separately.

- Added evidence: [A professor's account of the early steps of the classical research process](../evidence/interviews/2026-06-10-professor-classical-research-steps.md) — knowledge first (measured by weekly explain-back), then a five-part research proposition, then an MVP, then parallel expert discussion. Relayed secondhand; confidence weak.
- Added evidence: [First background audit of the pilot workspace](../evidence/observations/2026-06-10-pilot-workspace-audit.md) — the pilot re-cut the scaffold within two days (AI-as-full-team working mode, HANDOFF/INTAKE retired, reconciliation deferred), kept and exercised a teach→quiz gate that no guideline owned (one real gap caught), left the reflective ledgers empty, and had not yet begun the paper source-walks as of the snapshot.
- Opened the pilot case-study record: [case-studies/snn-research/](../case-studies/snn-research/README.md) — indexes the channels and the open items; the substance stays in `evidence/`.

## Guidelines added

All four adapt classical practice to the AI-native regime; none is a copy. All start `proposed`.

**Number:** G16
**Name:** Gate knowledge-building with an explain-back check
**Status:** proposed
**Addresses:** A13, A16 (A5, A7, A8 shape the caveats)
**Evidence:** the professor interview and the pilot audit — two convergent (not fully independent: the professor supervises the pilot team; both recorded via the maintainer) sources pointing at the same practice (the professor's weekly explain-a-concept instrument; the pilot's teach→quiz gate, which caught a real gap and survived the pilot's posture relaxation)
**One-line motivation:** the inquiry's first measured (not felt) instrument for the second output; candidate answer to Q11.

**Number:** G17
**Name:** Converge the survey into a researcher-authored five-part research proposition
**Status:** proposed
**Addresses:** A4, A7 (A8 governs the existing-approaches part)
**Evidence:** the professor interview
**One-line motivation:** gives the survey→design transition a concrete, researcher-authored exit artifact the process sketch lacked.

**Number:** G18
**Name:** Build a minimum viable version early; iterate against reality
**Status:** proposed
**Addresses:** A1, A3 (bounded by A9, A17)
**Evidence:** the professor interview (the step); the AI-regime rationale is the maintainer's extension, marked as such
**One-line motivation:** AI collapses build cost for recombination parts, shifting the design bet toward early contact with reality — under G4/G5/G9 discipline.

**Number:** G19
**Name:** Put the work in front of expert humans early, and in parallel
**Status:** proposed
**Addresses:** A6, A8 (and A7)
**Evidence:** the professor interview; the pilot audit corroborates the existence of the mentor channel (research-question commitment reserved to a decision with the supervising mentor), while the early-and-parallel shape rests on the interview alone
**One-line motivation:** the expert human is the categorically independent critic, strongest exactly at the frontier where AI is weakest; first concrete mechanism for the process sketch's collaboration gap.

## Views updated

`methodology/agent-operating-guide.md` (phases 2, 3, cross-cutting) and `methodology/ai-native-research-process.md` (phase 2, phase 3, collaboration note, track-both-outputs discipline, double-booking table) updated to carry G16–G19, with the new material tagged to the new evidence. Guideline counts refreshed in `README.md` and `CLAUDE.md` §Status.

## Verification round

An adversarial coherence check (three independent review passes over the day's diff, run before this entry was finalized) caught and led to fixing: a broken evidence citation (G19 cited the audit for a mentor-gated-commitment observation the audit had not recorded — the observation is verifiable pilot-repo state and was recorded properly, and G19's claim was narrowed to what it supports); a misattributed finding (the nine-discipline compression in the pilot's CLAUDE.md is HANDOFF v0's own design, not a pilot re-cut — corrected in the audit and its echoes); an overclaimed "two independent sources" framing for G16 (softened: the professor supervises the pilot team and both sources arrive via the maintainer); the interview's confidence label (moderate → weak, matching its own caveats); and several wording-level overreaches ("validated" at n=1, "stalled" at two days). One deliberate restatement risk is accepted for now: the explain-back and proposition mechanics appear in guidelines.md (source) and, compressed, in the two process views — the views should be thinned toward pointers if they drift.

## Flagged, not acted on

- **The pilot's posture reversal.** Two days after adopting the methodology, the pilot team chose an AI-as-full-team working mode that its own state file says contradicts the advise-don't-author posture; reconciliation is deferred on their side. This is the strongest contact-with-reality signal the inquiry has against (or about the framing of) its central operating posture — and it is one team, early, with their own verdict pending. Recorded in the observation file; to be taken up with the team in today's conversation before any foundation or G1-framing move. Bears on Q9/Q10.
- **Zero ledger adoption and the stalled source-walk handoff** — recorded as evidence; G6/G7/G10/G11 design implications await more signal (and the team's own account).
- **HANDOFF v1 candidates** from the pilot's re-cut (transient intake, pin-in-CLAUDE instead of a persistent handoff file, drafted-observation/human-verdict convention, agent-side refusal lines, mid-project entry path) — listed in the observation file's implications; deliberately not applied to `HANDOFF.md` yet. The interface is under study, and the team's conversation notes should land first.
- **Two GOAL.md reconciliations await a deliberate revision by the maintainer:** the charter describes the pilot's repo as "private while the pilot runs" while the team's workspace is public, and its Status still counts 15 guidelines. Both noted (here and in the case-study record) rather than edited — GOAL revisions are deliberate and rare by its own rule.
