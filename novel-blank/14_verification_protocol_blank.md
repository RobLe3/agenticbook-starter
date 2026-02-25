# Doc 14: Verification Protocol (QVP) — [NOVEL_TITLE]

**14-Layer Quality Verification Protocol | Novel-flavor fiction**

---

## Overview

The Quality Verification Protocol (QVP) is a structured sequence of verification passes that must be run in the order given. Order matters: errors in early layers contaminate later layers if the sequence is skipped. A CFR violation that survives into the prose quality assessment (Layer 8) will cause the quality score to be based on prose that contains a foundational error — the score is therefore meaningless.

> Note for agent: The 14 layers are divided into two sweep structures. Layers 1–7 run per five-chapter batch — after every five chapters are drafted, run these seven layers before continuing. Layers 8–13 run per chapter — after each chapter is drafted and before it is marked as done. Layer 14 runs once, after all [CHAPTER_COUNT] chapters are complete. This structure prevents error accumulation and catches systemic problems before they propagate across the whole manuscript.

**Total layers:** 14 (vs. 8 for Topic-flavor — the 6 additional layers address fiction-specific failure modes: character consistency sweep, timeline rhyme check, free indirect discourse audit, pacing sweep, cross-reference audit, and dialogue integrity.)

---

## Sweep A: Per Five-Chapter Batch (Layers 1–7)

Run Layers 1–7 after every five chapters are drafted. Do not continue to the next five chapters until the batch has passed all seven layers.

---

### Layer 1: CFR Audit

**Run this first. A CFR violation stops the batch.**

Check all [TOTAL_ENTRY_COUNT] entries in Doc 13 (CFR) against the full text of the five chapters in the batch. Process the text in sections of approximately 3,000 words.

**Method:** For each CF entry, verify the fact is present where relevant and correct where stated. For each HC entry, verify the claim is accurate where it appears. Flag any discrepancy with the specific entry number (CF-xxx or HC-xxx).

**Flag format:** `CFR VIOLATION: [ENTRY_NUMBER] | Chapter [N] | [BRIEF_DESCRIPTION] | Fix before Layer 2.`

**Gate:** Any violation stops Layer 1. Fix all violations, then restart Layer 1 from the beginning of the batch.

> Note for agent: CFR audit runs first because character fact and historical claim errors contaminate every subsequent layer. A chapter that contains a wrong character fact will generate an incorrect character consistency assessment in Layer 2, an incorrect voice assessment in Layer 5, and an incorrect dialogue assessment in Layer 12. Fix the foundational fact first; then the dependent assessments are meaningful.

---

### Layer 2: Character Consistency Sweep

For each of the [CHARACTER_COUNT] characters who appear in the batch: verify that their psychology — specifically the wound, desire, and fear documented in Doc 06 — is visible in their scenes.

**Flag format:** `CHAR CONSISTENCY: [CHARACTER_NAME] | Chapter [N] | [PSYCHOLOGY_DIMENSION_ABSENT] | e.g., "[CHARACTER_NAME] acts without their established defense mechanism present in this scene."`

Check specifically:
- [POV_CHARACTER_1]: [POV_CHARACTER_1_CONSISTENCY_CHECK]
- [POV_CHARACTER_2]: [POV_CHARACTER_2_CONSISTENCY_CHECK]
- [CHARACTER_ANTAGONIST_1]: [CHARACTER_ANTAGONIST_1_CONSISTENCY_CHECK]
- [CHARACTER_SUPPORTING_1]: [CHARACTER_SUPPORTING_1_CONSISTENCY_CHECK]

---

### Layer 3: Chronological Integrity

Verify both timelines maintain correct internal chronology. No impossible time jumps. No events occurring in the wrong sequence.

**Reference timeline (maintain across all [CHAPTER_COUNT] chapters):**
- [TIMELINE_2_LABEL]: [TIMELINE_2_DURATION_AND_CONSTRAINTS]
- [TIMELINE_1_LABEL]: [TIMELINE_1_DURATION_AND_CONSTRAINTS]

**Method:** Create or update a scene-by-scene date log. For each chapter, record: Timeline ([TIMELINE_1_PERIOD] / [TIMELINE_2_PERIOD]), approximate date within that timeline, location, events. Verify no chapter places a character somewhere they could not yet be, or references an event that has not yet occurred.

**Flag format:** `CHRONOLOGY: Chapter [N] | [DESCRIPTION_OF_IMPOSSIBLE_OR_CONTRADICTORY_TIMING]`

---

### Layer 4: Domain Accuracy Check

Verify all [DOMAIN_1_LABEL] procedures against the fixed procedures and "what does NOT happen" list in Doc 12. Verify all [TIMELINE_2_LABEL] claims against Doc 12 and the historical context section.

