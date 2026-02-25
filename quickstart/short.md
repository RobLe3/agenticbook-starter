# Quick-Start Card: Short Flavor

> 20–40K words · 4–6 world model documents · 15–20 sessions

No world model yet? The Static Prompt Library (`prompts/stage-1-concept.md`) provides a Phase 0 on-ramp — structured prompts that generate Short-flavor chapters without infrastructure. See `prompts/` for the full library.

---

```
=== SHORT FLAVOR QUICK-START ===

WHEN TO USE:
  - Non-fiction guide, handbook, pamphlet, or novella
  - Under 40,000 words
  - 1-3 major entities (characters, topics, locations)
  - Linear structure (chapters are mostly independent)
  - Output: PDF for personal use or limited distribution

3-DOC STARTER PATH (first output in 60-120 minutes):
  [ ] Concept/outline
  [ ] Style guide
  [ ] Fact registry
  [ ] Generate one test chapter before expanding docs

WORLD MODEL (4-6 documents, build before writing):
  [ ] Concept doc — What you're writing and why (500-1K words)
  [ ] Outline — Chapter structure with intent (500-1K words)
  [ ] Style guide — Voice decisions + 2 exemplar paragraphs
  [ ] Fact registry (CFR) — Claims that must be consistent

GENERATION SETUP:
  [ ] Directory: /project/docs/, /manuscript/, /output/
  [ ] MEMORY.md — Project name, flavor, key decisions
  [ ] Generation prompt: embed concept + outline + style guide
  [ ] [VERIFY] flag — Required in every prompt

SESSION PROTOCOL:
  1. Read relevant world model docs before prompting
  2. Build prompt: context → constraints → material → instruction
  3. Generate and save immediately (v01, v02...)
  4. Score against 8 dimensions; apply ×0.85 correction
  5. Log: chapter, date, calibrated score, next target

VERIFICATION:
  [ ] CFR pass (full text — it's under 40K, just do it)
  [ ] Prose repetition check (one pass)

QUALITY GATES:
  Draft: >=5.0 calibrated, all sections present
  Revision: >=6.5 calibrated, Clarity >=7
  Done: >=7.5 calibrated, 3 of 5 ship-it signals

SHIP-IT SIGNALS (need 3 of 5):
  [ ] Quality threshold met (>=7.5 calibrated)
  [ ] 2/2 reader archetypes return "Yes"
  [ ] Build produces valid PDF
  [ ] Product description complete
  [ ] Last revision delta <0.3 points

DO_DONT CIRCUIT BREAKER (all flavors):
  Before running another revision:
    Don't iterate because the system allows it
    Don't chase micro-gains
    Do stop when reader models converge
    Do notice boredom or resistance

CALIBRATION RULE (all flavors):
  Raw score x0.85 = calibrated score
  If agent says 9.0 -> probably 7.5-8.0 (publication quality)
  If agent says 8.0 -> probably 6.8-7.5 (revision quality)
  Trust the lowest score from two passes

TYPICAL SESSION COUNT:
  World model: 2-3 sessions
  Generation: 1 session per chapter
  Verification: 1-2 sessions
  Revision: 2-3 sessions
  Build: 1 session
  Total: 15-20 sessions
```
