# updates/

The downstream channel: how changes to the methodology reach researchers already working in scaffolded workspaces.

**Audience: the researcher's agent, not the researcher.** Each document here describes a batch of methodology changes in a form an agent can mediate — what changed, why (with the evidence), and what to ask its researcher. The researcher never reads a diff; their agent reads the document and runs a conversation: adopt, skip, or adapt, item by item. The `update` skill in the starter knows to look in this directory.

## Conventions

- Documents are numbered and dated: `NNNN-short-slug.md`, ascending. An agent whose workspace pin predates a document's `applies_from` should walk that document with its researcher.
- Each item in a document carries: **what changed**, **why** (one line, linking evidence), **what to ask your researcher**, and **how to apply** (the concrete edit, if adopted).
- Adoption is per-item and always the researcher's call. Skipped items are recorded in the workspace (`context/records/`) so future updates know the history. After walking an update, the agent moves the workspace pin forward — deliberately, never silently.
- Updates here describe **methodology changes only** — posture, gates, skills, defaults. They never instruct an agent to touch the researcher's own content (state, knowledge, records).
