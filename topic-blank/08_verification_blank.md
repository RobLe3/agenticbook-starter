<!--
Book reference: Lab 8 (Chapter 7: Verification Documents — protocol).
Fill in this template to create your 8-layer verification protocol.
Compare to topic-example/08_verification_protocol.md for structure guidance.
KEY DISTINCTION: Short-flavor has 3 verification layers. Topic-flavor requires 8.
The additional layers address: reader archetype alignment, prose quality gating,
cross-reference auditing, and pre-publication checklisting.
-->

# Verification Protocol — [YOUR_PROJECT_TITLE]

**Project:** [YOUR_FULL_PROJECT_TITLE_AND_SUBTITLE]
**Flavor:** Topic ([WORD_COUNT_LOW]–[WORD_COUNT_HIGH] words)
**Verification depth:** 8-layer full QVP

> **Note for agent:** Run layers in sequence. Each layer catches errors earlier layers
> may not surface. Do not skip layers.

---

## When to Run This Protocol

- After completing the first full draft (before reader testing)
- After any revision pass that changed 3 or more chapters
- Before any publication or distribution (final gate)

Run targeted verification (layers 1–3 only) after single-chapter edits.

---

## Layer 1: CFR Audit (Claim Fact Registry)

**Purpose:** Ensure every technical claim matches the canonical values in Doc 07.

**Method:**
1. Read Doc 07 fully
2. Scan each chapter for numeric claims (measurements, ratios, times, percentages)
3. Compare each claim to Doc 07 registry
4. Flag mismatches: `<!-- CFR MISMATCH: found [value], canon is [value], ID: [ID] -->`

**Common mismatches in [YOUR_SUBJECT]:**
- [SPECIFIC_MISMATCH_TYPE_1 — describe a typical error for your subject]
- [SPECIFIC_MISMATCH_TYPE_2]
- [SPECIFIC_MISMATCH_TYPE_3]

**Completion criteria:** Zero unresolved CFR mismatches.

---

## Layer 2: Internal Consistency Check

**Purpose:** Verify the same process, term, or recommendation is described identically
everywhere it appears.

**Method:**
1. Create a consistency checklist of [5–8 terms/processes that appear in multiple chapters]:
   - [TERM_OR_PROCESS_1] — appears in [Ch N, Ch M, Ch P]
   - [TERM_OR_PROCESS_2] — appears in [Ch N, Ch M]
   - [TERM_OR_PROCESS_3] — appears in [Ch N, Appendix A]
2. Verify identical canonical phrasing at each appearance

**Completion criteria:** Consistent phrasing for all tracked terms.

---

## Layer 3: Sequence Integrity Check

**Purpose:** Verify concepts are introduced before they are referenced.

**Method:**
1. List all terms from Doc 04 in manuscript appearance order
2. Verify each term appears in correct chapter order relative to its definition
3. Check cross-references — verify referenced chapter precedes the reference

**Common failures in [YOUR_SUBJECT]:**
- [DESCRIBE A SPECIFIC SEQUENCING FAILURE COMMON IN YOUR DOMAIN]

**Completion criteria:** No undefined forward references in process text.

---

## Layer 4: Scope Discipline Check

**Purpose:** Verify no chapter introduces content outside the scope guardrails in Doc 01.

**Scope guardrails to enforce:**
- [OUT_OF_SCOPE_ITEM_1 from Doc 01]
- [OUT_OF_SCOPE_ITEM_2]
- [OUT_OF_SCOPE_ITEM_3]
- [OUT_OF_SCOPE_ITEM_4]

**Completion criteria:** Zero out-of-scope content.

---

## Layer 5: Reader Archetype Alignment Check

**Purpose:** Verify each chapter serves its declared primary reader from Doc 03.

**Method:** For each chapter, read with each archetype in mind:
- Does [ARCHETYPE_1] have sufficient orientation?
- Does [ARCHETYPE_2] get credit for prior knowledge?
- Does [ARCHETYPE_3] receive a diagnostic angle?
- Does [ARCHETYPE_4 (if applicable)] receive their specific content type?

**Completion criteria:** Each chapter provides at least one explicit entry point per archetype.

---

## Layer 6: Prose Quality Gate

**Purpose:** Verify no chapter falls below the minimum quality threshold.

**Method:** Apply calibrated scoring (raw × 0.85) using your 12-dimension rubric.
- ≥ 7.0 calibrated = pass
- 6.5–7.0 = conditional pass (flag for targeted revision)
- < 6.5 = revision required

**Dimensions to check:**
1. Clarity (accessible without prior knowledge)
2. Accuracy (all claims match Doc 07)
3. Completeness (chapter intent fully executed)
4. Voice consistency (same author voice throughout)
5. Jargon compliance (all new terms defined on first use)
6. Structure (opens correctly, sections follow conventions from Doc 06)
7. [YOUR_CALLOUT_BOX_TYPE] usage (used correctly per Doc 06 policy)
8. [PROCESS_FORMAT] formatting (ordered steps formatted as lists, not paragraphs)
9. Numeric precision (all ranges correct per Doc 07)
10. Reader archetype coverage (all archetypes served per Doc 02)
11. [CHAPTER-END_ELEMENT — e.g., troubleshooting section, summary, or Lab] present
12. Chapter opening hook (opens with appropriate hook per Doc 06 §Chapter Opening Format)

**Completion criteria:** All chapters score ≥ 7.0 calibrated.

---

## Layer 7: Cross-Reference Audit

**Purpose:** Verify all "See Chapter N" references are valid and accurate.

**Method:**
1. List all cross-references in the manuscript
2. Verify referenced chapter contains the described content
3. Verify reference directs to a preceding chapter (or is labeled as forward pointer)

**Completion criteria:** Zero broken or inaccurate cross-references.

---

## Layer 8: Pre-Publication Checklist

- [ ] Front matter complete (title page, copyright, table of contents)
- [ ] Author bio accurate (credentials match Doc 05)
- [ ] All [APPENDIX_CONTENT — e.g., recipes, templates, checklists] verified
- [ ] Chapter numbers in table of contents match manuscript
- [ ] All callout boxes display correctly in both PDF and EPUB
- [ ] No placeholder text remaining
- [ ] [YOUR_PROJECT_SPECIFIC_CHECK_1]
- [ ] [YOUR_PROJECT_SPECIFIC_CHECK_2]
- [ ] ISBN/copyright year/edition noted (if publishing)

**Completion criteria:** All checklist items complete.

---

## Verification Log Format

```
Pass N — [date]
Scope: [full / targeted / targeted Ch N]
Layers completed: [list]
Issues found: [count per layer]
Issues resolved: [count]
Remaining: [count + brief description]
Calibrated score range: [low–high across chapters]
```

---

*Doc Version: 1.0 | Flavor: Topic | Phase: 1 (Pending)*
