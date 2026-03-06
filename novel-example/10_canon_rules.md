<!-- Book reference: Lab 7 (Chapter 7) -->
<!-- Novel-flavor example: "The Glass Meridian" -->
<!-- Flavor comparison: see novel-example/00_index.md for Short/Topic/Novel contrast table -->
# Doc 10: Canon Rules — The Glass Meridian

> **Book Lab reference — Lab 7 (Chapter 7):** If you completed Lab 7, compare your canon rules to this example — look for: 3-tier hierarchy (Inviolable/Alterable/Emergent), load-bearing facts identification, Novel-flavor depth vs Short-flavor's CFR-lite.

**Version 1.0 | Established: World Model Phase | Novel-flavor**

---

## Overview

The canon rules document establishes a three-tier hierarchy of facts for The Glass Meridian. Every fact in the novel — character detail, historical claim, plot point, procedural detail — belongs to one of these tiers. The tier determines what happens when the fact conflicts with something else.

This document does not contain all facts in the novel. It contains the facts that require explicit protection because changing them would require rewriting multiple chapters, or because they are load-bearing for the novel's central argument.

---

## Tier 1 — Inviolable

These facts cannot be changed without rewriting multiple chapters and revisiting the novel's central argument. They are stated as complete sentences because that is how they will appear in the manuscript, and because complete-sentence phrasing is searchable in a way that keyword labels are not.

> Note for agent: Tier 1 facts are written as complete sentences, not as keyword labels. "The manifest is found in a copper-sealed document cylinder in the captain's cabin" is searchable against manuscript text in a way that "manifest location: captain's cabin" is not. When running a CFR audit (Doc 14), you are pattern-matching these sentences against the prose, not looking up a keyword.

1. The *Meridian Star* sank in 1872 off the Azores — not elsewhere, and not in any other year.
2. Amara Quaye survives the voyage; her log is destroyed or confiscated by Calder before the ship reaches its final destination.
3. Dr. James Alderton knew about the suppression of the Fante diplomatic commission records for exactly twenty years before the novel opens.
4. The Fante diplomatic commission was real — within the novel's world, it occurred and was systematically erased from the official record.
5. Mara's husband died eighteen months before the novel opens. This timing is fixed because it determines which phase of grief Mara is in at every point in the present timeline.
6. The cargo manifest is found inside a copper-sealed document cylinder located in the captain's cabin of the *Meridian Star*.

**Proposed changes to any Tier 1 fact:** Require explicit human author sign-off. Do not proceed with any chapter that would require a Tier 1 change. Flag the conflict and stop.

---

## Tier 2 — Established

These facts were fixed during the world model phase. They can be changed, but only in an explicit revision session with a recorded rationale. Changing a Tier 2 fact without a recorded session is an error.

> Note for agent: Tier 2 vs. Tier 2 conflicts are the most dangerous category — they look like they should be resolvable by judgment, but they often are not. The conflict resolution protocol for Tier 2 vs. Tier 2 is binary: stop and flag to the human author. The reason for this is that Tier 2 facts are interconnected. "Helena Voss has been suppressing Section C for 15 years" is connected to "Alderton knew for 20 years" — if Voss's suppression tenure changes, Alderton's foreknowledge period may need to change too. This is not something an agent should resolve autonomously.

### Character facts (Tier 2)

| Character | Established Fact |
|-----------|-----------------|
| Dr. Mara Osei | Age 38. British-Ghanaian. Marine archaeologist. Imperial College London. |
| Tomás Ferreira | Age 52. Portuguese. Dive master, Horta Harbor, Faial. |
| Dr. Helena Voss | Age 57. German-Portuguese. Director of Maritime Heritage, Portuguese National Archives. Has been suppressing Section C for fifteen years. |
| Kwame Osei | Age 35. Ghanaian. Investigative journalist, Accra. Mara's younger brother. |
| Prof. James Alderton | Age 65. British. Emeritus, Oxford. Mara's former PhD supervisor. |
| Isabel Santos | Age 29. Portuguese. Junior archivist, Torre do Tombo. Not senior, not mid-level. |
| Amara Quaye | Age 22. Fante. Educated at Cape Coast missionary school. Steward, not deck crew. |
| Captain William Calder | Age 49. British. Master of the *Meridian Star*. |

### Wreck facts (Tier 2)

- The wreck depth is 44 meters.
- The wreck location is 3.2 kilometers off Pico Passage.
- The wreck is an unregistered 1872 Liverpool merchant brig.

### Institutional facts (Tier 2)

- Helena Voss has been suppressing Section C (maritime records) for fifteen years — not twelve, not eighteen.
- Waterhouse & Sons, Liverpool, ordered the cargo manifest falsification.

---

## Tier 3 — Flexible

These facts can be adjusted without cascading changes to other chapters. Tier 3 adjustments do not require a revision session or human sign-off — but they should be recorded in the chapter notes so the adjustment is visible during verification.

**Tier 3 includes:**
- Chapter-level scene detail: which specific café in Horta, exact time of day, secondary character names (the harbor official, the archivist's colleague)
- Dialogue specifics: the exact words of a conversation (not the gist — the gist may be Tier 2 if it conveys a plot-critical piece of information)
- Weather and ambient description
- The specific document Kwame retrieves at the National Archives of Ghana, and the mechanism by which he obtains access
- Isabel Santos's specific cover story for giving Mara access to Section C

---

## Conflict Resolution Protocol

This protocol is binary. There is no "agent judgment" option at Tier 1 or for Tier 2 vs. Tier 2 conflicts.

> Note for agent: The conflict resolution protocol deliberately removes agent discretion at the most critical decision points. This is not because the agent cannot reason about these conflicts — it is because the cost of a wrong autonomous resolution compounds across 28 chapters. An agent that resolves a Tier 2 conflict incorrectly in Chapter 8 may generate 20 chapters of inconsistent prose before the error surfaces. Stopping and flagging is always the right action.

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
