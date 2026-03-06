# Quick-Start Card: Before You Begin

> Not sure which flavor fits your project? Start here. · 15 minutes to your first scored output.

---

```
=== BEFORE YOU BEGIN ===

CHOOSE YOUR FLAVOR (60 seconds):
  Short  (<=40K words  · 4-6 docs  · 15-20 sessions)
    Best for: guides, handbooks, pamphlets, novellas
  Topic  (50-80K words · 8-12 docs · 30-50 sessions)
    Best for: non-fiction, business books, technical guides
  Novel  (80K+ words   · 15-25+ docs · 65-95 sessions)
    Best for: fiction, narrative non-fiction

  Rule: start Short or Topic. Novel requires the full
  methodology — do not start there on your first project.

CHOOSE YOUR ROUTE:
  GREEN  (8-12 wks · coherence 88/100)
    Every chapter, every lab. Full system from scratch.
    Use when: this is your first AI-assisted project.
  YELLOW (4-6 wks · coherence 85/100)
    Core methodology + labs that match your output type.
    Use when: you already understand prompting and want
    to apply a system to a project in motion.
  FAST   (1-2 wks · starter kit only)
    These four documents + one test chapter. Ship fast,
    graduate to YELLOW when drift appears.
    Use when: you need proof of concept before committing.

THE 4 STARTER DOCUMENTS (build before any chapter):
  Create a docs/ folder. Build these four — in order.

  [ ] 00_index.md
      Navigation guide for your project. One page.
      Keeps every session anchored. Start here.

  [ ] 01_concept.md
      What your book is. Core thesis, scope, one-sentence
      value promise. (500-1,000 words)

  [ ] 02_readers.md
      Who reads this. 2-3 reader types with goals and
      fears. (300-600 words)

  [ ] 03_architecture.md
      Chapter list with one-sentence intent per chapter.
      (500-1,000 words)

  Core rule: "The world model is the product, not the
  manuscript." Build the model before writing a word.

LAB 0 — PROVE IT (15 minutes):
  1. Create your docs/ folder and open 01_concept.md
  2. Write your concept in one paragraph:
     - What the book is
     - Who it's for
     - What the reader can do after finishing it
  3. Paste it into your AI agent with this prompt:
     "Score this concept 1-10 on clarity, specificity,
     and reader value. List three gaps."
  4. Revise until the agent scores it 8+

  Success signal: a scored, improved concept statement.
  That is your world model starting.

WEEK-1 ANTI-PATTERN GUARDRAILS:
  Mistake: Starting with the manuscript
  Fix:     Build the 4 starter docs first. Every time.

  Mistake: Skipping the world model entirely
  Fix:     The model is the product. The manuscript is
           the output. One produces the other.

  Mistake: Re-prompting without reading the last output
  Fix:     Read the output. Score it. Then prompt again.

CALIBRATION RULE (applies from session one):
  Raw score x0.85 = calibrated score
  If agent says 9.0 -> probably 7.5-8.0 (publication quality)
  If agent says 8.0 -> probably 6.8-7.5 (revision quality)
  Trust the lowest score from two passes, not the highest.

DONE SIGNAL:
  Calibrated score >= 7.5 AND your reader types do not
  quit before the end. Not perfect. Done.
```

---

## Next Step: Choose Your Flavor Card

When your 4 starter documents exist, open the matching flavor card:

| Your project | Card |
|---|---|
| Guide, handbook, pamphlet (<=40K) | [`short.md`](short.md) |
| Non-fiction, business book (50-80K) | [`topic.md`](topic.md) |
| Fiction, narrative non-fiction (80K+) | [`novel.md`](novel.md) |

The flavor card gives you the full world model doc list, generation setup,
session protocol, verification layers, and quality gates for your scope.

---

## Worked Examples

Before building your own docs, compare what a completed starter set looks like:

| Flavor | Example location | What to compare to your Doc 01 |
|---|---|---|
| Short | [`../docs/01_book_concept.md`](../docs/01_book_concept.md) | Concept clarity + scope boundary |
| Topic | [`../topic-example/01_book_concept.md`](../topic-example/01_book_concept.md) | Argument structure + evidence basis |
| Novel | [`../novel-example/01_premise.md`](../novel-example/01_premise.md) | Logline + comparable titles |

Differences between your doc and the example are expected — these are different
projects. Look for: structure match, scope clarity, reader specificity.

---

## Source

This card is an adaptation of the pre-flavor on-boarding card from
*Agentic Book Writing: The Smart Way* by Roble Mumin (roblemumin.com).
If this card and the book diverge, the book takes precedence.
