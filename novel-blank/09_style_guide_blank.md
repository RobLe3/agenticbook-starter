# Doc 09: Style Guide — [NOVEL_TITLE]

**Novel-flavor | [GENRE_DESCRIPTION] | [STRUCTURAL_DESCRIPTION]**

---

## Overview

This document is the authoritative prose standard for [NOVEL_TITLE]. Every chapter draft is checked against these rules before scoring. When a scoring dimension and a style rule conflict, the style rule wins — the scoring rubric measures how well the style is executed, not whether to follow it.

---

## Part I: Voice

### Register

[PROSE_REGISTER_DESCRIPTION]

> Note for agent: "Precise, unhurried, emotionally attentive" is a compass, not a formula. When in doubt, prefer the specific detail over the general statement, the slower sentence over the fast one, and the underwritten emotional moment over the explained one.

### [POV_CHARACTER_1]'s Chapters

[PROTAGONIST_VOICE_DESCRIPTION]

**Signal phrases to watch for:** [POV_CHARACTER_1_VOICE_WARNING]

### [POV_CHARACTER_2]'s Chapters

[SECONDARY_POV_VOICE_DESCRIPTION]

- **[SECONDARY_POV_INTERNAL_REGISTER_LABEL]:** [SECONDARY_POV_INTERNAL_VOICE_DESCRIPTION]
- **[SECONDARY_POV_PERFORMED_REGISTER_LABEL]:** [SECONDARY_POV_PERFORMED_VOICE_DESCRIPTION]

**Signal phrases to watch for:** [POV_CHARACTER_2_VOICE_WARNING]

> Note for agent: The two POV voices are the most important craft differentiator in this novel. If you cover the chapter heading and cannot tell from the first paragraph whether you are in [POV_CHARACTER_1]'s chapter or [POV_CHARACTER_2]'s, the voice differentiation has failed. This is the most common failure mode in AI-generated dual-timeline fiction — the prose defaults to a unified register and the chapter heading does all the work.

---

## Part II: Point of View

**Rule:** Third person limited, deep. No head-hopping within scenes. One POV character per chapter, always.

**Free indirect discourse (FID):** The primary technique for conveying character interiority. The character's thought-world enters the narration without "she thought" tags. The reader inhabits the character's perspective through the narration itself, not through reported thought.

**Example of what to avoid:**
> [EXPLICIT_ATTRIBUTION_EXAMPLE]

**Example of FID:**
> [FID_EXAMPLE]

The second version does not signal whose thought this is — the reader fills in that it is [POV_CHARACTER_1]'s inference. This is FID working correctly.

**Irony rule:** The reader may know something the POV character does not — but only through what the POV character notices without understanding. The narration does not wink at the reader. It does not step outside the POV character's knowledge to signal the irony. The reader earns the irony by paying attention to what the character fails to understand.

> Note for agent: POV discipline is stated this explicitly because POV leakage is the most common AI failure in literary fiction. The narration will slip into brief omniscience — a sentence that reports what another character is feeling, or a narratorial observation that the POV character could not have made. Run a POV audit on every chapter: every sentence should be something the POV character could see, think, infer, or notice.

---

## Part III: Tense

- **[TIMELINE_1_LABEL] ([POV_CHARACTER_1]'s chapters):** Past tense.
- **[TIMELINE_2_LABEL] ([POV_CHARACTER_2]'s chapters):** Past tense.

Both timelines are written in past tense. The [TIMELINE_DISTANCE_QUALITY] is established through [TIMELINE_DIFFERENTIATION_MECHANISM] — not through tense shift.

> Note for agent: The most common beginner error in dual-timeline fiction is using present tense for the "present" chapters to signal contemporaneity. This novel does not do that. Past tense for both timelines is a deliberate choice: it puts both timelines at the same narrative distance, which is part of the novel's argument about [TENSE_THEMATIC_RATIONALE].

---

## Part IV: Structural Conventions

### Chapter Openings

Begin in scene. No generalities. The first paragraph establishes physical location and the POV character's attention within three sentences. The reader should know within the first paragraph: where we are, whose eyes we are seeing through, and what that person is attending to.

### Chapter Endings

End on a shift. The shift can be:
- A new piece of information that changes what the reader understands
- A decision by the POV character (not announced, but made)
- An image that resonates with the chapter's thematic material

**Do not end on:** Action-thriller cliffhangers. The chapter ending is not a hook — it is a completion that opens a question. The question should be intellectual or emotional, not suspenseful.

### Section Breaks

Three asterisks (`***`) centered on their own line. Maximum two per chapter.

### Dialogue

| Character | Dialogue Convention |
|-----------|-------------------|
| [CHARACTER_NAME_1] | [CHARACTER_NAME_1_DIALOGUE_STYLE] |
| [CHARACTER_NAME_2] | [CHARACTER_NAME_2_DIALOGUE_STYLE] |
| [CHARACTER_NAME_3] | [CHARACTER_NAME_3_DIALOGUE_STYLE] |
| [CHARACTER_NAME_4] | [CHARACTER_NAME_4_DIALOGUE_STYLE] |
| [CHARACTER_NAME_5] | [CHARACTER_NAME_5_DIALOGUE_STYLE] |
| [CHARACTER_NAME_6] | [CHARACTER_NAME_6_DIALOGUE_STYLE] |
| [CHARACTER_NAME_7] | [CHARACTER_NAME_7_DIALOGUE_STYLE] |
| [CHARACTER_NAME_8] | [CHARACTER_NAME_8_DIALOGUE_STYLE] |

---

## Part V: Jargon Policy

### [DOMAIN_1_LABEL] Terms

[DOMAIN_1_JARGON_POLICY]

**What to avoid:** [DOMAIN_1_JARGON_AVOID]

### [DOMAIN_2_LABEL] Terms

[DOMAIN_2_JARGON_POLICY]

**What to avoid:** [DOMAIN_2_JARGON_AVOID]

> Note for agent: Period accuracy in [POV_CHARACTER_2]'s chapters is both a craft and an ethical responsibility. [DOMAIN_2_ETHICAL_NOTE] When in doubt: specific period detail over general historical atmosphere.

---

## Part VI: Structural Element Policy

This is literary fiction. The structural conventions differ from non-fiction.

- **No callout boxes within chapters.** The manuscript has no tcolorbox environments, no sidebars, no margin notes within chapters.
- **[EPISTOLARY_ELEMENT_LABEL]:** [EPISTOLARY_ELEMENT_POLICY]
- **Chapter headers:** Chapter number + timeline marker in brackets. Format: `Chapter 7 [TIMELINE_1_MARKER]` or `Chapter 8 [TIMELINE_2_MARKER]`. The timeline marker appears on its own line below the chapter number.
- **No chapter epigraphs** unless explicitly approved per chapter in Doc 05 (narrative architecture). Epigraphs are not a default structural element.

---

## Part VII: What Good Looks Like

A chapter that executes this style guide well has the following qualities:

1. You can cover the chapter heading and identify the POV character from the first paragraph.
2. The most emotionally significant moment in the chapter is underwritten — the reader feels it without being told to.
3. Every [DOMAIN_1] or [DOMAIN_2] term that appears is either contextually clear or appropriately glossed for a non-specialist character present in the scene.
4. The chapter ends with a question — not a cliffhanger, but something incomplete that the reader wants to resolve.
5. No explicit thought-attribution markers survive: "she thought," "she felt," "she wondered if" are converted to FID or cut.
