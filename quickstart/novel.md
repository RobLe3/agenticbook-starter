# Quick-Start Card: Novel Flavor

> 80K+ words · 15–25+ world model documents · 65–95 sessions

---

```
=== NOVEL FLAVOR QUICK-START ===

WHEN TO USE:
  - Fiction of any genre, narrative non-fiction
  - 80,000+ words
  - 10+ major entities (characters, locations, concepts)
  - Complex structure (multiple timelines, arcs, reveals)
  - Output: Multi-format + publisher submission package

3-DOC STARTER PATH (first output in 60-120 minutes):
  [ ] Concept/outline
  [ ] Style guide
  [ ] Canon/fact registry
  [ ] Generate one test chapter before expanding docs

WORLD MODEL (15-25+ documents):
  Content Tier (7-9 docs):
  [ ] Worldbuilding / Topic Overview
  [ ] Character / Entity Registry (full profiles)
  [ ] Locations (verified, detailed)
  [ ] Lexicon / Terminology
  [ ] Narrative Architecture (all chapters with intent)
  [ ] Psychology / Domain Guide
  [ ] Source Inventory (for non-fiction elements)

  Standards Tier (3-5 docs):
  [ ] Quality scoring (16 dimensions with weights)
  [ ] Style guide (5+ pages: voice + format + conventions)
  [ ] Canon rules (full three-tier hierarchy + update protocol)
  [ ] Story quality assessment (3-pillar engagement)
  [ ] Domain authenticity guide (if applicable)

  Verification Tier (5+ docs):
  [ ] CFR — Character/Claim Fact Registry
  [ ] All 6 logic protocols defined
  [ ] 14-layer verification checklist
  [ ] QVP template (5-layer batch sweep)
  [ ] Reader simulation framework (4 archetypes)

GENERATION SETUP:
  [ ] Full directory structure with /archive/
  [ ] MEMORY.md — Full project knowledge base
  [ ] CLAUDE.md — Complete agent instructions
  [ ] Handover protocol — Session-end handover.md
  [ ] Version control: archive-before-bump + git commits
  [ ] Stats script ready

SESSION PROTOCOL:
  1. Open MEMORY.md + handover.md before starting
  2. Read: chapter outline + character profiles (active)
     + location data + style guide + canon rules
     + preceding chapter endpoint
  3. Build prompt: embed <=5K words of targeted materials
  4. Generate; save immediately; version-stamp
  5. Run voice check (first 500 vs. last 500 words)
  6. Score (16 dims); calibrate (×0.85); log in MEMORY.md
  7. Write handover.md before ending session

VERIFICATION (14 layers, 5-layer QVP sweep):
  Layer 1: CFR — Fact consistency (foundation — do first)
  Layer 2: CETC — Timeline/progression coherence
  Layer 3: Domain accuracy (military, medical, technical)
  Layer 4: KSIB + other logic protocols
  Layer 5: Cross-reference consistency
  Plus: Prose repetition, pacing, accessibility sweeps

QUALITY GATES:
  Draft: >=5.0 calibrated, all format sections present
  Revision: >=7.0 calibrated, no dimension below 6
  Done: >=7.5 calibrated, 5 of 5 ship-it signals

SHIP-IT SIGNALS (need 5 of 5):
  [ ] Quality threshold met (>=7.5 calibrated)
  [ ] At least 3/4 reader archetypes return "Yes"
  [ ] Build: PDF + EPUB + MOBI, all validated
  [ ] Publisher package complete (7-8 documents)
  [ ] Last two revision deltas are micro-gains (<0.3 each)
      or scores plateau across 3 cycles

READER ARCHETYPES (4):
  Fiction: Plausibility-Focused, Human-Impact,
           Momentum-Driven Market, Genre-Literate
  Non-Fiction: Practitioner, Skeptic, Browser, Expert
  Branching: use Fiction set for genre fiction; use Non-Fiction
  set for narrative/memoir; combine 2+2 for literary non-fiction

CALIBRATION RULE (all flavors):
  Raw score ×0.85 = calibrated score
  If agent says 9.0 -> probably 7.5-8.0 (publication quality)
  If agent says 8.0 -> probably 6.8-7.5 (revision quality)
  Trust the lowest score from two passes

DO_DONT CIRCUIT BREAKER (all flavors):
  Before running another revision:
    Don't iterate because the system allows it
    Don't chase micro-gains
    Do stop when reader models converge
    Do notice boredom or resistance

TYPICAL SESSION COUNT:
  World model: 10-14 sessions
  Generation: ~1 session per chapter × 25-30 chapters
  Verification: 10-14 sessions (5-layer QVP)
  Revision: 12-18 sessions (8-12 passes)
  Build + package: 5-7 sessions
  Total: 65-95 sessions
```

