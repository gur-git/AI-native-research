# Step 0 landscape — deeper Karpathy and Anthropic Claude usage guides (2026-05-17)

Same-day follow-on to the round-2 expansion. Maintainer asked for additions on Andrej Karpathy (already lightly cited) and on Anthropic's published "web guides for AI" (not previously engaged with). Both produced more substantive findings than expected.

Source doc updated in place: [`../evidence/survey-2026-05/step-0-landscape.md`](../evidence/survey-2026-05/step-0-landscape.md).

## What was done

One focused subagent covered both extensions in parallel passes. Six Karpathy artifacts surfaced (Software 2.0 / Medium 2017; Software 3.0 / YC keynote June 2025; LLM OS thread / X Sept 2023; vibe coding origin / X Feb 2025 plus Feb 2026 walkback; context engineering endorsement / X 2025; Eureka Labs launch July 2024; Sequoia AI Ascent 2026). Five Anthropic methodology documents characterized (Building Effective Agents Dec 2024; prompt engineering reference; Claude Skills docs + Oct 2025 engineering blog; Claude Code best practices; Anthropic Cookbook).

## What changed in the inquiry's understanding

**Karpathy is closer to the repo's stance than round 2 captured.** The Sequoia AI Ascent 2026 piece contains the most precise empower-not-replace formulation in the entire survey: *"You can outsource your thinking, but you can't outsource your understanding."* Plus an explicit list of irreducible developer skills (system design judgment, spec creation, code review, fundamental concepts, security threat assessment) that is methodology-shaped. Eureka Labs (his AI-native education startup, July 2024) is the most explicit institutional embodiment of empower-not-replace among Vector 2 voices. The gap between Karpathy and the repo: he frames it **negatively** (what cannot be outsourced) where the repo frames it **positively** (what AI use should grow).

**The Anthropic Claude usage guides are arguably the most operationally specific methodology corpus in the field.** More concrete than the positioning of any AI-lab leader (Altman, Hassabis, Suleyman) and more specific than most academic AI-for-science position papers. The Claude Code best practices document in particular is the closest any AI-lab document comes to engaging skill formation as a positive design criterion — its "develop your intuition" section treats expert judgment as a learnable craft. A new cross-cutting observation added to §4 of the step-0 doc: **operational methodology often comes wrapped as product documentation.** The mechanism is structural — product companies have incentive to publish detailed usage guidance; leaders and academics have incentive to position at higher levels of abstraction. The most actionable answers to "how should a researcher actually work with AI?" are currently in product docs, not manifestos.

**Vector taxonomy still holds.** Karpathy remains in Vector 2 (architectural prescription) but with explicit note that he crosses into Vector 3 (craft) via the agentic-engineering body of work. The Anthropic guides are also Vector 2 but sit at a different register from the philosophical-advocate entries — a "Vector 2b: operational methodology / product documentation" sub-position is sketched in the cross-cutting note rather than as a sixth vector. No new vectors created.

## Findings most worth carrying into the foundation

In rough order of weight:

1. **Karpathy's "you can outsource your thinking but you can't outsource your understanding"** is so close to the repo's framing that the foundation should engage with it directly — either as an adjacent quotation that anchors empower-not-replace in mainstream AI-lab discourse, or as a sibling-but-distinct framing the repo's positive design criterion is meant to extend beyond. Either way, the foundation should not pretend it isn't there.
2. **The product-docs-as-methodology observation** is itself a methodological finding about where to look. If true, the survey's stage 3 (per-territory literature pass) should treat AI-lab usage documentation as a primary literature, not just promotional material. This is a real shift from how academic literature surveys usually source.
3. **The Claude Code best practices "develop your intuition" framing** is the closest analogue in product documentation to what the repo's methodology articulates positively. Worth a literature-note-grade read alongside Elicit and Scite.ai (already on the stage-3 list).
4. **Eureka Labs is a working institutional instance of empower-not-replace** — worth tracking as a case study even though it's pre-pilot for this repo's own case-studies/ directory.

## Still open

- Parallel question: what do **OpenAI's, Google's, Mistral's, and xAI's** equivalent usage documentation prescribe? If they reach similar prescriptions, the product-docs-as-methodology finding is robust; if they diverge, the divergence is itself interesting. This belongs in stage 3.
- The "vibe coding" walkback (Feb 2026) is a clean illustration of how methodology terms drift as they cross audiences. The repo's eventual vocabulary decisions (whether to adopt centaur/cyborg, agentic engineering, vibe coding, supervise-the-process, etc.) should account for this drift risk.

## Format addendum (same day)

Following the content additions above, an **At a glance — five visions, five bets** preamble was prepended to the step-0 doc. Each of the five vectors gets a one-line "unique" + one-line "bet" framing; a sixth entry positions where this inquiry sits (for transparency about the document's point of origin). The motivation is pitch-readiness: a new reader gets the field map and the implicit wagers before encountering the detailed treatment. No content was changed in the numbered sections; the preamble sits between the "About this document" callout and `## 1. Purpose`. Section numbering is unchanged so existing references (this log entry's references to `§4` and `§6` of the step-0 doc remain valid).
