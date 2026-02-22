# Project Instructions — [Your Book Title]

> **How to use this file:** This file tells Claude Code (or any coding agent) the rules
> for working on this specific project. Copy this starter and customize it.
> Keep it under 800 words — longer files slow down every session.

---

## What This Project Is

[1–2 sentences describing your book. Copy from Doc 01.]

**Flavor:** [Short / Topic / Novel]
**World model location:** `docs/`
**Manuscript location:** `manuscript/`

---

## My Role / Your Role

I am the architect. You are the builder.
I make creative decisions. You implement them.
When in doubt about a structural decision, ask. When in doubt about a prose decision, make a choice and note it.

---

## Reading Order (Every Session)

Before doing anything else, read:
1. `MEMORY.md` — Current project state and decisions
2. `docs/00_index.md` — World model navigation
3. The specific docs relevant to today's task (listed in MEMORY.md "Current work")

Do not write any content before reading these three files.

---

## Writing Rules

- **Voice:** [Second person "you" / First person / Third person — your choice]
- **Jargon:** Define every technical term on first use; assume no prior knowledge unless Doc 02 specifies otherwise
- **Examples:** Draw only from Doc 05 (case study) for "author experience" examples; do not invent new author experiences
- **Length:** Target [number] words per chapter; flag if you are significantly over or under
- **Callout boxes:** Use sparingly — one per major section maximum
- **Tables and lists:** Always introduce with at least one sentence explaining what follows; always follow with at least one sentence synthesizing the key takeaway

---

## DO

- Read the relevant world model docs before writing anything
- Ask before making structural decisions (adding/removing sections, changing chapter scope)
- Update `MEMORY.md` at the end of each session with decisions made
- Flag contradictions between world model docs instead of resolving them yourself
- Mark uncertain facts with [VERIFY] rather than guessing

---

## DO NOT

- Invent facts not established in the world model
- Invent author experiences not documented in Doc 05
- Skip the quality scoring step after generating a chapter
- Start a new chapter without checking MEMORY.md for the current state
- Make prose decisions autonomously that contradict the style guide

---

## Quality Check (After Every Chapter)

Before declaring a chapter complete, verify:
1. Does every table and list have an intro sentence and a synthesis sentence? (Pacing)
2. Does every technical term get defined on first use? (Clarity)
3. Does every "author experience" example trace to Doc 05? (Grounding)
4. Is the chapter within 20% of its target word count? (Scope Discipline)
5. Does the lab (as specified in Doc 03) produce a specific, tangible artifact? (Actionability)
6. Apply the 15% calibration correction to any AI quality score — AI self-assessment inflates by ~15%. A raw score of 8.0 = 6.8 calibrated.

---

## Session End Protocol

Before ending any session:
1. Save all open files
2. Update `MEMORY.md`: add decisions made, update chapter word counts, update "Next session"
3. Commit: `git add docs/ manuscript/ MEMORY.md && git commit -m "[brief description of what was done]"`
   (Add only project files — never add .env files, credentials, or API keys)
