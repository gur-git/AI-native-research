# Lab AI-use survey enters the evidence base (2026-06-01)

The maintainer ran a survey of lab members on how they use AI tools in their work
(Google Form, "שימוש בכלי AI במעבדה" / *Use of AI tools in the lab*). It is the first
piece of evidence in the repo that is **multi-respondent and ongoing** — the form is
still accepting responses — rather than a fixed snapshot. That changes how it has to be
recorded.

## What was done today

- Added a new evidence category, `evidence/lab-surveys/`, for surveys administered to a
  group (distinct from `interviews/`, which are 1:1). First entry:
  [`../evidence/lab-surveys/ai-tool-use-2026/README.md`](../evidence/lab-surveys/ai-tool-use-2026/README.md).
- Built that entry as a **living document** rather than a static evidence file: the
  instrument (§1), the responses (§2), and a provisional descriptive synthesis (§3) are
  separated so the data sections can be regenerated in place as the response count grows.
  Frontmatter carries `n_responses` and `as_of` so the document's freshness is legible at
  a glance, and a change log (§5) records every refresh and instrument change.
- Documented a refresh procedure (§4): link the form to a Google Sheet once, after which
  every update is a single Sheet read through the Drive integration.

## What blocked the data pull

The form's questions and responses could not be read with the available tools:

- The local `.gform` file is a cloud-only Google Drive placeholder; it would not hydrate
  for any reader (Read, PowerShell, copy), returning `ERROR_INVALID_FUNCTION` even with the
  sandbox disabled.
- The Drive integration cannot enumerate or read Google Forms, and no responses Sheet was
  linked to the form, so there was nothing Sheet-shaped to read either.

So the scaffold was built and committed to structure, but the instrument and responses are
marked **pending**. Populating them needs either a form→Sheet link (preferred — makes
future refreshes automatic) or a manual CSV export from the maintainer.

## Still open

- Confirm the lab/PI name and the actual date the form opened (the doc uses the form's
  last-modified date, 2026-05-23, as a proxy).
- Pull in the instrument and responses, then set `confidence` and map the synthesis to
  specific attributes in `foundation/01-ai-attributes.md` (A15, A16, A13, A17 are the
  likely candidates, to be confirmed against the data, not assumed).
- Once N is meaningful, decide via `update-foundation` whether anything observed refines a
  foundation claim — drawn separately, not in the evidence file.
