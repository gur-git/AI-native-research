---
name: update-foundation
description: Revise a foundation document (why-reimagine, ai-attributes, what-this-implies, open-questions) based on new evidence, with a clear traceability trail. Use when accumulated evidence refines, contradicts, or extends a current foundation claim.
---

# update-foundation

Update a foundation document in response to evidence. The point of this skill is not just to edit a file — it is to *make the change auditable*. A foundation document that cannot be traced to its evidence is a hot take with extra steps.

## When to invoke

- A new piece of evidence in `evidence/` makes a current foundation claim look wrong, incomplete, or sharper than it should be.
- Multiple pieces of evidence have accumulated on a point and the foundation should now reflect the consolidated view.
- A foundation attribute's tag (`structural`, `temporary`, `ambiguous`) needs revision because the underlying technology or understanding has moved.
- A new attribute has emerged that wasn't on the radar when the foundation was first written.

Do not invoke for typos, formatting, or rewording without substantive change. Use a normal edit for those.

## Inputs to gather

1. **Which foundation file** — `00-why-reimagine.md`, `01-ai-attributes.md`, `02-what-this-implies.md`, or `03-open-questions.md`.
2. **What is changing** — the specific claim, attribute, or section being revised. Quote the current text.
3. **Why** — which piece(s) of evidence are driving the change. List by path. If the change is driven by external news or a new source, link it and add it to the reading list as a separate step.
4. **Proposed new text** — draft the replacement before committing the edit.
5. **Tag change (if applicable)** — for `01-ai-attributes.md`, if a tag is moving (e.g., `temporary` → `ambiguous`), note it explicitly and explain.

## Procedure

1. **Read the current foundation file** in full. Do not edit blind.
2. **Confirm the evidence** by reading the cited evidence files. If the evidence does not actually support the proposed change, stop and surface this.
3. **Write the diff in plain English first**, in the conversation, before touching the file. Format:
   ```
   File: foundation/01-ai-attributes.md
   Section: Attribute N — <name>
   Current: <current claim or tag>
   Proposed: <new claim or tag>
   Driven by: evidence/{type}/{file}.md, evidence/{type}/{file}.md
   ```
4. **Apply the edit** only after the diff is explicit.
5. **Add a traceability footnote** in the foundation file at the bottom of the affected section:
   ```
   *Last revised YYYY-MM-DD based on [filename](../evidence/.../filename.md).*
   ```
6. **Append a log entry** in `log/YYYY-MM-DD-{topic}.md`:
   ```markdown
   ## Foundation update

   **File:** `foundation/01-ai-attributes.md`
   **Section:** Attribute N — <name>
   **Change:** <one-sentence summary>
   **Driven by:** [evidence file(s)]
   **Reason:** <one-paragraph explanation of why the evidence motivates this change>
   ```

## Reminders

- The foundation is allowed to change. Pretending it is settled when evidence shifts is the bigger risk.
- If a change is contested (different pieces of evidence point different directions), prefer to add to `03-open-questions.md` rather than picking a side prematurely.
- If a change moves a tag from `structural` to `temporary` (or vice versa), the bar is higher. Tag changes mean the methodology design budget shifts. Demand strong evidence and write a fuller explanation.
- Never delete superseded text without preserving it in the log entry. The history of how a claim was understood is itself useful.
