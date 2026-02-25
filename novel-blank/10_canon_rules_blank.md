# Doc 10: Canon Rules — [NOVEL_TITLE]

**Version 1.0 | Established: World Model Phase | Novel-flavor**

---

## Overview

The canon rules document establishes a three-tier hierarchy of facts for [NOVEL_TITLE]. Every fact in the novel — character detail, historical claim, plot point, procedural detail — belongs to one of these tiers. The tier determines what happens when the fact conflicts with something else.

This document does not contain all facts in the novel. It contains the facts that require explicit protection because changing them would require rewriting multiple chapters, or because they are load-bearing for the novel's central argument.

---

## Tier 1 — Inviolable

These facts cannot be changed without rewriting multiple chapters and revisiting the novel's central argument. They are stated as complete sentences because that is how they will appear in the manuscript, and because complete-sentence phrasing is searchable in a way that keyword labels are not.

> Note for agent: Tier 1 facts are written as complete sentences, not as keyword labels. "The manifest is found in a copper-sealed document cylinder in the captain's cabin" is searchable against manuscript text in a way that "manifest location: captain's cabin" is not. When running a CFR audit (Doc 14), you are pattern-matching these sentences against the prose, not looking up a keyword.

1. [TIER_1_FACT_1]
2. [TIER_1_FACT_2]
3. [TIER_1_FACT_3]
4. [TIER_1_FACT_4]
5. [TIER_1_FACT_5]
6. [TIER_1_FACT_6]

**Proposed changes to any Tier 1 fact:** Require explicit human author sign-off. Do not proceed with any chapter that would require a Tier 1 change. Flag the conflict and stop.

---

## Tier 2 — Established

These facts were fixed during the world model phase. They can be changed, but only in an explicit revision session with a recorded rationale. Changing a Tier 2 fact without a recorded session is an error.

> Note for agent: Tier 2 vs. Tier 2 conflicts are the most dangerous category — they look like they should be resolvable by judgment, but they often are not. The conflict resolution protocol for Tier 2 vs. Tier 2 is binary: stop and flag to the human author. The reason for this is that Tier 2 facts are interconnected. Changing one Tier 2 fact may require cascading changes to others. This is not something an agent should resolve autonomously.

### Character facts (Tier 2)

| Character | Established Fact |
|-----------|-----------------|
| [CHARACTER_NAME_1] | [CHARACTER_NAME_1_TIER2_FACTS] |
| [CHARACTER_NAME_2] | [CHARACTER_NAME_2_TIER2_FACTS] |
| [CHARACTER_NAME_3] | [CHARACTER_NAME_3_TIER2_FACTS] |
| [CHARACTER_NAME_4] | [CHARACTER_NAME_4_TIER2_FACTS] |
| [CHARACTER_NAME_5] | [CHARACTER_NAME_5_TIER2_FACTS] |
| [CHARACTER_NAME_6] | [CHARACTER_NAME_6_TIER2_FACTS] |
| [CHARACTER_NAME_7] | [CHARACTER_NAME_7_TIER2_FACTS] |
| [CHARACTER_NAME_8] | [CHARACTER_NAME_8_TIER2_FACTS] |

### [TIER_2_FACT_GROUP_1_LABEL] facts (Tier 2)

- [TIER_2_FACT_GROUP_1_ITEM_1]
- [TIER_2_FACT_GROUP_1_ITEM_2]
- [TIER_2_FACT_GROUP_1_ITEM_3]

### [TIER_2_FACT_GROUP_2_LABEL] facts (Tier 2)

- [TIER_2_FACT_GROUP_2_ITEM_1]
- [TIER_2_FACT_GROUP_2_ITEM_2]

---

## Tier 3 — Flexible

These facts can be adjusted without cascading changes to other chapters. Tier 3 adjustments do not require a revision session or human sign-off — but they should be recorded in the chapter notes so the adjustment is visible during verification.

**Tier 3 includes:**
- Chapter-level scene detail: [TIER_3_SCENE_DETAIL_EXAMPLES]
- Dialogue specifics: the exact words of a conversation (not the gist — the gist may be Tier 2 if it conveys a plot-critical piece of information)
- Weather and ambient description
- [TIER_3_FLEXIBLE_ITEM_1]
- [TIER_3_FLEXIBLE_ITEM_2]

---

## Conflict Resolution Protocol

This protocol is binary. There is no "agent judgment" option at Tier 1 or for Tier 2 vs. Tier 2 conflicts.

> Note for agent: The conflict resolution protocol deliberately removes agent discretion at the most critical decision points. This is not because the agent cannot reason about these conflicts — it is because the cost of a wrong autonomous resolution compounds across [CHAPTER_COUNT] chapters. An agent that resolves a Tier 2 conflict incorrectly in an early chapter may generate many chapters of inconsistent prose before the error surfaces. Stopping and flagging is always the right action.

| Conflict Type | Resolution |
|---------------|-----------|
| Tier 1 vs. Tier 2 | Tier 1 wins. Flag the conflict. Propose a Tier 2 revision that accommodates the Tier 1 fact. Await human approval before proceeding. |
| Tier 1 vs. Tier 3 | Tier 1 wins. Adjust the Tier 3 detail. No flag required, but note the adjustment. |
| Tier 2 vs. Tier 3 | Tier 2 wins. Adjust the Tier 3 detail. Note the adjustment. |
| Tier 2 vs. Tier 2 | Stop. Flag to human author. Do not resolve autonomously. |
| Proposed change to any Tier 1 fact | Human sign-off required. Do not proceed without approval. |

---

## Update Protocol

When a Tier 1 or Tier 2 fact is approved for change:

1. Update this document with the new fact.
2. Increment the version number (1.0 → 1.1).
3. Record the change in the log below.

**Change log:**

| Version | Date | Changed fact | What it changed from | What necessitated the change |
|---------|------|-------------|---------------------|------------------------------|
| 1.0 | World model phase | (Initial establishment) | — | — |

---

## Canon Compliance Check

Before submitting any chapter to the quality scoring rubric (Doc 08), verify:

1. No Tier 1 fact has been altered, contradicted, or implicitly overwritten.
2. No Tier 2 fact has been altered without a recorded revision session.
3. The CFR (Doc 13) shows no new violations flagged since the last chapter.

Canon Compliance is a binary dimension in the quality rubric (D16, 2% weight). A fail on this dimension invalidates the chapter score regardless of performance on the other 15 dimensions.
