# AI-native research

AI changed what it costs to produce research output — and quietly changed what it costs to *become* a researcher. This repo is an open inquiry into how research should be done when you work with AI, built so you can actually use it: bring a research project, and run it with your AI agent in a way that leaves you more capable, not less.

It is a record of an inquiry, not a finished framework. The diagnosis — what about AI forces research workflows to change — is settled enough to act on. The methodology is grown from evidence over time, and every part of it is marked with how much we actually know.

## The idea, in one minute

Every earlier tool of knowledge work took a skill and handed back a new one. The calculator would not compute until you knew what to ask; you grew because the tool insisted on it. AI is the first tool that does not insist: a sentence in, a draft out. You can produce passable work indefinitely without building any compensating capacity — though that work is quietly below what the same prompt produces in skilled hands.

So the usual reassurance — *the worker is still skilled, just at different things* — fails for AI, and it fails hardest for a researcher, whose real second output is **themselves**: a person who can do harder work next time than last. The methodology here answers with one principle: **empower, not replace.** Use AI in ways that grow your capacity to do the research job at the level it is actually judged on — not in ways that quietly substitute for it. (Routine work below that level — syntax, formatting, unit conversions — is fine to hand off; the principle is judged at the level of the whole job.)

The full argument is in [`GOAL.md`](GOAL.md), the charter, and [`foundation/00-why-reimagine.md`](foundation/00-why-reimagine.md).

## The shape of the work

Working this way is not a fixed pipeline, but it has a recognizable arc:

- **Get oriented** — you and your agent start from a shared understanding of the methodology: what it is, and why.
- **Set context** — your question, what would convince you and a skeptic that an answer is right, and which capacities you mean to keep yours. Mid-project, you start by saying where you already are.
- **Understand broadly, then narrow** — use AI to map the landscape so *you* build the broad picture, then find the specific points worth pursuing. The map is for your learning, not a substitute for it.
- **Design with verification first** — decide what would convincingly verify an answer before building toward it.
- **Do the work, hands on where it counts** — hand off the routine; stay in the parts where the substantive judgment lives.
- **Verify independently, keep state, track your growth** — check results against a source independent of what produced them, hold project state in files, and watch your own capacity, not only the output.

This arc is a hypothesis under test, like everything else here. The detailed, still-evolving version is in [`methodology/ai-native-research-process.md`](methodology/ai-native-research-process.md).

## Why you can trust it

This is written for a working researcher, so it tries to earn trust the way you would want it earned:

- **Evidence-driven, and honest about the gaps.** Every claim traces to a source or is marked as the maintainer's own observation. The methodology's 19 guidelines are all still `proposed` — hypotheses under test, not validated results — and they say so.
- **No selling.** You will not find "revolutionary" or "10x" here. Where something is speculative it is tagged speculative; where the evidence is thin it says so.
- **It revises in the open.** Guidelines can move to `testing`, `adopted`, or `retired`, and the reasoning stays visible in [`log/`](log/). A methodology that never changes has stopped being honest about a technology that is still moving.

If that reads like a lot of caveats — that is the point. The caveats are why the parts that are *not* caveated are worth your time.

## How to start

You bring a topic, or a project already underway; the repo gets you and your agent working inside the methodology. The technical part is light — mostly plugging in your agent:

1. **Make a fresh repo** for your project (private is fine).
2. **Drop in [`HANDOFF.md`](HANDOFF.md)** and hand the repo to your AI agent: *"Follow `HANDOFF.md`."* It sets up a light workspace — a project-state file, two thin ledgers, a short intake — and picks up its operating manual ([`methodology/agent-operating-guide.md`](methodology/agent-operating-guide.md)), which is what lets it *advise* you through the work. It will not do your research.
3. **Fill the intake** — your question, what would convince you (and a skeptic) that an answer is right, and which capacities to protect versus hand off — then work. If you are mid-project, you start by telling your agent where you already are. Your research lives in your repo and stays yours.

[`HANDOFF.md`](HANDOFF.md) is an explicit **v0**: the lightest version that carries the methodology, and itself something we are still learning to get right. If a piece does not earn its place, drop it — noticing what chafes is exactly the feedback this is being built from.

---

