<!-- Book reference: Lab 7 (Chapter 7) -->
<!-- Novel-flavor example: "The Glass Meridian" -->
<!-- Flavor comparison: see novel-example/00_index.md for Short/Topic/Novel contrast table -->
# Doc 15: Volatile Facts Register (VFR) — The Glass Meridian

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
| V-001 | Fante diplomatic missions to London: specific dates and composition of the delegations sent in the early 1870s | HIGH | New archival work on the Fante Confederation or Gold Coast colonial correspondence; publication of new scholarly work on the period | February 2026 |
| V-002 | Cape Coast missionary school literacy rates among Fante in the 1860s, including female literacy | MED | New scholarship on Gold Coast education history or missionary society records | February 2026 |
| V-003 | 1872 Fante Confederation political structure: internal factions, leadership, and the specific nature of its diplomatic authority | HIGH | New historiography on Fante political organization; publication of primary sources from the period | February 2026 |
| V-004 | Cargo manifest falsification penalties under 1872 Board of Trade regulations: specific statute and severity | MED | Access to 1872 Board of Trade records or maritime law scholarship covering this period | February 2026 |
| V-005 | Liverpool merchant vessel specifications for a brig of this class in the 1860s: crew complement, cargo capacity, voyage duration | MED | Merchant shipping registry records from the period; maritime history scholarship | February 2026 |
| V-006 | Portuguese harbormaster record-keeping requirements in the Azores in 1872: what logs were required, how they were stored | LOW | Portuguese maritime archive scholarship or Azorean regional history | February 2026 |
| V-007 | Waterhouse & Sons is an invented company name; however, the structure of Liverpool merchant houses engaged in West African trade in the 1870s must match historical practice | MED | New scholarship on Liverpool merchant trade with the Gold Coast in the 1860s–1880s | February 2026 |

---

## Category 2: Marine Archaeology Procedure

Claims subject to regulatory change or updates to professional practice standards. 5 entries.

| Entry | Claim | Risk | Recheck Trigger | Last Verified |
|-------|-------|------|-----------------|---------------|
| V-008 | IGESPAR registration process and requirements for found-wreck reporting in Portuguese territorial waters | HIGH | Changes to Portuguese maritime heritage law or IGESPAR's regulatory framework; any institutional reorganization of Portuguese cultural heritage bodies | February 2026 |
| V-009 | Portuguese maritime law on found-wreck reporting: the specific obligation to report and timeline for doing so | HIGH | Legislative changes to Portuguese maritime law; EU maritime heritage directives that would apply to Azorean waters | February 2026 |
| V-010 | Decompression schedule for 44m depth with a 20-minute bottom time: specific stop depths and durations | MED | Updates to PADI/NAUI decompression tables; new dive medicine research on staged decompression requirements | February 2026 |
| V-011 | Copper patina preservation chemistry for objects submerged in seawater for 150 years: handling requirements and stabilization process | LOW | Advances in marine conservation chemistry; changes to professional conservation standards for found-metal artifacts | February 2026 |
| V-012 | XRF (X-ray fluorescence) analysis for copper alloy dating and provenance assessment: methodology and what it can and cannot determine | LOW | Advances in XRF methodology; new applications to maritime archaeology | February 2026 |

---

## Category 3: Institutional Details

Claims about real institutions that may have changed their structure, access policies, or holdings. 4 entries.

| Entry | Claim | Risk | Recheck Trigger | Last Verified |
|-------|-------|------|-----------------|---------------|
| V-013 | Torre do Tombo (Arquivo Nacional Torre do Tombo) archive access procedures: current process for researcher access, restrictions on restricted collections, identity verification requirements | HIGH | Changes to ANTT access policy; any new digitisation project that would make previously restricted materials available; any new restriction on previously accessible materials | February 2026 |
| V-014 | British Library Calder Estate papers sealed until 2031: estate paper seals are sometimes revised by court order or family request | MED | Any court proceedings relating to the Calder Estate (invented, but the mechanism is real); changes to British Library estate deposit terms | February 2026 |
| V-015 | Imperial College London marine archaeology department structure: specifically, whether Mara's institutional affiliation and departmental home are plausible within the current ICL organisational structure | MED | ICL departmental reorganization; any significant change to the Earth Science and Engineering faculty structure | February 2026 |
| V-016 | National Archives of Ghana maritime and colonial collection holdings: scope and accessibility of the 19th-century Gold Coast colonial correspondence | MED | NAG digitisation projects; changes to access for colonial-era records; new acquisitions from British archives | February 2026 |

---

## Category 4: Plot-Dependent Claims

Claims that can be falsified not by external research but by choices made in later chapters. This category is unique to fiction.

> Note for agent: Plot-dependent claims are the VFR category most likely to be overlooked during verification. They do not require checking against external sources — they require checking against the manuscript itself. An entry in this category is a signal that says: "when you write Chapter N, verify that the choice you make is consistent with what this entry says." Run Category 4 entries as part of Layer 13 (Volatile Facts Check) in the QVP.

| Entry | Claim | Risk | Recheck Trigger | Last Verified |
|-------|-------|------|-----------------|---------------|
| V-017 | Amara's log survival mechanism: the copper document cylinder (Doc 10 Tier 1 fact) must remain the sole mechanism by which the log material survives 150 years — no other survival mechanism should be introduced or implied in any of the 28 chapters | HIGH | Any chapter in the 1872 timeline that depicts Amara writing, hiding, or transmitting the log in any way other than the established mechanism; any chapter that implies a second copy exists | February 2026 |
| V-018 | The harbormaster's log from Pico, 1872: this in-world document must not be referenced, anticipated, or foreshadowed in any chapter before Mara finds it in Chapter 22 — neither Mara nor any other character should know it exists before that point | HIGH | Any present-timeline chapter before Chapter 22 that references Pico archival records; any conversation in which a character suggests checking Pico for records | February 2026 |
| V-019 | Alderton's specific knowledge: he knew the location of the suppressed documents (where Section C was held and what it contained in general) but did not know the content of the diplomatic commission itself — this distinction between knowing about a suppression and knowing the specifics of what was suppressed must hold across all his chapters | HIGH | Any chapter (before or after the Chapter 16 reveal) in which Alderton demonstrates knowledge that goes beyond the established scope; any dialogue in which he says or implies he knew the content of the Fante commission | February 2026 |
| V-020 | Helena Voss's motivation: she suppressed Section C for professional reputation and institutional protection — not for financial gain, not for political ideology, not on behalf of any government — this must be consistently implied (not stated) across all her scenes | HIGH | Any chapter in which another character speculates about or discovers Voss's motivation; any chapter in which Voss's behavior could be read as financially motivated; the Chapter 25 confrontation scene, which is the highest risk moment for motivation drift | February 2026 |

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
