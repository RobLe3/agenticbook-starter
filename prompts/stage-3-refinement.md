# Stage 3: Refinement

> Prompts: **COREF** (Consistency Reference Check) | **STRAL** (Style Alignment) | **COMAC** (Comprehension and Accessibility Check) | **CAM** (Chapter Arc Map)
>
> Run Stage 3 prompts after 3+ chapters are drafted. They check consistency and coherence
> across chapters — critical once multiple chapters must agree about facts, terms, and voice.
>
> **DO_DONT circuit breaker (run before starting):**
> Don't iterate because the system allows it. Don't chase micro-gains. Do stop when reader
> models converge. Do notice boredom or resistance.

---

## COREF — Consistency Reference Check

**Use when:** Every 3 chapters — before drift compounds. Run against your accumulated keyword matrix and fact list.

```
Check this chapter for consistency with my reference material.

=== KEYWORD MATRIX ===
[PASTE your current keyword matrix — all terms and definitions]

=== KEY FACTS (must not change) ===
[PASTE your fact list — 5-10 key claims that must
stay consistent across all chapters]

=== CHAPTER TO CHECK ===
[PASTE chapter text]

Check for:
1. KEY TERM USE: any term used inconsistently with the
   matrix definition?
2. FACT CONSISTENCY: any claim that contradicts the
   fact list?
3. NEW TERMS: any term introduced here that should be
   added to the matrix?
4. VOICE DRIFT: any paragraph that breaks from the
   established voice?

Report each finding: [Location] / [Issue] / [Fix]
```

**World model equivalent:** COREF is the manual equivalent of the CFR protocol (Chapter 7) and the consistency layer of the QVP sweep. With a world model, the CFR registry is permanent and the check runs against an external file — not re-stated inline every time.

---

## STRAL — Style Alignment

**Use when:** After every 4–5 chapters. Voice audit across chapter extracts.

STRAL identifies where the voice has drifted from your established register.

```
Audit these chapter extracts for voice consistency.

Target voice (from my style guide):
"[PASTE 2-3 sentences that represent your exact target
voice and register]"

Extract 1 (Chapter [N], first 300 words):
[PASTE]

Extract 2 (Chapter [N+2], first 300 words):
[PASTE]

Extract 3 (Chapter [N+4], first 300 words):
[PASTE]

For each extract:
1. VOICE MATCH: does it match the target? (YES / PARTIAL / NO)
2. SPECIFIC DRIFT: what exactly is different? (sentence
   length, register, person, vocabulary level)
3. WORST OFFENDER: the single paragraph most at odds
   with the target voice
4. FIX: how to bring it back in line

Priority order for revision: [1] / [2] / [3]
```

---

## COMAC — Comprehension and Accessibility Check

**Use when:** After generation, before revision. Read from the target reader's perspective.

COMAC flags passages where the reader will lose the thread, concepts that need more scaffolding, and jargon that lands before it has been defined.

```
Audit this chapter for comprehension and accessibility.

Target reader: [WHO — 1 sentence, specific knowledge level]

Chapter to audit:
[PASTE CHAPTER TEXT]

Check for:
1. DEFINITION GAPS: technical terms used before they are
   defined, or defined without adequate context
2. LOGIC GAPS: arguments where a step is missing — reader
   is expected to make a leap that isn't supported
3. PACING PROBLEMS: sections where too much information
   arrives without consolidation
4. ASSUMPTION MISMATCHES: where the chapter assumes the
   reader knows something they likely do not
5. UNCLEAR ANTECEDENTS: "this," "it," "that approach"
   with no clear referent

For each: [Location] / [Problem] / [Fix in 1 sentence]
```

---

## CAM — Chapter Arc Map

**Use when:** After every 5 chapters. Cross-chapter coherence check.

CAM verifies the book is building its argument in a logical sequence. Run it on the chapter titles and one-sentence summaries — not the full text.

```
Check the coherence of this chapter sequence:

Book premise: [1-2 sentences]
Target reader: [1 sentence]

Chapter sequence:
Ch 1: "[Title]" — [1-sentence summary]
Ch 2: "[Title]" — [1-sentence summary]
[... all chapters drafted so far ...]

Check for:
1. ARGUMENT FLOW: does each chapter build on the previous?
2. MISSING STEPS: is there a conceptual jump the reader
   cannot make without a missing chapter?
3. DUPLICATE EFFORT: do any two chapters cover the same
   ground without additive value?
4. ANTICLIMAX: does the sequence end with decreasing
   importance rather than building to the book's payoff?
5. READER STATE: at the end of each chapter, what can
   the reader now do that they could not before?

Verdict: [COHERENT / NEEDS RESTRUCTURE]
Priority fixes: [1] / [2] / [3]
```

**World model equivalent:** CAM does manually what the narrative architecture document (Doc 03) enforces structurally. With a world model, the chapter structure is embedded in every generation prompt — it does not drift to the extent that a post-hoc CAM audit is necessary.
