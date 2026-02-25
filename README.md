# agenticbook-starter

**A reader-facing bootstrap companion for *Agentic Book Writing: The Smart Way*.**

This repository contains a filled Short-flavor example world model for a fictional project — *First Light: A Beginner's Guide to Night Sky Photography* — plus the static prompt library, flavor quick-start cards, and versioned tool guides from the book's appendices.

Use this as:
- A **reference** while reading the book (Option C — no clone required)
- A **starter scaffold** to copy and adapt (Option A or B — clone and customize)
- A **complete teaching example** for core world-model concepts before you build your own

---

## Boundary (Read First)

This starter kit is an external companion repository.
It is **not** the production world model for the Agentic Book manuscript.

- Starter kit role: fast reader onboarding and bootstrap execution
- Production role: canonical methodology and manuscript claims

Do not treat starter file names or starter simplifications as production canon.

---

## What's in This Repo

```text
agenticbook-starter/
├── CLAUDE.md                  # Filled example agent instruction file (First Light)
├── MEMORY.md                  # Filled example session tracking file (First Light)
├── docs/                      # Example world model (Short-flavor, First Light)
│   ├── 00_index.md            # Navigation + phase tracker
│   ├── 01_book_concept.md     # Problem statement, unique value, scope guardrails
│   ├── 02_target_readers.md   # Two reader personas + jargon tolerance
│   ├── 03_book_architecture.md # Chapter outline + lab structure + word targets
│   ├── 04_key_concepts.md     # 18-term glossary with Short-flavor depth markers
│   ├── 05_case_study.md       # Author credentials + project evidence
│   ├── 06_verification_lite.md # CFR/consistency/cross-ref checks (3 layers)  [optional]
│   ├── 07_vfr_lite.md         # Volatile-claim tracking (lightweight VFR)     [optional]
│   └── 08_prepublication_checklist.md  # Lightweight release gate             [optional]
├── blank/                     # Empty templates matching all docs/ files
│   ├── 00_index_blank.md
│   ├── 01_concept_blank.md
│   ├── 02_readers_blank.md
│   ├── 03_architecture_blank.md
│   ├── 04_glossary_blank.md
│   ├── 05_casestudy_blank.md
│   ├── 06_verification_lite_blank.md        [optional]
│   ├── 07_vfr_lite_blank.md                 [optional]
│   └── 08_prepublication_checklist_blank.md [optional]
├── quickstart/                # Flavor quick-start cards (Appendix C)
│   ├── README.md
│   ├── short.md               # Short flavor: 20-40K words, 15-20 sessions
│   ├── topic.md               # Topic flavor: 50-80K words, 30-50 sessions
│   └── novel.md               # Novel flavor: 80K+ words, 65-95 sessions
├── prompts/                   # Static prompt library (Appendix D)
│   ├── README.md
│   ├── stage-1-concept.md     # STRUO, ANALY, COMPR
│   ├── stage-2-writing.md     # CHDD, CHFO, SUBREF
│   ├── stage-3-refinement.md  # COREF, STRAL, COMAC, CAM
│   ├── stage-4-review.md      # AASS, DARE, IRIN + Reader Simulation
│   ├── stage-5-illustration.md # Visual briefs, captions
│   └── stage-6-supplemental.md # Author bio, blurb, metadata
└── tools/                     # Versioned tool guides (Appendix B)
    ├── README.md
    ├── tool-tiers.md           # Tier table with current versions
    ├── claude-code.md          # Tier 2 setup guide
    ├── latex-setup.md          # XeLaTeX for Novel flavor (versioned)
    ├── markdown-setup.md       # Pandoc for Short/Topic flavor (versioned)
    ├── version-control.md      # Git setup for book projects
    └── stats-script.md         # Stats script with customization notes
```

---

## How to Use This

### Option A: Start from the example (fastest — ⚡ FAST route)

1. Clone this repo alongside your book project:
   ```bash
   git clone https://github.com/RobLe3/agenticbook-starter.git starter
   cd starter
   ```
