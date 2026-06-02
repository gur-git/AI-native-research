---
type: survey
source: lab members (self-administered Google Form, anonymous unless noted)
lab: "<lab / PI name — to confirm>"
instrument_file: "G:\\My Drive\\שימוש בכלי AI במעבדה.gform"
instrument_title: "שימוש בכלי AI במעבדה (Use of AI tools in the lab)"
date_opened: 2026-05-23        # form last-modified date as a proxy; replace with actual open date
status: ongoing                # living document — the form is still accepting responses
n_responses: pending           # update on every refresh
as_of: pending                 # date the figures below were last regenerated
confidence: pending            # small-N self-report; set honestly once N is meaningful (weak → moderate)
related_attributes: []         # map to foundation/01-ai-attributes.md once responses are in
raw_material: pending          # link the Form to a Google Sheet, then record the Sheet URL/ID here
---

# Lab survey — AI tool use (2026)

> **About this document.** This is a *living* evidence record of a survey of lab members on how they
> use AI tools in their work. Unlike a one-shot interview or experiment, the form is expected to keep
> receiving responses, so this document is built to be **re-generated in place** as the response count
> grows. Two numbers in the frontmatter make the document's freshness legible at a glance:
> `n_responses` (how many responses the figures below reflect) and `as_of` (when they were last
> regenerated). Anything below the "Synthesis" heading is **descriptive evidence, not a conclusion** —
> conclusions about the foundation or methodology are drawn separately, via the `update-foundation`
> and `add-guideline` skills, and must cite this document with its `as_of` snapshot.
>
> **Status: awaiting data.** The questions and responses have not yet been pulled in. The form lives on
> the maintainer's Google Drive as a cloud-only file that the toolchain cannot read directly, and Google
> Forms responses are not reachable through the Drive integration. See **§4 How to refresh** for the
> one-time setup (link the form to a Google Sheet) that makes every future update a single read.

---

## 1. The instrument

The questions, exactly as posed, in form order. Keeping the verbatim wording here matters: response
distributions can only be read against the precise question and its answer options.

> **PENDING.** To be filled from the form (or its linked responses Sheet — the column headers are the
> questions). For each question record: the **number**, the **verbatim text**, the **type**
> (single-choice / multi-select / scale / short-text / long-text), and the **answer options** where the
> question is closed-form.

| # | Question (verbatim) | Type | Options / scale |
|---|---------------------|------|-----------------|
| 1 | _pending_ | _pending_ | _pending_ |

If a question is added, removed, or reworded after responses already exist, note it in **§5 Change log**
rather than silently editing the table — older response counts were collected against the old wording.

---

## 2. Responses

One subsection per question. Closed-form questions get a small distribution table; open-text questions
get representative excerpts (lightly de-identified) plus a count of how many responses raised each theme.
This section is regenerated wholesale on each refresh — do not hand-edit individual figures.

> **PENDING.** No responses pulled in yet. `n_responses = pending`.

<!-- Template for each closed-form question:

### Q<n> — <short label>

*<verbatim question>* — N = <responses to this question>

| Answer | Count | % of N |
|--------|------:|-------:|
| …      |     … |      … |

-->

<!-- Template for each open-text question:

### Q<n> — <short label>

*<verbatim question>* — N = <responses to this question>

Themes raised (a single response may touch several):

- **<theme>** (<count>) — <one-line gloss>

Representative excerpts (de-identified):

> "<excerpt>"

-->

---

## 3. Synthesis (provisional, descriptive)

What the responses appear to show, stated neutrally and stamped with the N and date they rest on. This is
the *observed* picture, not a claim about what the methodology should do. Resist drawing conclusions here;
flag candidate implications as suggestions for `update-foundation` / `add-guideline` to weigh separately.

> **PENDING.** Fill once responses exist. Keep each observation tied to the specific question(s) it
> rests on, and keep small-N caveats visible — a handful of self-reports from one lab is `weak` to
> `moderate` evidence no matter how clear the pattern looks.

**Candidate attribute links** (to confirm against the actual responses, from
[`foundation/01-ai-attributes.md`](../../../foundation/01-ai-attributes.md)): a survey of self-reported
AI use in a lab is most likely to bear on **A15** (vibes-driven adoption), **A16** (output without
reciprocal skill development), **A13** (the perception gap between felt and actual usefulness), and
**A17** (tasks resisting clean human/AI decomposition). Confirm or drop each once the data is in; do not
assume them.

---

## 4. How to refresh this document

The form keeps receiving responses, so this document is meant to be regenerated, not rewritten. The
cheapest durable setup routes responses through a Google Sheet the toolchain *can* read (Drive Forms are
not directly readable; Sheets are).

**One-time setup (maintainer, in Google Forms):**

1. Open the form → **Responses** tab → **Link to Sheets** → create a new spreadsheet.
2. Record that Sheet's URL/ID in this file's `raw_material` frontmatter field.
3. The Sheet's first row becomes the verbatim question list (fills **§1**); each subsequent row is one
   response (fills **§2**).

**Each refresh (can be done by an assistant via the Drive integration):**

1. Read the linked responses Sheet (Drive MCP `read_file_content` / `download_file_content` support
   spreadsheets).
2. Regenerate **§1** only if questions changed (and log the change in **§5**).
3. Regenerate **§2** wholesale from the current rows.
4. Re-derive **§3** from the new distributions; revisit the `confidence` and `related_attributes`
   frontmatter.
5. Update frontmatter `n_responses` and `as_of`.
6. Add a dated line to **§5 Change log**.
7. Append a one-line entry to that day's `log/` file noting the refresh and the new N.

**Without a linked Sheet (fallback):** the maintainer downloads responses as CSV from the form and the
data is pasted in for a manual regeneration. Works, but every update needs a fresh manual export — the
linked Sheet is preferred precisely because it makes the refresh repeatable.

---

## 5. Change log

Each refresh and each instrument change gets one dated line, newest first. This is what lets a later
reader trust an `as_of` figure and see how the response set grew.

- **2026-06-01** — Document created as an updateable scaffold; awaiting instrument + responses. N = 0.
