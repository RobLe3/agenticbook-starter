<!-- Book reference: Lab 7 (Chapter 7) -->
<!-- Novel-flavor example: "The Glass Meridian" -->
<!-- Flavor comparison: see novel-example/00_index.md for Short/Topic/Novel contrast table -->
# Doc 13: Character/Claim Fact Registry (CFR) — The Glass Meridian

**50 entries | 20 Character Facts + 30 Historical/Domain Claims**

---

## Overview

The CFR is the audit surface for the quality verification protocol (Doc 14). Every entry is a fixed fact that must not vary across the 28 chapters, prologue, and epilogue. Character facts (CF) drift through small incremental errors — an age that shifts, a detail that contradicts a later scene. Historical/domain claims (HC) fail catastrophically when a load-bearing historical or procedural fact is wrong.

> Note for agent: Character Facts and Historical Claims are separate sections because they fail in different ways. CF entries accumulate drift through small inconsistencies — the agent writes "Kwame, a researcher" in Chapter 3 and "Kwame, a journalist" in Chapter 9, and neither seems obviously wrong in isolation. HC entries fail catastrophically when a fact appears in authoritative dialogue (a character stating a historical claim as true) and is wrong. For HC entries marked HIGH risk, verify against an external source before the chapter enters final state.

**Conflict recording format:** If generated content contradicts a CFR entry, record: `Date | Entry violated | Chapter | Violation description | Resolution`

---

## Section A: Character Facts (CF-001 to CF-020)

| Entry | Character | Fact | Where Established | Chapters Where Relevant |
|-------|-----------|------|-------------------|------------------------|
| CF-001 | Dr. Mara Osei | Age 38 at the novel's opening | Doc 02 | All present-timeline chapters |
| CF-002 | Dr. Mara Osei | British-Ghanaian nationality | Doc 02 | Ch 01, 05, 09, 17, 27 |
| CF-003 | Dr. Mara Osei | Marine archaeologist, Imperial College London | Doc 02 | All present-timeline chapters |
| CF-004 | Dr. Mara Osei | Widowed; husband died 18 months before novel opens | Doc 02, Doc 10 Tier 1 | All present-timeline chapters — grief arc |
| CF-005 | Dr. Mara Osei | Published in Journal of African Archaeological Heritage (JAAH) | Doc 02 | Ch 01, 11, 15 |
| CF-006 | Dr. Mara Osei | PhD supervised by Alderton at Oxford | Doc 02 | Ch 01, 13, 16 |
| CF-007 | Tomás Ferreira | Age 52 | Doc 02 | Ch 01, 03, 07, 19 |
| CF-008 | Tomás Ferreira | Portuguese. Has worked Azorean waters for 30 years | Doc 02 | Ch 01, 03, 07 |
| CF-009 | Tomás Ferreira | Dive master at Horta Harbor, Faial | Doc 02 | Ch 01, 03, 07, 19 |
| CF-010 | Dr. Helena Voss | Age 57 | Doc 02 | Ch 05, 11, 21, 25 |
| CF-011 | Dr. Helena Voss | German-Portuguese — both nationalities, not one | Doc 02 | Ch 05, 25 |
| CF-012 | Dr. Helena Voss | Director of Maritime Heritage, Portuguese National Archives | Doc 02 | Ch 05, 11, 21 |
| CF-013 | Dr. Helena Voss | Has been suppressing Section C (maritime records) for 15 years | Doc 02, Doc 10 Tier 2 | Ch 05, 11, 21, 25, 27 |
| CF-014 | Kwame Osei | Age 35 — younger than Mara (38), not older | Doc 02 | Ch 05, 13, 23 |
| CF-015 | Kwame Osei | Investigative journalist based in Accra, Ghana | Doc 02 | Ch 05, 13, 19, 23 |
| CF-016 | Kwame Osei | Mara's brother — younger, not older | Doc 02 | Ch 05, 13, 23 |
| CF-017 | Prof. James Alderton | Age 65. Emeritus, Oxford | Doc 02 | Ch 03, 09, 16 |
| CF-018 | Prof. James Alderton | Mara's former PhD supervisor — not colleague, not friend in origin | Doc 02 | Ch 03, 09, 16 |
| CF-019 | Prof. James Alderton | Knew about the suppression for exactly 20 years | Doc 02, Doc 10 Tier 1 | Ch 09, 16, 25 |
| CF-020 | Isabel Santos | Age 29. Junior archivist at Torre do Tombo — not senior | Doc 02 | Ch 07, 11, 17 |

---

| Entry | Character | Fact | Where Established | Chapters Where Relevant |
|-------|-----------|------|-------------------|------------------------|
| CF-021 | Amara Quaye | Age 22 in 1872 | Doc 02 | All past-timeline chapters |
| CF-022 | Amara Quaye | Fante. Born and raised on the Gold Coast | Doc 02 | All past-timeline chapters |
| CF-023 | Amara Quaye | Educated at Cape Coast missionary school — literate in English and Twi | Doc 02 | Ch 02, 06, 10, 14 |
| CF-024 | Amara Quaye | Steward, not deck crew — different role, different access aboard ship | Doc 02 | All past-timeline chapters |
| CF-025 | Captain William Calder | Age 49 in 1872 | Doc 02 | Ch 04, 08, 12, 20 |
| CF-026 | Captain William Calder | British. Master of the *Meridian Star* — not first mate, not owner | Doc 02 | All past-timeline chapters |

---

## Section B: Historical and Domain Claims (HC-001 to HC-030)