2. Open `CLAUDE.md` and replace `First Light` content with your own project.
3. Open `MEMORY.md` and fill in your project details.
4. Open `docs/00_index.md` — this is your session navigation file.
5. Open the `docs/` example files as reference; open the `blank/` files to fill in.
6. Run Lab E (Appendix E of the book) for the full onboarding walkthrough.

### Option B: Start from blank files (most flexible)

1. Clone this repo.
2. Copy files from `blank/` into your project `docs/` folder.
3. Fill core docs first (`00`–`05`), then optional ops docs (`06`–`08`) when needed.
4. Use the `docs/` examples for reference while filling in the blanks.

### Option C: Reference only (no clone required)

Browse the repository on GitHub while reading Chapters 3–15 of the book. When a chapter introduces a document type, open the corresponding starter file to see a complete worked example. No setup required — every file is readable in GitHub's web interface.

---

## Chapter-to-Folder Mapping

| Chapters | What to use |
|----------|-------------|
| Ch 3–5 (World Model Concept, Workshop Setup, Content Docs) | `docs/` + `blank/` |
| Ch 6–7 (Standards, Verification) | `docs/06_verification_lite.md` + `docs/07_vfr_lite.md` |
| Ch 8 (Flavor Matrix) | `quickstart/` (compare all three flavor cards) |
| Ch 9–10 (Generation, Measurement) | `prompts/stage-2-writing.md` + `prompts/stage-4-review.md` |
| Ch 11–12 (Revision, Reader Validation) | `prompts/stage-3-refinement.md` + `prompts/stage-4-review.md` |
| Ch 13–15 (Build, Publisher Package, Done) | `tools/` + `prompts/stage-6-supplemental.md` |
| Appendix C | `quickstart/` |
| Appendix D | `prompts/` |
| Appendix B | `tools/` |

---

## Starter → Production Mapping

| Starter Asset | Starter Role | Production Equivalent |
|---|---|---|
| `CLAUDE.md` (filled example) | Agent instruction file for First Light | Your own CLAUDE.md adapted from blank |
| `MEMORY.md` (filled example) | Session tracking for First Light | Your own MEMORY.md |
| `docs/00_index.md` | Session navigation | World-model index pattern (Template 01) |
| `docs/01–05` | Core Short-flavor content docs | Content + standards templates (Templates 02–06) |
| `docs/06_verification_lite.md` | 3-layer verification gate | Full verification stack (Template 07 + Template 08) |
| `docs/07_vfr_lite.md` | Volatile-claim tracking (minimal) | Full VFR workflow |
| `quickstart/` | Flavor cards (reference + session protocol) | Templates 16/17/18 (per flavor) |
| `prompts/` | Static prompt library (Phase 0 + supplement) | Templates 10–15 (world-model-grounded prompts) |
| `tools/` | Versioned install + tool guides | Appendix B (illustrative) + your own tool stack |

---

## When to Graduate from the Starter Kit

Move to the full methodology when any of these are true:

- Your target exceeds ~40,000 words
- You are beyond Chapter 5–8 and context drift appears
- Re-stating context takes longer than writing
- Cross-chapter contradictions keep recurring
- You need advanced verification, multi-format output, or a publisher submission package

---

## The Example Project

**Title:** *First Light: A Beginner's Guide to Night Sky Photography*
**Flavor:** Short (22,000–28,000 words)
**Genre:** Non-fiction how-to / beginner guide
**Why this topic:** Night sky photography is unrelated to AI or writing — demonstrating that the methodology works for any subject matter.

---

## Version

This repository is described in *Agentic Book Writing: The Smart Way* at tag **v0.6.0** (February 2026). If the repository structure has changed since this tag, see the tagged release or the archived ZIP at the book's download page.

---

## Book

*Agentic Book Writing: The Smart Way* by Roble Mumin — [roblemumin.com](https://roblemumin.com)
