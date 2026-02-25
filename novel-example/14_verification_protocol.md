<!-- Book reference: Lab 7 (Chapter 7) -->
<!-- Novel-flavor example: "The Glass Meridian" -->
<!-- Flavor comparison: see novel-example/00_index.md for Short/Topic/Novel contrast table -->
# Doc 14: Verification Protocol (QVP) — The Glass Meridian

**14-Layer Quality Verification Protocol | Novel-flavor fiction**

---

## Overview

The Quality Verification Protocol (QVP) is a structured sequence of verification passes that must be run in the order given. Order matters: errors in early layers contaminate later layers if the sequence is skipped. A CFR violation that survives into the prose quality assessment (Layer 8) will cause the quality score to be based on prose that contains a foundational error — the score is therefore meaningless.

> Note for agent: The 14 layers are divided into two sweep structures. Layers 1–7 run per five-chapter batch — after every five chapters are drafted, run these seven layers before continuing. Layers 8–13 run per chapter — after each chapter is drafted and before it is marked as done. Layer 14 runs once, after all 28 chapters are complete. This structure prevents error accumulation and catches systemic problems before they propagate across the whole manuscript.

**Total layers:** 14 (vs. 8 for Topic-flavor — the 6 additional layers address fiction-specific failure modes: character consistency sweep, timeline rhyme check, free indirect discourse audit, pacing sweep, cross-reference audit, and dialogue integrity.)

---

## Sweep A: Per Five-Chapter Batch (Layers 1–7)

Run Layers 1–7 after every five chapters are drafted. Do not continue to the next five chapters until the batch has passed all seven layers.

---

### Layer 1: CFR Audit

**Run this first. A CFR violation stops the batch.**

Check all 50 entries in Doc 13 (CFR) against the full text of the five chapters in the batch. Process the text in sections of approximately 3,000 words.

**Method:** For each CF entry, verify the fact is present where relevant and correct where stated. For each HC entry, verify the claim is accurate where it appears. Flag any discrepancy with the specific entry number (CF-xxx or HC-xxx).

**Flag format:** `CFR VIOLATION: [entry number] | Chapter [N] | [Brief description] | Fix before Layer 2.`

**Gate:** Any violation stops Layer 1. Fix all violations, then restart Layer 1 from the beginning of the batch.

> Note for agent: CFR audit runs first because character fact and historical claim errors contaminate every subsequent layer. A chapter in which Kwame is described as 40 years old (he is 35) will generate an incorrect character consistency assessment in Layer 2, an incorrect voice assessment in Layer 5, and an incorrect dialogue assessment in Layer 12. Fix the foundational fact first; then the dependent assessments are meaningful.

---

### Layer 2: Character Consistency Sweep

For each of the 8 characters who appear in the batch: verify that their psychology — specifically the wound, desire, and fear documented in Doc 06 — is visible in their scenes.

**Flag format:** `CHAR CONSISTENCY: [Character name] | Chapter [N] | [Psychology dimension absent] | e.g., "Mara acts without her defense mechanism (precision-as-control) present in this scene."`

Check specifically:
- Mara: Is her grief present even in procedural scenes? Does her defense mechanism (precision, methodical control) operate when she is under pressure?
- Amara: Is her dual-register voice maintained? Does she perform deference while thinking something different?
- Helena Voss: Is she oblique rather than direct? Does she never quite say what she means?
- Alderton (before Chapter 16): Does he maintain plausible deniability in his paternalism?

---

### Layer 3: Chronological Integrity

Verify both timelines maintain correct internal chronology. No impossible time jumps. No events occurring in the wrong sequence.

**Reference timeline (maintain across all 28 chapters):**
- 1872 timeline: Voyage from Cape Coast to Azores to Liverpool takes approximately 6 weeks. Chapter events in the 1872 timeline must be consistent with this voyage duration.
- 2024 timeline: Total investigation span is 11 weeks from Mara's first dive to the public reckoning.

**Method:** Create or update a scene-by-scene date log. For each chapter, record: Timeline (1872 / 2024), approximate date within that timeline, location, events. Verify no chapter places a character somewhere they could not yet be, or references an event that has not yet occurred.

**Flag format:** `CHRONOLOGY: Chapter [N] | [Description of impossible or contradictory timing]`

---

### Layer 4: Domain Accuracy Check

Verify all marine archaeology procedures against the fixed procedures and "what does NOT happen" list in Doc 12. Verify all 1872 colonial history claims against Doc 12 and the historical context section.

**Checklist for marine archaeology scenes:**
- [ ] No bare-hand artifact contact
- [ ] No flash photography at depth
- [ ] Copper cylinder not opened on seabed or immediately on boat
- [ ] Staged decompression depicted or referenced when relevant
- [ ] IGESPAR registration referenced before material removal

**Checklist for 1872 scenes:**
- [ ] No anachronistic language
- [ ] Fante Confederation's legal status in 1872 accurate (pre-protectorate)
- [ ] Calder's perspective consistent with period commercial norms (not retrospective guilt)
- [ ] Amara's literacy presented as plausible, not exceptional

---

### Layer 5: Dual-POV Consistency

Read all Mara chapters in the batch consecutively, without the Amara chapters. Then read all Amara chapters consecutively, without the Mara chapters.

**Assessment questions:**
- Do the Mara chapters feel like a consistent register — precise, controlled, emotionally submerged?
- Do the Amara chapters feel like a consistent register — sharper, more ironic, with the dual-voice tension?
- If you covered the chapter heading, could you identify the POV character from the first paragraph?

