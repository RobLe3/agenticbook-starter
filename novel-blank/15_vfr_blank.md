# Doc 15: Volatile Facts Register (VFR) — [NOVEL_TITLE]

**20 entries | 4 categories | Novel-flavor fiction**

---

## Overview

The Volatile Facts Register (VFR) tracks claims that might require updating due to new historical scholarship, regulatory changes, evolving archival access, or choices made in later chapters. It is distinct from the CFR (Doc 13), which tracks fixed facts. VFR entries are facts that were accurate when established but carry a recheck trigger — a condition under which they should be verified again before the chapter enters final state.

> Note for agent: The "plot-dependent claims" category (Category 4) is unique to fiction. Non-fiction VFRs track external facts that might change due to new research or regulation. Fiction VFRs must also track internal consistency claims — facts that can be falsified not by the outside world but by choices the author makes in later chapters. This is the layer of verification that most static-prompt workflows miss entirely: the claim that was consistent in Chapter 3 is no longer consistent after the decision made in Chapter 19. Category 4 entries exist specifically to catch this class of error.

**Entry format:** `V-XXX | Claim | Risk | Recheck Trigger | Last Verified`

---

## Category 1: Historical Scholarship

Claims that may be revised by new archival work or historiographical development. 7 entries.

| Entry | Claim | Risk | Recheck Trigger | Last Verified |
|-------|-------|------|-----------------|---------------|
| V-001 | [VOLATILE_CLAIM_DESCRIPTION] | HIGH | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-002 | [VOLATILE_CLAIM_DESCRIPTION] | MED | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-003 | [VOLATILE_CLAIM_DESCRIPTION] | HIGH | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-004 | [VOLATILE_CLAIM_DESCRIPTION] | MED | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-005 | [VOLATILE_CLAIM_DESCRIPTION] | MED | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-006 | [VOLATILE_CLAIM_DESCRIPTION] | LOW | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-007 | [VOLATILE_CLAIM_DESCRIPTION] | MED | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |

---

## Category 2: [DOMAIN_1_LABEL] Procedure

Claims subject to regulatory change or updates to professional practice standards. 5 entries.

| Entry | Claim | Risk | Recheck Trigger | Last Verified |
|-------|-------|------|-----------------|---------------|
| V-008 | [VOLATILE_CLAIM_DESCRIPTION] | HIGH | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-009 | [VOLATILE_CLAIM_DESCRIPTION] | HIGH | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-010 | [VOLATILE_CLAIM_DESCRIPTION] | MED | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-011 | [VOLATILE_CLAIM_DESCRIPTION] | LOW | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-012 | [VOLATILE_CLAIM_DESCRIPTION] | LOW | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |

---

## Category 3: Institutional Details

Claims about real institutions that may have changed their structure, access policies, or holdings. 4 entries.

| Entry | Claim | Risk | Recheck Trigger | Last Verified |
|-------|-------|------|-----------------|---------------|
| V-013 | [VOLATILE_CLAIM_DESCRIPTION] | HIGH | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-014 | [VOLATILE_CLAIM_DESCRIPTION] | MED | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-015 | [VOLATILE_CLAIM_DESCRIPTION] | MED | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-016 | [VOLATILE_CLAIM_DESCRIPTION] | MED | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |

---

## Category 4: Plot-Dependent Claims

Claims that can be falsified not by external research but by choices made in later chapters. This category is unique to fiction.

> Note for agent: Plot-dependent claims are the VFR category most likely to be overlooked during verification. They do not require checking against external sources — they require checking against the manuscript itself. An entry in this category is a signal that says: "when you write Chapter N, verify that the choice you make is consistent with what this entry says." Run Category 4 entries as part of Layer 13 (Volatile Facts Check) in the QVP.

| Entry | Claim | Risk | Recheck Trigger | Last Verified |
|-------|-------|------|-----------------|---------------|
| V-017 | [VOLATILE_CLAIM_DESCRIPTION] | HIGH | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-018 | [VOLATILE_CLAIM_DESCRIPTION] | HIGH | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-019 | [VOLATILE_CLAIM_DESCRIPTION] | HIGH | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |
| V-020 | [VOLATILE_CLAIM_DESCRIPTION] | HIGH | [RECHECK_TRIGGER_DESCRIPTION] | [VERIFICATION_DATE] |

---

## VFR Maintenance Protocol

When a VFR entry is rechecked and updated:
1. Update the "Last Verified" date.
2. If the underlying fact has changed, update the relevant CFR entry (Doc 13) and note the change.
3. If the change requires a manuscript revision, flag the affected chapters and log the revision requirement before proceeding.

When a new volatile claim is identified during drafting:
1. Add a new V-entry with the next available number.
2. Assign risk level, recheck trigger, and initial verification date.
3. Run it immediately as a Layer 13 check on the chapter being drafted.