**Checklist for [DOMAIN_1_LABEL] scenes:**
- [ ] [DOMAIN_1_CHECKLIST_ITEM_1]
- [ ] [DOMAIN_1_CHECKLIST_ITEM_2]
- [ ] [DOMAIN_1_CHECKLIST_ITEM_3]
- [ ] [DOMAIN_1_CHECKLIST_ITEM_4]
- [ ] [DOMAIN_1_CHECKLIST_ITEM_5]

**Checklist for [TIMELINE_2_LABEL] scenes:**
- [ ] [TIMELINE_2_CHECKLIST_ITEM_1]
- [ ] [TIMELINE_2_CHECKLIST_ITEM_2]
- [ ] [TIMELINE_2_CHECKLIST_ITEM_3]
- [ ] [TIMELINE_2_CHECKLIST_ITEM_4]

---

### Layer 5: Dual-POV Consistency

Read all [POV_CHARACTER_1] chapters in the batch consecutively, without the [POV_CHARACTER_2] chapters. Then read all [POV_CHARACTER_2] chapters consecutively, without the [POV_CHARACTER_1] chapters.

**Assessment questions:**
- Do the [POV_CHARACTER_1] chapters feel like a consistent register — [POV_CHARACTER_1_REGISTER_DESCRIPTION]?
- Do the [POV_CHARACTER_2] chapters feel like a consistent register — [POV_CHARACTER_2_REGISTER_DESCRIPTION]?
- If you covered the chapter heading, could you identify the POV character from the first paragraph?

**Flag format:** `DUAL-POV: Chapter [N] | [VOICE_REGISTER_FAILURE_DESCRIPTION] | e.g., "[POV_CHARACTER_2]'s narration in Chapter [N] reads as [POV_CHARACTER_1]'s register; their distinctive voice is absent."`

> Note for agent: Layer 5 requires reading all of one character's chapters consecutively rather than in alternating order. This is the only way to detect voice drift that happens gradually — a single chapter that is slightly less distinctive than the previous one is hard to catch; five consecutive chapters where the voice has progressively faded is immediately apparent.

---

### Layer 6: Timeline Rhyme Check

For each pair of adjacent chapters (one [POV_CHARACTER_1] / one [POV_CHARACTER_2]), verify that the two chapters are in a meaningful structural relationship. The relationship should be one of: rhyme (they echo each other), contrast (they make the same moment look different), or complication (the past chapter adds information that recontextualizes the present, or vice versa).

**Flag format:** `TIMELINE RHYME: Chapters [N] and [N_PLUS_1] | [DESCRIPTION_OF_FAILURE] | e.g., "These two chapters are not in dialogue; switching from Ch [N] to Ch [N_PLUS_1] loses momentum without reward."`

A failed timeline rhyme check does not necessarily mean revising the chapter — it may mean revising the sequencing decision (which chapter follows which).

---

### Layer 7: Canon Compliance

Verify all Tier 1 and Tier 2 facts from Doc 10 are honored across the five chapters. Specifically verify that no Tier 2 fact has been implicitly changed — through accumulated small decisions rather than a single obvious error.

**Most common implicit Tier 2 drift:**
- [TIER_2_DRIFT_EXAMPLE_1]
- [TIER_2_DRIFT_EXAMPLE_2]
- [TIER_2_DRIFT_EXAMPLE_3]

---

## Sweep B: Per Chapter (Layers 8–13)

Run Layers 8–13 after each individual chapter is drafted. These layers apply to one chapter at a time.

---

### Layer 8: Prose Quality Gate

Score the chapter using the 16-dimension rubric in Doc 08. Apply the ×0.85 calibration.

**Gate:** Calibrated score ≥ 7.0. Any chapter below 7.0 calibrated is flagged for revision before the chapter proceeds to Layers 9–13. A chapter below 5.0 calibrated is returned for full redraft.

---

### Layer 9: Free Indirect Discourse Audit

Scan the chapter for explicit thought-attribution markers:
- "she thought that"
- "she felt"
- "she wondered if"
- "she realized"
- "she noticed"

**Threshold:** Fewer than 5 explicit attribution markers per chapter. Any chapter with 5 or more requires a targeted revision pass to convert explicit attribution to genuine FID or to cut the attributed thought entirely.