*Everything below is reference — for understanding the inquiry, or digging into any part. The clean read is above; follow the links when you want more.*

## What's here

- **[`GOAL.md`](GOAL.md)** — the charter. The why, the how, and the commitments everything else aligns to. Read first.
- **[foundation/](foundation/)** — the diagnosis: the central argument (with the recombination-vs-innovation distinction in §3), the catalog of 17 AI attributes (5 clusters, each tagged structural / temporary / ambiguous), the implications, and the open questions.
- **[methodology/](methodology/)** — the prescription: [`guidelines.md`](methodology/guidelines.md) (19 guidelines, all `proposed`, each tied to an attribute, an evidence trail, and a skill implication), a speculative [`ai-native-research-process.md`](methodology/ai-native-research-process.md) (a `v0` sketch of the end-to-end process), and [`agent-operating-guide.md`](methodology/agent-operating-guide.md) — the agent's operating manual, the back-end counterpart to this README.
- **[`HANDOFF.md`](HANDOFF.md)** — the tool: the file you give your agent to scaffold a workspace.
- **[evidence/](evidence/)** — the substrate: interviews, experiments, observations, a self-study stream, a lab survey, and an annotated reading list.
- **[log/](log/)** — the chronicle: what changed, when, and why.
- **[case-studies/](case-studies/)** — the pilot's documented record (the research itself lives in the researcher's own repo).

## A reading path

- **Five minutes:** [`GOAL.md`](GOAL.md).
- **Fifteen:** add [`foundation/00-why-reimagine.md`](foundation/00-why-reimagine.md) — the full argument in compact form.
- **An hour:** add [`foundation/01-ai-attributes.md`](foundation/01-ai-attributes.md), then [`methodology/guidelines.md`](methodology/guidelines.md) and the [process sketch](methodology/ai-native-research-process.md).
- **The whole picture:** `foundation/` in order (`00` → `03`), the [innovation literature note](evidence/literature-notes/innovation-as-different-operation.md), the methodology, then the [reading list](evidence/reading-list.md).

## What this is not

- Not a framework asserted upfront — it is grown from evidence, and guidelines can be retired.
- Not a way to do research faster while letting AI do more of it. Faster-but-hollowing is the failure mode it exists to push against.
- Not a recipe for autonomous research. The reimagining is about *your* workflow.
- Not a competitor to system-level efforts (FutureHouse, DeepMind co-scientist, PSI / GPD, Sakana). It works at a different layer — an individual or small group using best-in-class tools well.
- Not finished. Expect revision.

## Status

Foundation v1 as of 2026-05-06: five foundation documents. The methodology has 19 guidelines (all `proposed`; G16–G19 added 2026-06-10 from the first pilot-phase evidence), plus a speculative `v0` synthesis of the end-to-end process ([`methodology/ai-native-research-process.md`](methodology/ai-native-research-process.md)). Evidence collection has begun beyond the reading list — a self-study stream, a lab survey, and the pilot phase's first entries (an interview on the classical research steps and a pilot-workspace audit, 2026-06-10, which produced guidelines G16–G19). The first researcher-facing tool, [`HANDOFF.md`](HANDOFF.md), has shipped, and the pilot (the maintainer's own research project) is running against it.

## How the inquiry maintains itself

Four skills under [`.claude/skills/`](.claude/skills/) keep the methodology honest as it grows: `add-evidence` (record an interview, experiment, observation, or reading), `update-foundation` (revise a foundation claim with traceability), `add-guideline` (promote a practice to `proposed`), and `inquiry-status` (where things stand). The discipline is foundation-first, evidence-driven, observational in tone, and *empower over replace*. Full operating principles are in [CLAUDE.md](CLAUDE.md).

## Following along, contributing

The repo is **not currently accepting external contributions**. See [CONTRIBUTING.md](CONTRIBUTING.md) for the read-only / collaboration policy. If you are working on related problems and want to discuss a collaboration, email **masuryg@post.bgu.ac.il**.

If you want to follow along, watch or star the repo; updates are recorded in [log/](log/).

## License

MIT. See [LICENSE](LICENSE).

## Citing

If the framing or a specific document is useful in your work, citation is welcome. See [CITATION.cff](CITATION.cff).
