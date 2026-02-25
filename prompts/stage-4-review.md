# Stage 4: Review

> Prompts: **AASS** (Quality Scoring) | **DARE** (Targeted Dimension Review) | **IRIN** (Integrated Review Inline) | Reader Simulation panels
>
> **Calibration warning:** Apply **×0.80** to all AASS scores (not ×0.85). Static-prompt
> self-assessment inflates by ~20% without a world model anchoring the assessment.
> Apply **×0.85** to world-model-grounded scoring passes.
> Never treat a single scoring pass as a final quality determination.
>
> **DO_DONT circuit breaker:** Run the DO_DONT check before starting another revision pass.
> Don't iterate because the system allows it. Do stop when scores plateau across 2 passes.

---

## AASS — Accessibility and Structural Scoring

**Use when:** After drafting a chapter. Holistic quality review across 8 dimensions.

```
Score this chapter against the following 8 dimensions.

Chapter:
[PASTE CHAPTER TEXT]

Dimensions (score each 1-10):
1. Clarity: Is the core message clear throughout?
2. Coherence: Do sections connect logically?
3. Voice consistency: Does the register hold start to end?
4. Specificity: Are claims supported with specific detail
   rather than generalities?
5. Reader value: What does the reader gain? Is it stated?
6. Completeness: Does the chapter fulfill its stated intent?
7. Concision: Is every section earning its word count?
8. Transition quality: Do sections connect without abrupt jumps?

For each dimension: [Score] / [Evidence] / [Biggest weakness]

Raw weighted average: [X.X]
Apply ×0.80 calibration to this score before use.

Top 3 strengths:
Top 3 weaknesses (priority order for revision):
```

---

## DARE — Detailed Area Review

**Use when:** After AASS identifies weak dimensions. Targeted deep-dive on one dimension at a time.

DARE generates specific, actionable revision notes at the paragraph level.

```
Review this chapter specifically for [DIMENSION NAME].

Chapter:
[PASTE CHAPTER TEXT]

Focus entirely on [DIMENSION]. For every paragraph:
- Is this paragraph strong, adequate, or weak on [DIMENSION]?
- For weak paragraphs: what exactly is wrong and what is
  the minimum fix?

Output format:
[Para #] [STRONG/ADEQUATE/WEAK] — [Specific issue] — [Fix]

Summary: top 3 paragraphs to revise, in priority order.
```

---

## IRIN — Integrated Review Inline

**Use when:** After a revision pass — to verify the revision worked without re-running the full AASS.

IRIN scans for the specific issues DARE identified and confirms they are resolved.

```
Verify these specific issues have been resolved in the
revised chapter.

Issues from previous review:
1. [Location] — [Original issue]
2. [Location] — [Original issue]
3. [Location] — [Original issue]

[PASTE REVISED CHAPTER TEXT]

For each issue:
- RESOLVED: [what changed and how it fixes the problem]
- PARTIAL: [what improved but is not yet resolved]
- UNRESOLVED: [why the revision did not fix it]

> Note for agent: After generating IRIN output, parse
> [COMMENT: ...] tags in the revised text and address each
> one before marking the review complete.

New issues introduced by the revision (if any):
[List any regressions or new problems the revision created]
```

---

## Reader Simulation

**Use when:** After at least 3 chapters are drafted. Run 2 archetypes (Short flavor) or 3 archetypes (Topic flavor).

Use the archetype profiles from your flavor card (`quickstart/short.md` etc.) as the reader specification.

```
Simulate the reading experience for this archetype:

Archetype: [NAME — e.g., "The Practitioner: experienced
but new to this specific topic; reads to use, not to learn
for its own sake; values actionability over theory"]

DO NOT: invent reader reactions based on demographics not
in the archetype specification above.
DO NOT: assume the reader has read chapters not mentioned below.
DO: evaluate only based on the chapter text provided.

Chapters read so far: [Ch 1 summary] / [Ch 2 summary] / ...

Chapter to evaluate:
[PASTE CHAPTER TEXT]

Questions to answer from this archetype's perspective:
1. After this chapter, what can I do that I could not before?
2. What confused me? (specific passages, not vague "clarity")
3. What would make me stop reading here and not continue?
4. Signal: [CONTINUE / FLAGGED / WOULD_STOP]

If FLAGGED or WOULD_STOP: what is the minimum fix to convert?
```