---

## Worked Example: The Glass Meridian

The companion repository includes a complete Novel-flavor world model for *The Glass Meridian* — a literary mystery / historical thriller with a dual timeline (2024 Azores/London and 1872 Gold Coast/Atlantic/Liverpool), 82,000–88,000 words, 28 chapters plus prologue and epilogue.

**What it demonstrates:**
- Full 17-document world model (Docs 00–16) across Content, Standards, and Verification tiers
- Dual-timeline narrative architecture (30-entry chapter map with chapter intent per entry)
- Character registry with psychological profiles (wound/desire/fear/ghost) for 8 characters
- Location register with sensory anchors and 2024 vs 1872 contrast per location
- 16-dimension quality scoring rubric with weighted formula and ×0.85 calibration
- 14-layer verification protocol across three sweeps
- 4-archetype reader simulation framework for fiction

**Location in repo:** `novel-example/` (worked example) and `novel-blank/` (blank templates)

**Key contrast with Topic-flavor:** Adds a character registry (Doc 02), location register (Doc 03), psychology guide (Doc 06), story quality assessment (Doc 11), domain authenticity protocol (Doc 12), and four additional verification documents (Docs 13–16 vs Topic's Docs 07–09).

**Why this topic:** *The Glass Meridian* is fiction with two distinct research domains (marine archaeology and colonial West African history). It is deliberately unrelated to AI or writing methodology — demonstrating that the Novel-flavor world model works for any genre and subject matter.

```
novel-example/
├── 00_index.md              # Navigation + session checklist + flavor contrast table
├── 01_premise.md            # Logline, comparable titles, scope guardrails
├── 02_character_registry.md # 8 characters with full psychological profiles
├── 03_location_register.md  # 10 locations with sensory anchors and dual-era contrast
├── 04_glossary.md           # 30 terms across 3 categories (marine / colonial / craft)
├── 05_narrative_architecture.md  # 30-entry chapter map + 5-act arc + session plan
├── 06_psychology_guide.md   # Wound/desire/fear/ghost for 4 main characters
├── 07_research_foundation.md # Claims by verification risk + known vs. needs-verify
├── 08_quality_scoring.md    # 16 dimensions + weighted formula + Quick-Score card
├── 09_style_guide.md        # Voice differentiation + FID + tense + jargon policy
├── 10_canon_rules.md        # Three-tier hierarchy + binary conflict resolution
├── 11_story_quality.md      # 3-pillar framework (Plausibility / Human Impact / Momentum)
├── 12_domain_authenticity.md # Fixed procedures + "what does NOT happen" lists
├── 13_cfr.md                # CF-001–CF-026 (character facts) + HC-001–HC-030 (history)
├── 14_verification_protocol.md # All 14 layers in 3 sweeps with gate conditions
├── 15_vfr.md                # 20 entries across 4 categories with recheck triggers
└── 16_reader_simulation.md  # 4 fiction archetypes + 3/4 gate + pillar-to-archetype map
```

Blank templates with `[PLACEHOLDER_NAME]` format are in `novel-blank/` — same structure, all Glass Meridian content replaced, all `> Note for agent:` methodology annotations preserved.
