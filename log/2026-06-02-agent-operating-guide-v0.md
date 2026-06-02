# The agent's operating guide, and a reconciled phase scheme (2026-06-02)

The conversation reconciled two phase schemes — the `v0` process sketch's `0a`–`9` and the
maintainer's `-1 / 0 / 1` on-ramp — into one, and added a governing stance for how the agent should
relate to the researcher and to the methodology itself.

## The governing stance (the key move)

The agent **advises; it does not march, and does not do the research.** It holds the methodology the
way a good collaborator holds a plan: it makes the step, its purpose, and the relevant guideline
visible, lays out the choice and the alternatives (including ones outside the methodology), and
leaves the decision to the researcher — who may also change the methodology to fit their work. This
is empower-not-replace applied recursively: even the proposed path is offered, not imposed. Marching
a researcher through stages on autopilot is the failure mode, because it replaces the judgment the
methodology exists to build.

## The reconciled phases

A proposed path, not a track; recurring and entry-flexible (meet the researcher where they are):
**0 Orient · 1 Context · 2 Survey-then-focus · 3 Design · 4 Execute · 5 Verify · 6 Disseminate ·
7 Respond to review**, with the genuinely cross-cutting disciplines (state, both-output ledgers,
portfolio/exploration, provenance, the empower/replace pause) pulled out of the sequence. The
on-ramp (Orient, Context) is the part the `v0` sketch had assumed; "Survey, then focus" carries the
broad→specific framing.

## What was added

- **`methodology/agent-operating-guide.md`** (v0) — the back-end counterpart to the README: the
  operating manual that tells an AI agent how to advise a researcher through the phases, with the
  advisory stance as its prime directive, the four front-end moves per phase (where we are / why it
  matters / the guideline / the choice), the cross-cutting disciplines, and a hard DO-NOT block. It
  is a *view* on the foundation/guidelines, referencing them by number rather than restating.

## Still to do (flagged, small)

- **Wire `HANDOFF.md`** so the scaffolded research-repo `CLAUDE.md` points the agent to this guide at
  the pinned commit (so the guidance loads on setup).
- **Loosen `HANDOFF.md`'s** agent-alteration rule: the agent may propose adapting the scaffold and
  apply it with the researcher's okay, not only note it in friction.
- **Reconcile** [`ai-native-research-process.md`](../methodology/ai-native-research-process.md) to the
  new phase scheme (its `0a`–`9` detail) so the descriptive and operating views share one structure
  — coherence debt, named here.

## Status

The maintainer approved the scheme as a starting point and will give feedback after interacting with
the agent — that empirical try is the real test. The advisory stance is a genuine addition to the
methodology (empower-not-replace applied to the process itself) and is worth capturing in the
foundation deliberately, via `update-foundation`, not only in this guide.
