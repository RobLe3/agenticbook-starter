<!--
Book reference: This example supports Lab 5 (Chapter 5: Content Documents).
If you completed Lab 5, compare your concept doc to this one.
Differences are expected — this is a different project (Short-flavor, photography guide).
Look for: premise clarity, problem statement specificity, scope guardrails, transformation test.
-->

# Doc 01: Book Concept

> **Example world model doc for *Agentic Book Writing: The Smart Way* — Chapter 5.**
> This document answers: What is this book? Who is it for? Why does it need to exist?
> Your agent embeds this in every chapter-generation prompt to anchor the work.
> *Book Lab → Lab 5 (Chapter 5). If you completed Lab 5, compare your concept doc to this one — look for: premise clarity, problem statement specificity, scope guardrails, transformation test.*

---

## Working Title

*First Light: A Beginner's Guide to Night Sky Photography*

> **Why this title:** "First Light" is the astronomy term for the first time a telescope
> or camera is pointed at the sky. It signals insider knowledge without jargon, and it
> captures the emotional experience of the intended reader — the feeling of seeing the
> Milky Way through their own lens for the first time.

**Subtitle candidate:** *How to photograph the night sky without expensive gear, dark-sky permits, or a physics degree*

---

## One-Line Premise

A practical, beginner-focused guide to night sky photography that starts with a smartphone and ends with a reader who can produce a publication-quality Milky Way image — within their first month of trying.

---

## The Problem This Book Solves

Most night sky photography guides assume you already own a DSLR, know what ISO means, and live near a certified dark-sky site. Beginners pick them up, hit the first gear list, and put them down.

The result: millions of people who have looked up at the Milky Way and thought "I want to photograph that" never do — not because the photography is hard, but because the entry path is invisible.

This book makes the entry path visible. Chapter 1 starts with a smartphone. Chapter 7 ends with a DSLR and a print-quality image. Every chapter in between adds exactly one new skill, one new piece of equipment, or one new location strategy — and nothing more.

> **Note for agent:** The problem statement is the emotional anchor. When writing any chapter,
> return to this: a reader who wants to photograph the night sky but doesn't know where to start.
> Every explanation, every technique, every example serves that reader.

---

## Core Thesis

You do not need expensive gear to take beautiful night sky photographs. You need the right technique for the gear you already own, and the knowledge to know when conditions are right.

---

## Unique Value

**What makes this book different from competitors:**

1. **Gear-progressive structure.** The book is organized not by topic (exposure, composition, location) but by gear level (smartphone → entry DSLR → full-frame). Most readers can find their current level and start there, rather than reading the whole book linearly.

2. **One-skill-per-chapter discipline.** Each chapter teaches exactly one skill and produces one tangible output (a photo with a specific quality). No chapter asks the reader to learn three new concepts simultaneously.

3. **Honest about weather and light pollution.** Most guides assume the reader has access to dark skies. This book starts from the assumption that most readers live near cities and includes dedicated sections on photographing from light-polluted environments.

---

## Book Specifications

> **Keep these numbers visible.** Your agent needs them when generating chapter prose
> (for accurate "you'll learn X in Chapter N" forward references) and when the word count
> per chapter needs to match the target.

| Field | Value |
|-------|-------|
| Flavor | Short |
| Target word count | 22,000–28,000 words |
| Chapters | 7 + Introduction |
| Target chapter length | 2,500–3,500 words each |
| Format | Print + eBook (Markdown → PDF via Pandoc) |
| Lab exercises | 7 (one per chapter; each produces a real photograph) |

---

## Market Position

**Comparable titles:**
- *The Backyard Astronomer's Guide* (Dickinson & Dyer) — broad astronomy; photography is secondary
- *iPhone Night Sky Photography* (Dyer) — phone-only; does not progress to DSLR
- *Nightscape Photography* (Rowell) — beautiful but assumes advanced equipment

*First Light* occupies the gap: gear-progressive, beginner-specific, urban-to-rural path.

**Primary retail category:** Photography > Night Photography
**Secondary category:** Astronomy > Amateur Astronomy

---

## What the Reader Can Do After Reading

> **The "transformation test."** Every chapter should move the reader one step closer to
> this outcome. If a chapter doesn't contribute to this transformation, it doesn't belong.

A reader who completes this book can:
1. Photograph star trails with a smartphone from their backyard tonight
2. Select the right DSLR settings (ISO, aperture, shutter speed) for their equipment and location
3. Find and evaluate dark-sky sites within driving distance
4. Plan a Milky Way shoot around moon phase, season, and weather
5. Produce a processed image good enough to print at 8×10 inches or larger

---

## Scope Guardrails

> **What this book does NOT cover.** Write these down to prevent scope creep in generation.
> If your agent tries to include these topics, redirect to this list.

- **Astrophotography with telescopes** — out of scope; different equipment class
- **Deep-sky objects (nebulae, galaxies beyond the Milky Way)** — out of scope; requires tracking mounts
- **Advanced image stacking** — mentioned briefly; not a core skill at this level
- **Videography or time-lapse** — out of scope; different skill set
- **Gear reviews or purchasing advice** — not a gear guide; techniques are equipment-agnostic where possible
