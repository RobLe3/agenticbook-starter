# Stage 2: Writing

> Prompts: **CHDD** (Chapter Detail Definition) | **CHFO** (Chapter From Outline) | **SUBREF** (Subject Reference Generator)
>
> CHFO is the core generation engine. Run CHDD before CHFO for complex chapters.
> SUBREF generates structured reference material for technically dense chapters.
>
> **World model equivalent:** CHFO is what Template 10 (Generation Prompt) does when you have
> a world model. With a world model, the style guide and entity data live in external files pasted
> once per session. CHFO re-states that information inline every chapter — by Chapter 5, you
> will feel the difference.

---

## CHDD — Chapter Detail Definition

**Use when:** Before CHFO, for chapters with complex or multi-section structure. Optional for simpler chapters.

CHDD produces a detailed brief — section by section — that CHFO then executes into prose.

```
Define the detailed structure for this chapter:

Book: [TITLE]
Chapter [N]: "[CHAPTER TITLE]"
Chapter intent: [WHAT THIS CHAPTER ACCOMPLISHES — 1 sentence]
Target words: [X,000]
Follows: [Chapter N-1 title and 1-sentence summary]
Leads to: [Chapter N+1 title]

Key terms for this chapter (from your keyword matrix):
- [Term 1]: [definition]
- [Term 2]: [definition]

Generate:
1. OPENING (150-200 words): hook approach — question /
   scenario / statistic / problem statement
2. SECTIONS (3-5): [Section title] — [intent] — [key points]
3. EXAMPLES TO INCLUDE: 2-3 concrete examples or case
   studies with specific details, not generic descriptions
4. TRANSITIONS: how each section connects to the next
5. CLOSING (100-150 words): summary approach + bridge
   to next chapter
```

---

## CHFO — Chapter From Outline

**Use when:** Generating chapter prose. This is the core generation prompt. Re-paste the Keyword Matrix and voice sample for every chapter.

```
Write Chapter [N] of my book.

=== BOOK CONTEXT ===
Title: [YOUR TITLE]
Premise: [2 sentences]
Target reader: [1 sentence]
Chapter [N] of [TOTAL]

=== VOICE & STYLE ===
Style: [CONVERSATIONAL / PROFESSIONAL / TECHNICAL]
Person: [Second — "you"]
Avoid: [LIST 2-3 specific phrases or patterns]
Voice sample: "[PASTE 2-3 sentences in exact target voice]"

=== KEYWORD MATRIX ===
[Term 1]: [1-sentence definition]
[Term 2]: [1-sentence definition]
[... 5-8 terms — paste full matrix every chapter ...]

Key facts that MUST stay consistent:
- [Fact 1]   - [Fact 2]   - [Fact 3]

=== THIS CHAPTER ===
Title: "[CHAPTER TITLE]"     Target: [X,000] words
Intent: [what reader knows or can do after reading]
Structure: [paste CHDD output, or list 4-5 key points]
Previous chapter: [2-3 sentence summary]
Next chapter: [1 sentence preview]

=== REQUIREMENTS ===
1. Open with: [hook type from CHDD]
2. Cover key points in order with transitions
3. Match voice sample exactly — do not drift
4. Use key terms with the definitions above
5. End with summary + bridge to next chapter
6. Target [X,000] words (±20% for first draft)
```

---

## SUBREF — Subject Reference Generator

**Use when:** Before CHFO for chapters with high factual density. SUBREF generates structured reference material — definitions, relationships, key facts — that CHFO then weaves into prose.

```
Generate structured reference material for this chapter:

Topic: [CHAPTER TOPIC]
Audience level: [BEGINNER / INTERMEDIATE / EXPERT]
Chapter intent: [what reader should understand after reading]

Provide:
1. CORE CONCEPTS: 5-8 concepts with 2-sentence definitions
2. KEY RELATIONSHIPS: how the concepts connect or depend
   on each other
3. COMMON MISCONCEPTIONS: 3-5 things readers typically
   get wrong about this topic
4. CONCRETE EXAMPLES: 4-6 specific, verifiable examples
   — not "a company like X" but named, real instances
5. CLAIMS REQUIRING CITATION: flag any claim that needs
   a source before publication

Format for easy embedding in CHFO.
```

**World model equivalent:** SUBREF maps to Doc 05 (Source Inventory / Case Study) — in the world model, reference material is built once and retrieved by reference rather than re-generated per chapter.
