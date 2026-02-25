# Project Instructions — First Light: A Beginner's Guide to Night Sky Photography

> **Note for reader:** This is a filled example for the *First Light* project.
> To use this for your own project: replace the project-specific content below
> with your own. See `blank/01_concept_blank.md` for a blank template.

---

## Boundary and Scope

This repository is the **starter kit** (bootstrap companion), not the production methodology repository.

- Use this kit for fast execution and learning the core loop.
- Do not assume starter file names or simplifications are production canon.
- If you need deeper methodology, graduate to the full system (see graduation triggers below).

---

## What This Project Is

*First Light: A Beginner's Guide to Night Sky Photography* is a Short-flavor practical guide for beginners who want to photograph the night sky but don't know where to start. The book is gear-progressive: it starts with a smartphone and ends with a DSLR producing a print-quality Milky Way image. Every chapter teaches exactly one skill and produces one tangible photograph.

**Flavor:** Short
**World model location:** `docs/`
**Manuscript location:** `manuscript/`
**Format:** Markdown → PDF via Pandoc (+ optional EPUB)

---

## Reading Order (Every Session)

Before doing anything else, read:
1. `MEMORY.md`
2. `docs/00_index.md`
3. Task-relevant core docs (`docs/01`–`05`)
4. Optional ops docs (`docs/06`–`08`) if this session includes verification, volatile claims, or release checks

Do not write content before reading these files.

---

## Writing Rules

- **Voice:** Second person ("you") — direct, warm, non-condescending
- **Tone:** Patient guide, not expert asserting status. The reader is a beginner; never make them feel behind.
- **Jargon:** Define technical photography terms (ISO, aperture, shutter speed, f-stop) on first use; repeat the definition at the chapter where it becomes a working skill, not just a concept.
- **Examples:** Draw only from Doc 05 (author credentials and project evidence) for author-experience examples. Do not invent experiences.
- **Length:** Target 2,500–3,500 words per chapter. Flag variance above 4,000 words.
- **Formatting:** Introduce every table and step-list with a lead sentence. Follow every numbered procedure with a brief "what you should see" note.
- **Chapters:** Each chapter must produce one tangible lab output — a real photograph, not a conceptual exercise.

---

## DO

- Read relevant world model docs before writing
- Ask before structural scope changes (adding chapters, splitting chapters, changing chapter order)
- Update `MEMORY.md` at session end with decisions and next action
- Flag contradictions between docs instead of silently resolving them — write `[CONFLICT: Doc X vs Doc Y]` and flag it
- Mark uncertain facts with `[VERIFY]` — never assert technical accuracy without a source
- Keep gear-progressive structure: smartphone first, DSLR later, telescopes never

---

## DO NOT

- Invent facts not in the world model — especially camera specifications, app prices, or astrophotography claims
- Invent author experiences not in Doc 05
- Skip quality scoring and calibration (apply ×0.85 to all AI self-assessment scores)
- Start a new chapter without checking current state in MEMORY.md
- Mix gear levels within a chapter (smartphone techniques and DSLR techniques are in separate chapters)
- Include telescope astrophotography — this is explicitly out of scope (see Doc 01 Scope Guardrails)

---

## Quality Check (After Every Chapter)

Before declaring a chapter complete:
1. Step-list intro and summary present
2. Photography terms defined on first use
3. Author-experience examples trace to Doc 05
4. Chapter within 20% of target (2,500–3,500 words)
5. Lab output is a specific, achievable photograph (not a generic exercise)
6. Apply ×0.85 calibration correction to AI quality scores
7. Gear level is consistent throughout (no cross-level mixing)

---

## Graduation Triggers (Switch to Full Methodology)

If any trigger is true, stop extending this starter and move to the full methodology:
- Target word count exceeds ~40,000 words
- Chapter count exceeds 10 with recurring drift between chapters
- Context restatement overhead is high each session (you are re-explaining the same concepts)
- Verification-lite no longer catches contradictions (especially around gear specifications)
- You need multi-format output (PDF + EPUB + print) or a publisher submission package

---

## Session End Protocol

1. Save all files
2. Update `MEMORY.md` with: decisions made, word counts, calibrated scores, next action
3. Commit only project files — never secrets, API keys, or personal credentials
