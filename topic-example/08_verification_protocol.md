<!--
Book reference: This example supports Lab 8 (Chapter 7: Verification Documents — protocol).
If you completed Lab 8, compare your verification protocol to this example.
Differences are expected. Look for: the 8-layer structure (vs Short-flavor's 3 layers),
the integration of CFR with verification, and the prose quality gate layer.
-->

# Verification Protocol — Sourdough at Home

**Project:** Sourdough at Home: A Practical Guide to Wild Yeast Baking
**Flavor:** Topic (55,000–65,000 words)
**Verification depth:** 8-layer full QVP (vs. 3-layer lite for Short-flavor)

> **Note for agent:** Run this protocol in the sequence listed. Each layer catches
> errors that earlier layers may not surface. Do not skip layers even if the manuscript
> "feels" correct.

---

## When to Run This Protocol

Run a complete 8-layer verification pass:
- After completing the first full draft (before any reader testing)
- After any revision pass that changed 3 or more chapters
- Before any publication or distribution (final gate)

Run targeted verification (layers 1–3 only) after single-chapter edits.

---

## Layer 1: CFR Audit (Claim Fact Registry)

**Purpose:** Ensure every technical claim in the manuscript matches the canonical
values in Doc 07 (Canon Rules).

**Method:**
1. Read Doc 07 fully (15 minutes)
2. Scan each chapter for numeric claims (temperatures, ratios, times, percentages)
3. Compare each claim to Doc 07 registry entry
4. Flag mismatches with the registry ID: `<!-- CFR MISMATCH: found [value], canon is [value], ID: P-004 -->`

**Common mismatches to check:**
- Bulk fermentation time stated as a single number instead of a range (e.g., "5 hours" vs "4–6 hours")
- Temperature stated in one unit only when protocol requires both F and C
- Hydration advice that narrows beyond canonical range
- Author statistics cited without "Level 3" context flag

**Completion criteria:** Zero unresolved CFR mismatches.

---

## Layer 2: Internal Consistency Check

**Purpose:** Verify that the same process, term, or recommendation is described
identically in every chapter where it appears.

**Method:**
1. Create a consistency checklist of terms and processes that appear in multiple chapters:
   - Bulk fermentation readiness: "50–75% volume increase" (appears in Ch 5, Ch 8, Ch 13)
   - Starter feeding ratio: "1:5:5" (appears in Ch 2, Ch 8, Appendix A)
   - Baking temperature: "475–500°F" (appears in Ch 7, recipes in Appendix B)
2. Verify that each is stated with the canonical value (not paraphrased differently)
3. Verify that the float test caveat appears every time float test is mentioned

**Completion criteria:** Consistent phrasing for all tracked terms across all chapters.

---

## Layer 3: Sequence Integrity Check

**Purpose:** Verify that concepts are introduced before they are referenced.
A reader should never encounter a term that requires a later chapter to understand.

**Method:**
1. List all terms from Doc 04 in the order they first appear in the manuscript
2. Verify that each term appears in the correct chapter order relative to its definition
3. Check cross-references ("See Chapter N") — verify the referenced chapter precedes the reference
   (or is clearly labeled as a forward reference with context provided)

**Common failures:**
- "Gluten development" referenced in Chapter 2 (starter) before it is defined in Chapter 4 (mixing)
- "CFR" acronym used in a chapter before the chapter that introduces it
- Troubleshooting concepts (Ch 13) referenced in process chapters without establishing they will be addressed later

**Completion criteria:** No undefined forward references in process text.

---

## Layer 4: Scope Discipline Check

**Purpose:** Verify that no chapter introduces content outside the scope guardrails
defined in Doc 01 (Book Concept).

**Scope guardrails to enforce:**
- No commercial yeast baking content in process chapters (brief orientation in Introduction only)
- No pastry or enriched dough techniques
- No milling, grain sourcing, or single-origin flour content
- No commercial-scale equipment or processes
- No advanced shaping beyond the three approved shapes (boule, batard, fougasse)

**Method:** Scan each chapter for scope creep. Flag any content outside these limits.

**Completion criteria:** Zero out-of-scope content.

---

## Layer 5: Reader Archetype Alignment Check

**Purpose:** Verify that each chapter serves the declared primary reader from Doc 03
(Book Architecture) and does not leave other archetypes behind unnecessarily.

**Method:** For each chapter, read with each archetype in mind:
- Does the New Baker have sufficient orientation for this chapter?
- Does the Transitioning Baker get credit for prior knowledge without being talked down to?
- Does the Troubleshooter receive a diagnostic angle or at least a "What went wrong?" section?
- Does the Fermentation Curious receive at least one Science Note callout?

**Completion criteria:** Each chapter provides at least one explicit entry point for each archetype.

---

## Layer 6: Prose Quality Gate

**Purpose:** Verify that no chapter falls below the minimum quality threshold.

**Scoring method:** Apply the Topic-flavor quality rubric (12 dimensions, Doc 06 calibration):
- Calibrated score (raw × 0.85) ≥ 7.0 = pass
- Calibrated score 6.5–7.0 = conditional pass (flag for targeted revision)
- Calibrated score < 6.5 = revision required before proceeding

**Dimensions to check (abbreviated):**
1. Clarity: Is the writing clear without prior knowledge?
2. Accuracy: Do all technical claims match Doc 07?
3. Completeness: Is the chapter's declared intent fully executed?
4. Voice consistency: Does this chapter sound like the same author as Chapter 1?
5. Jargon compliance: Are all new terms defined on first use?
6. Structure: Does the chapter follow the opening format and section heading conventions?
7. Callout box usage: Are boxes used correctly (Tip/Warning/Science Note/Troubleshooting)?
8. Process step formatting: Are ordered steps using ordered lists (not paragraphs)?
9. Numeric precision: Are all ranges correct per Doc 07?
10. Reader archetype coverage: Are all four archetypes served?
11. Troubleshooting section: Is the "What went wrong?" section present and specific?
12. Chapter opening hook: Does the chapter open with a recognizable baking moment?

**Completion criteria:** All 14 chapters score ≥ 7.0 calibrated.

---

## Layer 7: Cross-Reference Audit

**Purpose:** Verify that all "See Chapter N" references are valid and accurate.

**Method:**
1. List all cross-references in the manuscript
2. Verify that the referenced chapter exists and contains the content described
3. Verify that the reference directs the reader to a preceding chapter (not a future one,
   unless explicitly labeled as a forward pointer)

**Completion criteria:** Zero broken or inaccurate cross-references.

---

## Layer 8: Pre-Publication Checklist

**Purpose:** Final verification before distribution. Non-content checks.

- [ ] Front matter complete (title page, copyright, table of contents)
- [ ] Author bio accurate (credentials match Doc 05)
- [ ] All recipes in Appendix B tested and confirmed (bake log documentation)
- [ ] Starter log template in Appendix A is fillable (dates, measurements, columns correct)
- [ ] Chapter numbers in table of contents match manuscript
- [ ] All callout boxes display correctly in both PDF and EPUB outputs
- [ ] No placeholder text remaining (`[NAME]`, `[TBD]`, `[INSERT EXAMPLE HERE]`)
- [ ] ISBN/copyright year/edition noted (if publishing)
- [ ] Running head text consistent across chapters

**Completion criteria:** All 9 items checked.

---

## Verification Log Format

Record each verification pass:

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

*Doc Version: 1.0 | Flavor: Topic | Phase: 1 (Complete)*