> Note for agent: Layer 9 is a separate layer rather than part of the prose quality assessment because it identifies a systematic structural error that hides from holistic quality evaluation. A chapter with many explicit attribution markers can still feel like literary fiction to a reader assessing it holistically — the individual markers seem fine; the cumulative effect (that the narration is constantly separating itself from the character's perspective) is what fails. Counting the markers systematically catches what holistic reading misses.

---

### Layer 10: Pacing Sweep

Verify the chapter's scene density matches its position in the story's momentum curve.

| Act | Chapters | Expected density |
|-----|----------|-----------------|
| Act 1 | [ACT_1_CHAPTER_RANGE] | Establishing. Scenes may breathe. A chapter can spend time in a location without advancing plot. |
| Act 2A | [ACT_2A_CHAPTER_RANGE] | Building pressure. Each chapter should end with the reader in a different position than they started. |
| Act 2B | [ACT_2B_CHAPTER_RANGE] | Accelerating. Multiple developments per chapter. |
| Act 3 | [ACT_3_CHAPTER_RANGE] | Compressed. Chapters shorter. Scenes dense. The dual timelines converging. |

**Flag format:** `PACING: Chapter [N] | [ACT_POSITION] | [DENSITY_ASSESSMENT] | e.g., "Chapter [N] (Act 2B) has one scene and no forward movement — pacing inconsistent with momentum curve."`

Also check: chapter word count. Act 3 chapters should not be the longest chapters. A late chapter that runs far over the act-appropriate length when the pacing calls for compression is a flag.

---

### Layer 11: Cross-Reference Audit

Verify all explicit references between chapters are temporally accurate. If the chapter contains:
- [CROSS_REFERENCE_EXAMPLE_1] — verify [CHARACTER_NAME] was at that location before this chapter
- [CROSS_REFERENCE_EXAMPLE_2] — verify that the referenced scene preceded this chapter
- Any reference to a document, location, or piece of information the character has learned — verify the scene in which they learned it has occurred earlier in the chronology

**Flag format:** `CROSS-REF: Chapter [N] | [REFERENCE_DESCRIPTION] | [INCONSISTENCY] | e.g., "Chapter [N] references [OBJECT_OR_DISCOVERY], but [CHARACTER_NAME] doesn't find it until Chapter [LATER_CHAPTER]."`

---

### Layer 12: Dialogue Integrity

Verify that each character who speaks in the chapter does so in their established register (Doc 09, dialogue conventions).

**Quick-check markers:**
- [CHARACTER_NAME_1_DIALOGUE_CHECK]
- [CHARACTER_NAME_2_DIALOGUE_CHECK]
- [CHARACTER_NAME_3_DIALOGUE_CHECK]
- [CHARACTER_NAME_4_DIALOGUE_CHECK]

**Flag format:** `DIALOGUE: [CHARACTER] | Chapter [N] | [VIOLATION_DESCRIPTION]`

---

### Layer 13: Volatile Facts Check

Run all VFR entries (Doc 15) that are relevant to this chapter. Any entry marked "needs recheck before final" must be verified before the chapter enters final state.

**Check specifically:** [VFR_PRIORITY_ENTRIES_FOR_THIS_LAYER]

---

## Sweep C: Full Manuscript (Layer 14)

Run once, after all [CHAPTER_COUNT] chapters, [FRONTMATTER_ELEMENTS], and [BACKMATTER_ELEMENTS] are drafted and have passed Layers 1–13.

---

### Layer 14: Reader Simulation

Run all 4 reader archetypes from Doc 16 on the full manuscript. Use 3-chapter samples: beginning of each act ([ACT_1_SAMPLE_CHAPTERS]), midpoint ([MIDPOINT_SAMPLE_CHAPTERS]), and final act ([FINAL_ACT_SAMPLE_CHAPTERS]).

**Gate:** 3 of 4 archetypes return a "continuing" verdict.

**If fewer than 3 of 4 "continuing":**
- Identify which pillars (Doc 11) are failing for the archetypes that return "flagged"
- Determine whether the failure is manuscript-wide or act-specific
- Target revision at the specific pillar and act before running Layer 14 again

---

## QVP Summary Checklist

| Layer | Scope | Gate |
|-------|-------|------|
| 1: CFR Audit | Batch | All [TOTAL_ENTRY_COUNT] entries clear |
| 2: Character Consistency | Batch | Psychology visible for all [CHARACTER_COUNT] characters |
| 3: Chronological Integrity | Batch | No impossible time jumps |
| 4: Domain Accuracy | Batch | Procedure and history checklists pass |
| 5: Dual-POV Consistency | Batch | Voices distinct without chapter heading |
| 6: Timeline Rhyme | Batch | Each chapter pair in structural dialogue |
| 7: Canon Compliance | Batch | All Tier 1 and Tier 2 facts honored |
| 8: Prose Quality | Chapter | ≥ 7.0 calibrated |
| 9: FID Audit | Chapter | < 5 explicit attribution markers |
| 10: Pacing | Chapter | Density matches act position |
| 11: Cross-Reference | Chapter | All references temporally accurate |
| 12: Dialogue Integrity | Chapter | All characters in established register |
| 13: VFR Check | Chapter | All relevant volatile facts verified |
| 14: Reader Simulation | Full manuscript | 3 of 4 archetypes continuing |
