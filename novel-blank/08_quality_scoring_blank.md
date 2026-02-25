# Doc 08: Quality Scoring — [NOVEL_TITLE]

**Novel-flavor | 16 dimensions | Calibration: ×0.85**

---

## Why 16 Dimensions?

Topic-flavor fiction uses 12 quality dimensions. Novel-flavor adds four more: Dual-POV Consistency, Free Indirect Discourse, Chronological Integrity, and Canon Compliance. These four are fiction-specific failure modes that do not appear in non-fiction. Topic books have a single narrator; non-fiction does not require chronological integrity across two independent timelines; and canon compliance becomes critical only when a story world has fixed facts that must hold across [CHAPTER_COUNT] chapters.

> Note for agent: When you read documentation saying "16 dimensions" and another document says "12 dimensions," both are correct — they apply to different flavors. [NOVEL_TITLE] is Novel-flavor. Always use the 16-dimension rubric here.

---

## The 16 Dimensions

### Group 1: Prose Craft (38% total weight)

| # | Dimension | Weight | What It Measures |
|---|-----------|--------|------------------|
| 1 | Voice Consistency | 12% | Does the prose maintain its established register across scenes and chapters? Does [POV_CHARACTER_1]'s chapter feel like [POV_CHARACTER_1], and [POV_CHARACTER_2]'s feel like [POV_CHARACTER_2], from first page to last? |
| 2 | Sentence Rhythm | 8% | Does sentence length and structure vary purposefully — not randomly? Short sentences at moments of decision. Longer sentences during observation. The variation should be audible. |
| 3 | Specificity | 10% | Are generic descriptions replaced with concrete, particular detail? Not a generic sensory impression — what precisely does the detail tell us about [POV_CHARACTER_1] noticing it? |
| 4 | Free Indirect Discourse | 8% | For close-third POV, does the character's thought-world enter the narration without explicit attribution? Thought should appear as inflected narration, not tagged summary. |

> Note for agent: Voice Consistency is the highest-weighted prose dimension because it is the most common place AI-generated literary fiction fails. A score of 10 here requires rereading the first page of a chapter and then the last page and verifying they feel like the same register.

---

### Group 2: Structural Integrity (36% total weight)

| # | Dimension | Weight | What It Measures |
|---|-----------|--------|------------------|
| 5 | Chapter Function | 10% | Does every chapter change something in the reader's understanding — not just move plot? A chapter that only moves plot fails this dimension. |
| 6 | Timeline Coherence | 8% | Do the two timelines rhyme, contrast, or complicate each other structurally? Switching to [TIMELINE_2_PERIOD] must feel like gaining information, not losing momentum. |
| 7 | Pacing | 8% | Does the chapter's scene density match its place in the story's momentum curve? Act 1 chapters may breathe. Act 3 chapters may not. |
| 8 | Dual-POV Consistency | 10% | Do [POV_CHARACTER_1] and [POV_CHARACTER_2] have genuinely different voices, different relationship to language, different worldviews? If you covered the chapter heading, could you tell which POV you are in? |

> Note for agent: Dual-POV Consistency (D8) is one of the four Novel-flavor additions absent in Topic rubrics. It is weighted at 10% — the same as Chapter Function — because dual-timeline literary fiction fails most visibly here. AI prose tends toward a unified register; the chapter heading is doing work the prose itself should be doing.

---

### Group 3: Emotional Architecture (26% total weight)

| # | Dimension | Weight | What It Measures |
|---|-----------|--------|------------------|
| 9 | Reader Investment | 8% | Does the reader have a reason to care about what happens in this chapter — not just about the outcome of the novel? |
| 10 | Tension Maintenance | 8% | Is there an active question the reader wants answered, even in quieter scenes? Tension does not require conflict; it requires incompleteness. |
| 11 | Thematic Resonance | 6% | Does the chapter connect to the novel's central argument about [CENTRAL_THEME]? This should happen through scene, not through character speech. |
| 12 | Restraint | 4% | Are the most emotional moments underwritten rather than overwritten? The prose should not instruct the reader to feel. |

> Note for agent: Restraint (D12) is weighted at only 4% because it is a pass/fail criterion in practice — a chapter that over-writes its emotional moments cannot be rescued by excellence in other dimensions. A low Restraint score is a flag to revise regardless of the overall weighted total.

---

### Group 4: Accuracy and Integrity (6% total weight + binary gate)