**Flag format:** `DUAL-POV: Chapter [N] | [Voice register failure description] | e.g., "Amara's narration in Chapter 8 reads as Victorian literary prose; her ironic detachment is absent."`

> Note for agent: Layer 5 requires reading all of one character's chapters consecutively rather than in alternating order. This is the only way to detect voice drift that happens gradually — a single Amara chapter that is slightly less ironic than the previous one is hard to catch; five consecutive Amara chapters where the irony has progressively faded is immediately apparent.

---

### Layer 6: Timeline Rhyme Check

For each pair of adjacent chapters (one Mara / one Amara), verify that the two chapters are in a meaningful structural relationship. The relationship should be one of: rhyme (they echo each other), contrast (they make the same moment look different), or complication (the past chapter adds information that recontextualizes the present, or vice versa).

**Flag format:** `TIMELINE RHYME: Chapters [N] and [N+1] | [Description of failure] | e.g., "These two chapters are not in dialogue; switching from Ch 7 to Ch 8 loses momentum without reward."`

A failed timeline rhyme check does not necessarily mean revising the chapter — it may mean revising the sequencing decision (which chapter follows which).

---

### Layer 7: Canon Compliance

Verify all Tier 1 and Tier 2 facts from Doc 10 are honored across the five chapters. Specifically verify that no Tier 2 fact has been implicitly changed — through accumulated small decisions rather than a single obvious error.

**Most common implicit Tier 2 drift:**
- Helena Voss's suppression tenure shifting from 15 to "about a decade" or "nearly 20 years"
- Alderton's foreknowledge period described as "years" without the specific 20-year figure
- The wreck depth or distance described with different precision than established

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

> Note for agent: Layer 9 is a separate layer rather than part of the prose quality assessment because it identifies a systematic structural error that hides from holistic quality evaluation. A chapter with 12 "she thought" markers can still feel like literary fiction to a reader assessing it holistically — the individual markers seem fine; the cumulative effect (that the narration is constantly separating itself from the character's perspective) is what fails. Counting the markers systematically catches what holistic reading misses.

---

### Layer 10: Pacing Sweep

Verify the chapter's scene density matches its position in the story's momentum curve.

| Act | Chapters | Expected density |
|-----|----------|-----------------|
| Act 1 | Ch 1–8 | Establishing. Scenes may breathe. A chapter can spend time in a location without advancing plot. |
| Act 2A | Ch 9–16 | Building pressure. Each chapter should end with the reader in a different position than they started. |
| Act 2B | Ch 17–22 | Accelerating. Multiple developments per chapter. |
| Act 3 | Ch 23–28 | Compressed. Chapters shorter. Scenes dense. The dual timelines converging. |

**Flag format:** `PACING: Chapter [N] | [Act position] | [Density assessment] | e.g., "Chapter 21 (Act 2B) has one scene and no forward movement — pacing inconsistent with momentum curve."`

Also check: chapter word count. Act 3 chapters should not be the longest chapters. A Chapter 26 that runs 4,500 words when the pacing calls for compression is a flag.

---

### Layer 11: Cross-Reference Audit

Verify all explicit references between chapters are temporally accurate. If the chapter contains:
- "as she had discovered in Lisbon" — verify Mara was in Lisbon before this chapter
- "what Kwame had found in Accra" — verify that Kwame's Accra scenes preceded this chapter
- Any reference to a document, location, or piece of information the character has learned — verify the scene in which they learned it has occurred earlier in the chronology

**Flag format:** `CROSS-REF: Chapter [N] | [Reference description] | [Inconsistency] | e.g., "Chapter 17 references the Pico harbormaster's log, but Mara doesn't find it until Chapter 22."`

---

### Layer 12: Dialogue Integrity

Verify that each character who speaks in the chapter does so in their established register (Doc 09, dialogue conventions).

**Quick-check markers:**
- Helena Voss has no line that states her meaning directly
- Mara has no line of small talk
- Amara's performed dialogue (when speaking aloud to Calder or the ship's officers) uses formally correct English; her internal voice is different
- Alderton (before Chapter 16) sounds donnish and paternalistic, never direct

**Flag format:** `DIALOGUE: [Character] | Chapter [N] | [Violation description]`

---

### Layer 13: Volatile Facts Check

Run all VFR entries (Doc 15) that are relevant to this chapter. Any entry marked "needs recheck before final" must be verified before the chapter enters final state.

**Check specifically:** V-017 (Amara's log survival mechanism), V-018 (Pico harbormaster's log — not referenced before Chapter 22), V-019 (Alderton's specific knowledge — location but not content), V-020 (Helena Voss's motivation — professional reputation, not financial).

---

## Sweep C: Full Manuscript (Layer 14)

Run once, after all 28 chapters, prologue, and epilogue are drafted and have passed Layers 1–13.

---

### Layer 14: Reader Simulation

Run all 4 reader archetypes from Doc 16 on the full manuscript. Use 3-chapter samples: beginning of each act (Chapters 1–3), midpoint (Chapters 14–16), and final act (Chapters 25–27).

**Gate:** 3 of 4 archetypes return a "continuing" verdict.

**If fewer than 3 of 4 "continuing":**
- Identify which pillars (Doc 11) are failing for the archetypes that return "flagged"
- Determine whether the failure is manuscript-wide or act-specific
- Target revision at the specific pillar and act before running Layer 14 again

---

## QVP Summary Checklist

| Layer | Scope | Gate |
|-------|-------|------|
| 1: CFR Audit | Batch | All 50 entries clear |
| 2: Character Consistency | Batch | Psychology visible for all 8 characters |
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
