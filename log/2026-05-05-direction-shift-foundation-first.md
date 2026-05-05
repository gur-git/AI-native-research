# Direction shift: foundation-first (2026-05-05)

The repo's v0 plan changed today. Recording the shift, the reasoning, and what it means for the structure.

## What changed

The original plan (see [2026-05-05-initial-design-thinking.md](2026-05-05-initial-design-thinking.md)) was: build two runnable tools (literature triage + research log) plus a methodology document, and ship them as the repo's first version. The methodology document was structured around two AI attributes: forgetting and the perception gap.

The maintainer pushed back on three points:

1. The diagnosis was thin. Two attributes do not carry a reimagining of research. The honest list is more like fifteen attributes across four clusters, and not all of them are structural — some will be solved by capability improvements and the methodology should not over-commit to addressing them.
2. The proposed methodology was not impressive enough or tightly enough coupled to the diagnosis. It was a workflow, not a reimagining.
3. Reimagining research is a long-haul project. It cannot be one-shot. The repo should start by building a strong foundation — the story, the reasoning, the why — and then the methodology grows from that foundation, step by step, evidence-driven.

## What this means for the repo

- **v0 is the foundation, not the methodology.** The two foundation documents (`foundation/00-why-reimagine.md`, `foundation/01-ai-attributes.md`) are the substantive artifacts. The methodology is mostly empty by design and grows from evidence.
- **The repo's identity is "an inquiry in the open," not "a framework."** The foundation documents are written. The methodology will be written over months, in `methodology/guidelines.md`, with each guideline traced to evidence and an attribute.
- **The first tools built are repo-maintenance tools, not researcher tools.** Skills in `.claude/skills/` (`add-evidence`, `update-foundation`, `add-guideline`, `inquiry-status`) keep the inquiry coherent as it grows. Researcher-facing tools come later, when evidence has earned them.
- **The AI-attributes file uses structural / temporary / ambiguous tagging.** Each attribute gets a short complete description and a thorough explanation of why the tag is right. The point is to direct methodological investment toward the attributes that will not be solved by capability improvements.

## Files written today

- `CLAUDE.md` — operating principles
- `.claude/skills/{add-evidence,update-foundation,add-guideline,inquiry-status}/SKILL.md`
- `foundation/README.md`, `foundation/00-why-reimagine.md`, `foundation/01-ai-attributes.md`, `foundation/02-what-this-implies.md`, `foundation/03-open-questions.md`
- `evidence/README.md`, `evidence/reading-list.md`
- `methodology/README.md`, `methodology/guidelines.md` (schema, no guidelines yet)
- `log/README.md`, this entry, the preserved initial-thinking entry

Public-facing files (`README.md`, `LICENSE`, `CONTRIBUTING.md`, `CITATION.cff`) are next.

## What is open after today

The five questions in `foundation/03-open-questions.md` are the immediate ones. The most pressing is Q1 — whether the structural / temporary / ambiguous tagging holds up across model generations. That is answered by time and observation, not by reading. The first concrete next step is choosing the pilot research domain and beginning to gather observation evidence from real working sessions.
