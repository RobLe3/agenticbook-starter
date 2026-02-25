# Stage 1: Concept Development

> Prompts: **STRUO** (Concept Development) | **ANALY** (Domain Analysis) | **COMPR** (Concept Stress-Test)
>
> Run these before writing any chapter prose. STRUO builds your book concept.
> ANALY sharpens positioning. COMPR stress-tests the concept before you invest in prose.
>
> **World model equivalent:** Stage 1 output maps to Doc 01 (Book Concept), Doc 03 (Architecture),
> Doc 04 (Key Concepts / Glossary), and Doc 08 (Style Guide). When you transition to the agentic
> methodology, use the STRUO output as your source material for those four documents.

---

## STRUO — Structured Thought/Reasoning/Utility/Output

**Use when:** Building your book concept from scratch. Run this first.

STRUO builds your book's concept from a premise. Give it your core idea and target reader; it returns a structured concept outline with title options, positioning, chapter structure, key terms, and a voice sample. This output is the foundation every subsequent Stage 2–6 prompt draws from.

```
You are helping me develop a book concept.

Core idea: [YOUR IDEA IN 1-2 SENTENCES]
Target reader: [WHO READS THIS AND WHY]
Format: [non-fiction / fiction / guide / memoir]
Approximate length: [SHORT 20-40K / TOPIC 50-80K / NOVEL 80K+]

Generate a structured book concept including:
1. WORKING TITLE: 3-5 options with rationale
2. CORE PREMISE: 2 sentences — what the book argues or shows
3. TARGET READER PROFILE: specific, not demographic — who
   picks this up, what problem do they have, what changes
   for them after reading
4. CHAPTER STRUCTURE: 6-12 chapter titles with 1-sentence
   intent per chapter
5. VALUE PROPOSITION: why this book, why now, what exists
   that this improves on
6. KEY TERMS: 8-12 terms central to this book, with
   1-sentence definitions each — these anchor all future prompts
7. VOICE: 2-3 sample sentences demonstrating the exact
   register for this book
```

---

## ANALY — Domain Analysis

**Use when:** After STRUO — to sharpen the value proposition and identify comparable titles.

ANALY runs a structured analysis of your topic domain: what exists in the publishing space, what angles are underserved, where your book fits.

```
Analyze the publishing landscape for this book:

Book concept: [PASTE STRUO output, or summarize in
              5-6 sentences]

Provide:
1. EXISTING BOOKS: 5-7 comparable titles with brief
   descriptions — what they cover, what they miss
2. GAPS: what angles are underserved or absent
3. POSITIONING: where this book fits — not "better than
   X" but "for readers who want Y that X doesn't provide"
4. READER NEED: the specific frustration or gap the
   target reader has that existing books don't address
5. DIFFERENTIATION: 2-3 concrete differences between
   this book and the closest comparables

Flag any title or claim that may be speculative.
```

**World model equivalent:** ANALY output maps to Doc 01 (Book Concept) — specifically the positioning and comparable titles sections.

---

## COMPR — Concept Stress-Test

**Use when:** Before writing Chapter 1. Catch concept weaknesses at concept stage — not at revision stage.

```
Review this book concept and stress-test it:

[PASTE YOUR STRUO OUTPUT or full concept description]

Identify:
1. ARGUMENT GAPS: what the book claims but doesn't
   explain how to prove
2. READER ASSUMPTION PROBLEMS: what the target reader
   may not accept as given that the book assumes they do
3. MISSING EVIDENCE: claims that will need sources,
   examples, or data that aren't yet mentioned
4. SCOPE RISKS: where the book may over-promise or
   under-deliver relative to its stated scope
5. STRUCTURE PROBLEMS: chapters that duplicate effort,
   missing chapters, chapters that don't build on each other

For each issue: [Problem] / [Why it matters] / [Suggested fix]
```

**World model equivalent:** COMPR serves the same function as the world model audit pass (the Ralph Loop in Chapter 7's verification protocol).