Risk levels: HIGH = appears in authoritative character dialogue; verify before final. MED = invented-but-consistent with period; check for internal consistency. LOW = period colour; low falsifiability.

### The Meridian Star (Wreck)

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-001 | The *Meridian Star* sank in 1872 — exact year, not approximate | HIGH | Doc 10 Tier 1 (inviolable) | Prologue, Ch 01, 07, 27 |
| HC-002 | Wreck depth: 44 meters, Pico Passage | HIGH | Doc 10 Tier 2 | Ch 01, 03, 07 |
| HC-003 | Wreck location: 3.2 kilometers off Pico Passage, Azores | HIGH | Doc 10 Tier 2 | Ch 01, 03 |
| HC-004 | The *Meridian Star* was an unregistered 1872 Liverpool merchant brig | MED | Invented; consistent with period vessel registry practices | Ch 01, 07, 11 |
| HC-005 | The cargo manifest is found in a copper-sealed document cylinder in the captain's cabin | HIGH | Doc 10 Tier 1 (inviolable) | Ch 07, 09 |
| HC-006 | The copper cylinder was sealed specifically to preserve its contents — not standard cargo practice | MED | Domain inference (marine conservation) | Ch 09 |

### Marine Archaeology Procedure

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-007 | Pre-dive: site registration with IGESPAR required before material removal | HIGH | Doc 12 (fixed procedure) | Ch 01, 03 |
| HC-008 | Photogrammetric survey must precede contact with any artifact | HIGH | Doc 12 (fixed procedure) | Ch 03, 07 |
| HC-009 | 44m depth requires staged decompression; no simultaneous surfacing | HIGH | Doc 12; dive medicine | Ch 03, 07, 19 |
| HC-010 | Maximum two dives per day at 44m; no diving within 12 hours of flying | MED | Doc 12; dive medicine | Ch 03, 07 |
| HC-011 | Document cylinder retrieved in sealed container with ambient seawater; transported to lab within 4 hours | HIGH | Doc 12 (fixed procedure) | Ch 07 |
| HC-012 | Copper patina from 150-year submersion requires lab processing to safely open | HIGH | Conservation chemistry | Ch 09 |

### 1872 Fante Confederation

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-013 | The Fante Confederation was politically active 1868–1873 | HIGH | Historical record | Ch 02, 06, 14, 26 |
| HC-014 | A Fante diplomatic delegation to London in 1872 is historically plausible | HIGH | Historical record (multiple delegations sent) | Ch 06, 14, 26, 27 |
| HC-015 | Mission school literacy produced literate Fante men and women by the 1860s | MED | Historical record | Ch 02, 06 |
| HC-016 | The Fante Confederation had internal political divisions by 1872 | MED | Historical record | Ch 06, 14 |
| HC-017 | Twi and English were both used among educated Gold Coast Fante in this period | MED | Historical/linguistic record | Ch 02, 06, 10 |

### Colonial Administration and Law

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-018 | The Gold Coast was not a formal British protectorate until 1874 — not 1872 | HIGH | Historical record (key date) | Ch 06, 14, 26 |
| HC-019 | Cape Coast Castle was the seat of British colonial administration on the Gold Coast | HIGH | Historical record | Ch 02, 06, 10, 14 |
| HC-020 | Cargo manifest falsification was a criminal offense under 1872 Board of Trade regulations | HIGH | Legal history inference | Ch 12, 20, 26 |
| HC-021 | The Fante Confederation sent multiple delegations to negotiate with the British government | MED | Historical record | Ch 14, 26 |

### The Falsification (Plot-Critical)

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-022 | Waterhouse & Sons (Liverpool) ordered the cargo manifest falsification — Calder followed orders, did not initiate | HIGH | Doc 10 Tier 2; plot structure | Ch 12, 20, 24, 27 |
| HC-023 | Calder falsified the manifest under commercial pressure, not personal animus | MED | Character psychology (Doc 02, Doc 06) | Ch 04, 08, 12, 20 |
| HC-024 | The suppression of the Fante diplomatic commission records extended beyond the manifest | HIGH | Doc 10 Tier 1 | Ch 21, 25, 27 |

### Archive and Institutional Claims

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-025 | Torre do Tombo (Arquivo Nacional Torre do Tombo) holds Portuguese maritime records | HIGH | Institutional fact | Ch 07, 11, 17 |
| HC-026 | The restricted Section C at the Torre do Tombo contains maritime records suppressed from public access | MED | Invented restriction; plausible institutional structure | Ch 07, 11, 17, 21 |
| HC-027 | The British Library holds the 1872 newspaper archive and Calder Estate papers | MED | Institutional fact + invented estate papers | Ch 05, 13 |
| HC-028 | The Calder Estate papers are sealed until 2031 | MED | Invented; plausible (100-year seal from 1931) | Ch 13, 25 |
| HC-029 | The Pico harbormaster's log from 1872 survives in Portuguese regional archives | MED | Invented but procedurally plausible | Ch 22, 25 |

### Period Shipping

| Entry | Claim | Risk | Source Type | Chapters Where Used |
|-------|-------|------|------------|---------------------|
| HC-030 | A Liverpool-based merchant brig of this class in the 1860s–70s would have a crew of 12–18, including a steward | MED | Maritime history inference | Ch 04, 08, 20 |

---

## Conflict Log

Record violations here. Format: `Date | Entry violated | Chapter | Violation description | Resolution`

| Date | Entry | Chapter | Violation | Resolution |
|------|-------|---------|-----------|-----------|
| — | — | — | No violations recorded | — |
