# Quick-Start Card: Topic Flavor

> 50–80K words · 8–12 world model documents · 30–50 sessions

---

```
=== TOPIC FLAVOR QUICK-START ===

WHEN TO USE:
  - Non-fiction: how-to, business book, technical guide
  - 50,000-80,000 words
  - 4-10 major concepts, topics, or case studies
  - Moderate structure (parallel threads, cross-references)
  - Output: PDF + EPUB for wider distribution

3-DOC STARTER PATH (first output in 60-120 minutes):
  [ ] Topic overview/outline
  [ ] Style guide
  [ ] Canon/fact registry
  [ ] Generate one test chapter before expanding docs

WORLD MODEL (8-12 documents, build before writing):
  Content Tier:
  [ ] Topic overview — Scope, boundaries, key concepts
  [ ] Entity registry — Topics, concepts, case studies
  [ ] Source inventory — References, evidence, examples
  [ ] Argument structure — Thesis per chapter, logic map
  [ ] Structural outline — 10-15 chapters with intent

  Standards Tier:
  [ ] Style guide — Voice, jargon, exemplars (2-3 pages)
  [ ] Quality scoring — 12 dimensions with weights
  [ ] Canon rules — Three-tier hierarchy

  Verification Tier:
  [ ] CFR (Character/Claim Fact Registry)
  [ ] Verification checklist — CFR + IAC + KSIB defined

GENERATION SETUP:
  [ ] Directory: /docs/, /manuscript/, /output/, /archive/
  [ ] MEMORY.md — Project facts, key decisions, anti-patterns
  [ ] CLAUDE.md — Agent behavior instructions
  [ ] Version control: semantic versioning (v1.0, v1.1...)

SESSION PROTOCOL:
  1. Read chapter outline entry + relevant entity data
  2. Build prompt: context → constraints (<=15 items) →
     material (<=5K words embedded) → instruction
  3. Embed: outline + entity data + style guide + canon rules
     + preceding chapter endpoint
  4. Generate; save immediately; add to version log
  5. Score (12 dims); calibrate (×0.85); log delta

VERIFICATION (3-8 layers):
  [ ] CFR pass (full text, ~3K-line batches)
  [ ] IAC coherence check (argument follows premises)
  [ ] KSIB check (concepts introduced before referenced)
  [ ] Prose repetition sweep
  [ ] Cross-reference audit (check "See Chapter N" entries)

QUALITY GATES:
  Draft: >=5.0 calibrated, all sections present
  Revision: >=7.0 calibrated, no dimension below 6
  Done: >=7.5 calibrated, 4 of 5 ship-it signals

SHIP-IT SIGNALS (need 4 of 5):
  [ ] Quality threshold met (>=7.5 calibrated)
  [ ] At least 2/3 reader archetypes return "Yes"
  [ ] Build produces valid PDF + EPUB
  [ ] Package complete (query/proposal + bio + sample)
  [ ] Last two revision deltas are micro-gains (<0.3 each)
      or scores plateau across 3 cycles

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

READER ARCHETYPES (3):
  The Practitioner — "Can I use this?"
  The Skeptic — "Is this proven?"
  The Browser — "Is this interesting?"

TYPICAL SESSION COUNT:
  World model: 6-8 sessions
  Generation: 1-2 sessions per chapter × 12-15 chapters
  Verification: 6-8 sessions (8-layer verification, 3-5 QVP passes)
  Revision: 4-6 sessions (2-3 passes)
  Build + package: 3-4 sessions
  Total: 30-50 sessions
```

---

## Worked Example (Topic-Flavor)

The companion repository includes a complete Topic-flavor world model example:

**`topic-example/`** — *Sourdough at Home: A Practical Guide to Wild Yeast Baking*

| File | What it demonstrates |
|------|---------------------|
| `00_index.md` | Navigation + flavor comparison vs Short-flavor |
| `01–05` | Full Content tier (concept, readers, architecture, glossary, case study) |
| `06_style_guide.md` | Standards tier — voice, jargon policy, callout boxes |
| `07_canon_rules.md` | CFR — 46 technical claims across 7 categories |
| `08_verification_protocol.md` | 8-layer verification protocol |
| `09_vfr.md` | Volatile Facts Register — 19 claims with recheck triggers |

Compare this to the Short-flavor example (`docs/`) to see what Topic-flavor adds:
- Doc 06 (style guide) — new requirement at Topic-flavor
- Doc 07 (CFR) — dedicated fact registry, not just lite consistency checks
- Doc 08 (full 8-layer verification) vs Short's 3-layer lite
- Doc 09 (full VFR) vs Short's 6-item VFR-lite

**Blank templates:** `topic-blank/` — matching templates with `[PLACEHOLDER_NAME]` format.

If you completed Lab 6–7 (Chapters 6–7), compare your standards and verification docs to
`topic-example/06–09` to calibrate depth.
