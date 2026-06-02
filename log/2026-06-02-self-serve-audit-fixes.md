# Closing the self-serve gaps so the repo needs no runbook (2026-06-02)

The maintainer pushed back on a hand-written runbook: a researcher should need *only the repo*. The
runbook's existence was the signal that the repo was not yet self-serve. Rather than assert
self-serve, a stranger-walk audit (three perspectives — a fresh researcher, a mid-project
researcher, and the researcher's AI agent executing `HANDOFF.md` — plus a synthesis) found the gaps.

## The blocking gap

The documented path (README → `HANDOFF.md` → scaffolded `CLAUDE.md`) never connected the agent to
`methodology/agent-operating-guide.md` — the manual that makes it *advise* through the phases. The
agent would scaffold and stop, running the nine disciplines but never adopting the advisory phase
behavior. A researcher would have had to be told, out of band, to point their agent at the guide.
Compounding it: the guide lives in the (absent) source repo, reachable only via a source pin that
`HANDOFF` told the agent to leave as `TODO` with nothing prompting the researcher to fill it.

## Fixes applied

- **`HANDOFF.md`** — names the source repo URL; has the researcher record the URL + commit so the pin
  resolves; instructs the scaffolding agent to fetch and operate by the operating guide, and to flag
  an unresolved pin as a blocker; adds a mid-project intake field (`## 0. Where you already are`);
  clarifies the agent *may* transcribe the researcher's own dictated progress into `state.md`
  (the prohibition is only on inventing substance); and loosens the agent-alteration rule to match
  the operating guide (propose + apply with the researcher's okay).
- **`README.md`** and **`methodology/README.md`** — surface `agent-operating-guide.md` so it is
  discoverable while browsing and named in the "how to start" path.
- **`methodology/ai-native-research-process.md`** — a top note pointing to the reconciled `0–7`
  phase scheme in the operating guide as current, marking this document's `0a–9` as the older
  descriptive view under reconciliation (coherence).

## Residual (the one thing that can't be a literal value in-repo)

`HANDOFF.md` cannot hard-code the exact commit SHA a researcher took it from. The in-repo fix is the
*instruction* to record the URL + commit — which lives fully in the file. No external runbook
remains.
