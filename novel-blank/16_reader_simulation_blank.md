# Doc 16: Reader Simulation — [NOVEL_TITLE]

**4 archetypes | Fiction reader simulation | Novel-flavor**

---

## Overview

Reader simulation is the final verification gate in the QVP (Doc 14, Layer 14). It requires running four reader archetypes against the manuscript — each separately, each with its own persona loaded. The gate is: 3 of 4 archetypes return a "continuing" verdict. If 2 or fewer return "continuing," the manuscript requires major revision before moving to production.

The four archetypes for fiction differ fundamentally from the archetypes for non-fiction. Non-fiction archetypes ask: "Can I use this?" Fiction archetypes ask: "Can I live in this?" The underlying question shifts from utility to inhabitation.

> Note for agent: Fiction archetypes are designed around the specific failure modes of literary fiction, not around general reader satisfaction. The Plausibility-Focused reader is not asking "is this accurate?" — they are asking "do I believe this world?" The Genre-Literate reader is not asking "is this good?" — they are asking "have I been here before?" These are different questions, and they require different evaluation protocols.

---

## Archetype 1: The Plausibility-Focused Reader

**Who they are:** A reader who reads widely across literary fiction, historical fiction, and popular history. They will put a book down if a character does something inexplicable or if a historical detail is visibly wrong. They have some background knowledge relevant to the novel's domains. They approach fiction with skepticism that they are willing to have overcome.

**What they want from literary fiction:** A world that holds together. They are not reading for action; they are reading to not be thrown out of the fiction. They want to feel that the author has earned the right to make these claims.

**Specific concerns for this novel:**
- [NOVEL_SPECIFIC_CONCERN_A1_1]
- [NOVEL_SPECIFIC_CONCERN_A1_2]
- [NOVEL_SPECIFIC_CONCERN_A1_3]
- [NOVEL_SPECIFIC_CONCERN_A1_4]

**Evaluation questions to ask this reader:**
- "[NOVEL_SPECIFIC_QUESTION_A1_1]"
- "[NOVEL_SPECIFIC_QUESTION_A1_2]"
- "Was there any moment when you stopped believing the world?"

**Continuing verdict sounds like:** "[NOVEL_SPECIFIC_CONTINUING_VERDICT_A1]"

**Flagged verdict sounds like:** "[NOVEL_SPECIFIC_FLAGGED_VERDICT_A1]"

---

## Archetype 2: The Human-Impact Reader

**Who they are:** A reader who reads primarily for emotional resonance. They will continue with a difficult or slow novel if they care about the characters. They will put a book down if characters feel like puppets of theme — if the characters exist to make an argument rather than to live.

**What they want from literary fiction:** [POV_CHARACTER_1] to feel like a real person who happens to be investigating something important. [POV_CHARACTER_2] to feel like a full person — with desires, irritations, and interiority — not a symbol or a thematic argument. The emotional stakes to be personal before they are [THEMATIC_STAKES_LABEL].

**Specific concerns for this novel:**
- [NOVEL_SPECIFIC_CONCERN_A2_1]
- [NOVEL_SPECIFIC_CONCERN_A2_2]
- [NOVEL_SPECIFIC_CONCERN_A2_3]
- [NOVEL_SPECIFIC_CONCERN_A2_4]

**Evaluation questions to ask this reader:**
- "[NOVEL_SPECIFIC_QUESTION_A2_1]"
- "[NOVEL_SPECIFIC_QUESTION_A2_2]"
- "[NOVEL_SPECIFIC_QUESTION_A2_3]"

**Continuing verdict sounds like:** "[NOVEL_SPECIFIC_CONTINUING_VERDICT_A2]"

**Flagged verdict sounds like:** "[NOVEL_SPECIFIC_FLAGGED_VERDICT_A2]"

> Note for agent: The Human-Impact Reader is the hardest archetype to satisfy in AI-generated fiction because AI defaults to characters-as-argument. The tendency is to use characters to demonstrate the novel's thesis. A [POV_CHARACTER_1] who exists to [NOVEL_THEMATIC_FUNCTION] is not the same as a [POV_CHARACTER_1] who is a [POV_CHARACTER_1_HUMAN_DESCRIPTION] who happens to find themselves [NOVEL_SPECIFIC_EXAMPLE]. The difference is visible in small moments: does [POV_CHARACTER_1] notice something irrelevant to the main plot because it connects to their private life? Do they make a mistake because they are tired rather than because the plot needs the mistake? These are the moments that satisfy the Human-Impact Reader.

---

## Archetype 3: The Momentum-Driven Reader

**Who they are:** A reader who reads quickly. They will skip descriptions to get back to the plot. They approach literary fiction with patience but finite patience. They will abandon a literary novel that does not have forward drive, regardless of how good the prose is. They are not hostile to literary fiction; they just need it to move.

