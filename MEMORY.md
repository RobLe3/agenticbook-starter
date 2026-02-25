# First Light — Agent Memory

> **Note for reader:** This is a filled example for the *First Light* project.
> To use this for your own project: replace the project-specific content below
> with your own. See `blank/` for blank templates.

> **How to use this file:** This file is read by your AI agent at the start of every session.
> Add to it whenever you make a decision that the agent would otherwise need to re-invent.
> Keep it under 2,000 words — if it grows beyond that, archive older entries to their own files.

---

## Project Overview

- **Title:** *First Light: A Beginner's Guide to Night Sky Photography*
- **Subtitle:** *How to photograph the night sky without expensive gear, dark-sky permits, or a physics degree*
- **Flavor:** Short
- **Target word count:** 22,000–28,000 words
- **Target audience:** Complete beginners who want to photograph the night sky; own a smartphone or entry-level camera; live near cities (light-polluted environment assumed)
- **Core premise:** Most night sky photography guides assume gear and dark-sky access the reader doesn't have. This book starts from a smartphone and a city backyard, and progresses to DSLR + dark-sky planning by Chapter 7. Every chapter teaches exactly one skill and produces one photograph.

---

## Current Phase

**Phase:** 1 (World Model Construction) — COMPLETE
**Current work:** World model is complete. Ready to begin Phase 2 (First Draft Generation).
**Last session:** World model finalized — all 8 docs complete (00–08).
**Next session:** Begin Chapter 1 (Introduction to Night Sky Photography). Load CLAUDE.md + MEMORY.md + docs/00_index.md + docs/01_book_concept.md + docs/02_target_readers.md + docs/03_book_architecture.md before generating.

---

## Key Decisions Made

- 2026-02 — **Gear-progressive structure** — Organize chapters by gear level, not by topic. Reason: most beginner guides assume gear the reader doesn't own. Starting with a smartphone removes the first barrier.
- 2026-02 — **One-skill-per-chapter rule** — Each chapter must teach exactly one skill and produce one photograph. Reason: reduces cognitive load; gives the reader a clear win per session.
- 2026-02 — **Telescopes are out of scope** — Even though many night sky photographers eventually use telescopes, including them would require a different book. Explicitly out of scope per Doc 01.
- 2026-02 — **Urban-first assumption** — Most readers live near cities. Light-pollution workarounds are covered in every relevant chapter, not just a dedicated chapter at the end.
- 2026-02 — **Markdown source format** — Short flavor; Pandoc compilation to PDF + EPUB is sufficient. No LaTeX required.

---

## World Model File Status

| File | Status | Last Updated |
|------|--------|-------------|
| `docs/00_index.md` | COMPLETE | 2026-02 |
| `docs/01_book_concept.md` | COMPLETE | 2026-02 |
| `docs/02_target_readers.md` | COMPLETE | 2026-02 |
| `docs/03_book_architecture.md` | COMPLETE | 2026-02 |
| `docs/04_key_concepts.md` | COMPLETE | 2026-02 |
| `docs/05_case_study.md` | COMPLETE | 2026-02 |
| `docs/06_verification_lite.md` | COMPLETE | 2026-02 |
| `docs/07_vfr_lite.md` | COMPLETE | 2026-02 |
| `docs/08_prepublication_checklist.md` | COMPLETE | 2026-02 |

---

## Manuscript File Status

> Add a row for each chapter as you draft it.

| Chapter | Status | Word Count | Score (calibrated) |
|---------|--------|------------|-------------------|
| Introduction | Not started | — | — |
| Ch 1: Your Smartphone and the Night Sky | Not started | — | — |
| Ch 2: Understanding Light and Darkness | Not started | — | — |
| Ch 3: Finding Your First Dark Spot | Not started | — | — |
| Ch 4: Star Trails — Your First Composition | Not started | — | — |
| Ch 5: Moving Up to a Dedicated Camera | Not started | — | — |
| Ch 6: The Milky Way — Planning and Execution | Not started | — | — |
| Ch 7: Processing Your Best Shot | Not started | — | — |

---

## Important Conventions

- **Gear levels:** smartphone (Ch 1–3), entry DSLR (Ch 4–6), processing (Ch 7). Do not mix within a chapter.
- **Calibration:** all AI quality scores ×0.85 before logging. Never log raw scores.
- **`[VERIFY]` tag:** required for any technical claim (f-stop recommendations, ISO ranges, shutter speed guidance). Always include source or note that verification is needed.
- **Scope redirect:** if content about telescopes, deep-sky objects (nebulae/galaxies), or advanced image stacking comes up, redirect to scope guardrails in Doc 01.

---

## Problems Solved

> Log problems so you don't solve them twice.

- No problems logged yet — manuscript not started.
