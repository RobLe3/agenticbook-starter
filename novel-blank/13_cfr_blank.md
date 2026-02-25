# Doc 13: Character/Claim Fact Registry (CFR) — [NOVEL_TITLE]

**[TOTAL_ENTRY_COUNT] entries | [CF_COUNT] Character Facts + [HC_COUNT] Historical/Domain Claims**

---

## Overview

The CFR is the audit surface for the quality verification protocol (Doc 14). Every entry is a fixed fact that must not vary across the [CHAPTER_COUNT] chapters, [FRONTMATTER_ELEMENTS], and [BACKMATTER_ELEMENTS]. Character facts (CF) drift through small incremental errors — an age that shifts, a detail that contradicts a later scene. Historical/domain claims (HC) fail catastrophically when a load-bearing historical or procedural fact is wrong.

> Note for agent: Character Facts and Historical Claims are separate sections because they fail in different ways. CF entries accumulate drift through small inconsistencies — the agent writes one description in an early chapter and a contradictory description in a later chapter, and neither seems obviously wrong in isolation. HC entries fail catastrophically when a fact appears in authoritative dialogue (a character stating a historical claim as true) and is wrong. For HC entries marked HIGH risk, verify against an external source before the chapter enters final state.

**Conflict recording format:** If generated content contradicts a CFR entry, record: `Date | Entry violated | Chapter | Violation description | Resolution`

---

## Section A: Character Facts (CF-001 to CF-026)

| Entry | Character | Fact | Where Established | Chapters Where Relevant |
|-------|-----------|------|-------------------|------------------------|
| CF-001 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-002 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-003 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-004 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-005 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-006 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-007 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-008 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-009 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-010 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-011 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-012 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-013 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-014 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-015 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-016 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-017 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-018 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-019 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-020 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |

---

| Entry | Character | Fact | Where Established | Chapters Where Relevant |
|-------|-----------|------|-------------------|------------------------|
| CF-021 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-022 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-023 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-024 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-025 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |
| CF-026 | [CHARACTER_NAME] | [FACT_DESCRIPTION] | [SOURCE_DOC] | [CHAPTER_LIST] |

---

## Section B: Historical and Domain Claims (HC-001 to HC-030)

Risk levels: HIGH = appears in authoritative character dialogue; verify before final. MED = invented-but-consistent with period; check for internal consistency. LOW = period colour; low falsifiability.

### [HC_GROUP_1_LABEL]

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-001 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-002 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-003 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-004 | [FACT_DESCRIPTION] | MED | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-005 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-006 | [FACT_DESCRIPTION] | MED | [SOURCE_TYPE] | [CHAPTER_LIST] |

### [HC_GROUP_2_LABEL]

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-007 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-008 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-009 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-010 | [FACT_DESCRIPTION] | MED | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-011 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-012 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |

### [HC_GROUP_3_LABEL]

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-013 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-014 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-015 | [FACT_DESCRIPTION] | MED | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-016 | [FACT_DESCRIPTION] | MED | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-017 | [FACT_DESCRIPTION] | MED | [SOURCE_TYPE] | [CHAPTER_LIST] |

### [HC_GROUP_4_LABEL]

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-018 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-019 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-020 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-021 | [FACT_DESCRIPTION] | MED | [SOURCE_TYPE] | [CHAPTER_LIST] |

### [HC_GROUP_5_LABEL]

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-022 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-023 | [FACT_DESCRIPTION] | MED | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-024 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |

### [HC_GROUP_6_LABEL]

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-025 | [FACT_DESCRIPTION] | HIGH | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-026 | [FACT_DESCRIPTION] | MED | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-027 | [FACT_DESCRIPTION] | MED | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-028 | [FACT_DESCRIPTION] | MED | [SOURCE_TYPE] | [CHAPTER_LIST] |
| HC-029 | [FACT_DESCRIPTION] | MED | [SOURCE_TYPE] | [CHAPTER_LIST] |

### [HC_GROUP_7_LABEL]

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-030 | [FACT_DESCRIPTION] | MED | [SOURCE_TYPE] | [CHAPTER_LIST] |

---

## Conflict Log

Record violations here. Format: `Date | Entry violated | Chapter | Violation description | Resolution`

| Date | Entry | Chapter | Violation | Resolution |
|------|-------|---------|-----------|-----------|
| — | — | — | No violations recorded | — |