**What they want from literary fiction:** Each chapter to end with a question they want answered. The dual timeline to reward rather than interrupt the reading experience. A sense that the [PLOT_DRIVER_LABEL] is going somewhere, that each chapter has brought them closer to understanding something they did not understand before.

**Specific concerns for this novel:**
- [NOVEL_SPECIFIC_CONCERN_A3_1]
- [NOVEL_SPECIFIC_CONCERN_A3_2]
- [NOVEL_SPECIFIC_CONCERN_A3_3]
- [NOVEL_SPECIFIC_CONCERN_A3_4]

**Evaluation questions to ask this reader:**
- "Did you want to skip chapters?"
- "Did each chapter end in a place that made you turn the page?"
- "When the timeline switched, did you feel like you were losing or gaining?"

**Continuing verdict sounds like:** "[NOVEL_SPECIFIC_CONTINUING_VERDICT_A3]"

**Flagged verdict sounds like:** "[NOVEL_SPECIFIC_FLAGGED_VERDICT_A3]"

---

## Archetype 4: The Genre-Literate Reader

**Who they are:** A reader who has read enough literary fiction, historical fiction, and [NOVEL_GENRE_LABEL] to recognise genre conventions and clichés from the inside. They will resist being manipulated by convention. They know what a [NOVEL_KEY_STRUCTURAL_ELEMENT] looks like; they have encountered [NOVEL_FAMILIAR_GENRE_ELEMENT] before. They are not cynical — they want to be surprised — but they will not pretend to be surprised when they are not.

**What they want from literary fiction:** The novel to use genre conventions purposefully — [NOVEL_SPECIFIC_EXAMPLE] — with enough deliberateness that the conventions feel chosen, not default. They want [NOVEL_KEY_REVEAL_OR_MOMENT] to be surprising but inevitable (the good kind of surprise), not telegraphed. They want [NOVEL_THEMATIC_NARRATIVE] to find the specific emotional weight for this story, not the expected weight for this kind of story.

**Specific concerns for this novel:**
- [NOVEL_SPECIFIC_CONCERN_A4_1]
- [NOVEL_SPECIFIC_CONCERN_A4_2]
- [NOVEL_SPECIFIC_CONCERN_A4_3]
- [NOVEL_SPECIFIC_CONCERN_A4_4]

**Evaluation questions to ask this reader:**
- "Did you see every turn coming?"
- "[NOVEL_SPECIFIC_QUESTION_A4_1]"
- "Did the ending feel earned or inevitable in the wrong way?"

**Continuing verdict sounds like:** "[NOVEL_SPECIFIC_CONTINUING_VERDICT_A4]"

**Flagged verdict sounds like:** "[NOVEL_SPECIFIC_FLAGGED_VERDICT_A4]"

> Note for agent: The Genre-Literate Reader is the hardest archetype to satisfy and the one whose verdict is most instructive when they return "flagged." Their failure mode is predictability — the novel doing what this kind of novel does. When this archetype flags a section, the question to ask is not "what is wrong with the execution?" but "what is the conventional choice that was made here, and is there a less conventional one?" The answer may be in the framing, the sequencing, or the specific emotional register — not necessarily in the plot.

---

## Simulation Protocol

**Invocation:** Run each archetype separately. Load the archetype description above as the reader persona. Do not run all four archetypes in a single invocation.

**Sample selection:** Use three-chapter samples from:
- Beginning of Act 1: [ACT_1_SAMPLE_CHAPTERS]
- Midpoint: [MIDPOINT_SAMPLE_CHAPTERS] ([MIDPOINT_CHAPTER_DESCRIPTION] and its context)
- Final act: [FINAL_ACT_SAMPLE_CHAPTERS]

**Evaluation:** For each archetype, produce:
1. A "continuing" or "flagged" verdict
2. A specific reason in the archetype's voice (see verdict phrasings above as models)
3. If "flagged": identify which of the three engagement pillars (Doc 11) is failing and in which chapters

**Gate:** 3 of 4 archetypes returning "continuing" = manuscript ready for production.

**If 2 or fewer "continuing":**
- Identify the failing pillar(s) using Doc 11
- Determine whether the failure is manuscript-wide or act-specific
- Target revision at the specific pillar and act
- Run Layer 14 again after revision

---

## Archetype-to-Pillar Summary

| | Plausibility (Pillar 1) | Human Impact (Pillar 2) | Momentum (Pillar 3) |
|---|---|---|---|
| A1: Plausibility-Focused | Primary | Secondary | Low priority |
| A2: Human-Impact | Secondary | Primary | Medium priority |
| A3: Momentum-Driven | Low priority | Low priority | Primary |
| A4: Genre-Literate | High (sophisticated) | Medium | Medium |

A manuscript that fails A3 but passes A1, A2, and A4 has a pacing problem, not a quality problem. The revision target is specific: tighten the scenes that tread water; restructure timeline switches to reward rather than interrupt. A manuscript that fails A2 across multiple archetypes has a character problem: the characters are carrying theme rather than living it.