| # | Dimension | Weight | What It Measures |
|---|-----------|--------|------------------|
| 13 | Domain Accuracy | 8% | [DOMAIN_1] and [DOMAIN_2] details are consistent with Doc 12 (domain authenticity). The "what does NOT happen" list applies here. |
| 14 | Character Consistency | 6% | All [CHARACTER_COUNT] characters behave in ways traceable to their Doc 02 profiles. |
| 15 | Chronological Integrity | 4% | Both timelines maintain correct internal chronology and do not create paradoxes. |
| 16 | Canon Compliance | 2% | All CFR claims (Doc 13) upheld; no contradiction with Doc 10 (canon rules). **Binary: pass or fail. A fail here invalidates the chapter regardless of other scores.** |

> Note for agent: Canon Compliance is the only binary dimension. A chapter that scores 9.8 across fifteen dimensions but contradicts a Tier 1 canon rule is not a 9.8 chapter — it is a failed chapter. Check Doc 10 and Doc 13 before scoring this dimension. A fail here means revision is required before any other score is meaningful.

---

## Scoring Formula

```
Weighted Score = Σ (score_i × weight_i)   for i = 1 to 16

where score_i is on a 1–10 scale
and weight_i are the percentages above (sum = 100%)
```

**Step 1:** Score each of the 16 dimensions on a 1–10 scale.
**Step 2:** Verify Canon Compliance (D16). If fail: stop, revise, rescore.
**Step 3:** Calculate weighted sum.
**Step 4:** Apply calibration: `Calibrated Score = Raw Score × 0.85`

> Note for agent: The ×0.85 calibration is not optional and is not a penalty. It is a correction for AI self-assessment inflation, which runs approximately 15% optimistic on literary quality dimensions. A raw score of 8.8 calibrates to 7.5 — the publication threshold. This is by design.

---

## Minimum Thresholds

| Stage | Calibrated Threshold | Notes |
|-------|---------------------|-------|
| Draft | ≥ 5.0 | Chapter is usable as a working draft |
| Revision-ready | ≥ 7.0 | Chapter passes to revision queue |
| Publication-ready | ≥ 7.5 | Chapter meets final standard |
| Ship-it gate | ≥ 7.5 AND 5 of 5 ship-it signals | See below |

**The 5 ship-it signals:**
1. Canon Compliance: Pass
2. Domain Accuracy: ≥ 7.0
3. Dual-POV Consistency: ≥ 7.0
4. Restraint: ≥ 6.0 (underwriting, not overwriting, the emotional moments)
5. Reader Investment: ≥ 7.0

---

## Lowest-Scoring Dimensions in AI-Generated Dual-Timeline Fiction

Based on the methodology documented in the Nordlicht project and generalizable to Novel-flavor fiction:

1. **Free Indirect Discourse (D4):** AI defaults to explicit attribution ("she thought," "she felt"). Converting these to genuine FID requires revision sweeps, not initial generation.
2. **Dual-POV Consistency (D8):** AI generates unified prose; the chapter heading differentiates the POVs but the prose itself often does not.
3. **Restraint (D12):** AI tends to tell the reader what to feel at moments of emotional weight. Over-writing is the default; under-writing requires deliberate revision.
4. **Timeline Coherence (D6):** AI-generated chapter-by-chapter writing loses track of what the other timeline has established; the rhyme relationship between timelines requires explicit cross-chapter verification.

> Note for agent: If you are generating a chapter and then scoring it, expect D4, D8, and D12 to be your lowest scores. Run a targeted revision pass on these three dimensions before calculating the overall weighted score. This will raise your calibrated score by approximately 0.4–0.7 points and reduce the number of revision cycles.

---

## Quick-Score Card

For rapid in-session quality checking (not a substitute for full scoring):

| Signal | Green | Yellow | Red |
|--------|-------|--------|-----|
| POV clarity | Never in doubt | One moment ambiguous | Multiple POV slips |
| Voice register | Distinctive by first paragraph | Generic but consistent | [POV_CHARACTER_1] sounds like [POV_CHARACTER_2] |
| Emotional restraint | Show, don't explain | One over-written moment | Multiple instructions to feel |
| Domain detail | Specific and accurate | Generic | Anachronistic or procedurally wrong |
| Chapter ending | Question opened | Summary statement | Action cliffhanger |

A chapter that is Green across all five signals can proceed to the full 16-dimension score.
