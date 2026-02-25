<!--
Book reference: Lab 9 (Chapter 7: Verification Documents — VFR).
Fill in this template to create your Volatile Facts Register.
Compare to topic-example/09_vfr.md for structure guidance.
KEY DISTINCTION: Short-flavor has a VFR-lite (6 items, simpler format).
Topic-flavor requires a full VFR with 15+ claims, source citations, and recheck triggers.
-->

# Volatile Facts Register — [YOUR_PROJECT_TITLE]

**Project:** [YOUR_FULL_PROJECT_TITLE_AND_SUBTITLE]
**Flavor:** Topic ([WORD_COUNT_LOW]–[WORD_COUNT_HIGH] words)

> **Note for agent:** Volatile facts are claims that may become outdated, are frequently
> contested, or depend on external sources that can change. Check all items in this
> register before any publication update.

---

## What Makes a Fact Volatile?

A fact is volatile if:
1. It depends on a specific product, standard, or measurement that may change
2. It is drawn from consensus that may evolve as practice develops
3. It cites a statistic from the author's own data (which may be updated)
4. It involves a comparison to other books or products (competitive claims)

---

## Register

### Category 1: [EQUIPMENT_OR_PRODUCT_SPECS — e.g., "Equipment Specifications"]

| ID | Fact | Canonical Value | Source | Recheck Trigger |
|----|------|-----------------|--------|-----------------|
| V-001 | [FACT_DESCRIPTION] | [CANONICAL_VALUE] | [SOURCE_TYPE] | [WHAT_WOULD_MAKE_THIS_OUTDATED] |
| V-002 | [FACT_DESCRIPTION] | [CANONICAL_VALUE] | [SOURCE_TYPE] | [TRIGGER] |

**Last verified:** [DATE] ✓

---

### Category 2: [STANDARDS_OR_MEASUREMENTS — e.g., "Measurement Standards"]

| ID | Fact | Canonical Value | Source | Recheck Trigger |
|----|------|-----------------|--------|-----------------|
| V-003 | [FACT_DESCRIPTION] | [CANONICAL_VALUE] | [SOURCE_TYPE] | [TRIGGER] |
| V-004 | [FACT_DESCRIPTION] | [CANONICAL_VALUE] | [SOURCE_TYPE] | [TRIGGER] |
| V-005 | [FACT_DESCRIPTION] | [CANONICAL_VALUE] | [SOURCE_TYPE] | [TRIGGER] |

> **Note:** [Add any important note about geographic variation, version-specific issues,
> or other caveats for this category.]

**Last verified:** [DATE] ✓

---

### Category 3: [RESEARCH_OR_SCIENCE — e.g., "Research-Based Claims"]

| ID | Fact | Canonical Value | Source | Recheck Trigger |
|----|------|-----------------|--------|-----------------|
| V-006 | [FACT_DESCRIPTION] | [CANONICAL_VALUE] | [SOURCE_TYPE] | [TRIGGER] |
| V-007 | [FACT_DESCRIPTION] | [CANONICAL_VALUE] | [SOURCE_TYPE] | [TRIGGER] |
| V-008 | [FACT_DESCRIPTION] | [CANONICAL_VALUE] | [SOURCE_TYPE] | [TRIGGER] |

**Last verified:** [DATE] ✓

---

### Category 4: Author-Derived Statistics

| ID | Fact | Canonical Value | Source | Recheck Trigger |
|----|------|-----------------|--------|-----------------|
| V-009 | [STATISTIC_FROM_YOUR_OWN_DATA] | [VALUE] | Author's [DATA_SOURCE] (N=[SAMPLE_SIZE]) | If [N]+ new data points change proportion by >[THRESHOLD]% |
| V-010 | [SECOND_STATISTIC] | [VALUE] | Author's [DATA_SOURCE] | Same trigger |

> **Note:** Author-derived statistics are presented in the manuscript as personal data,
> not universal facts: "In my [EXPERIENCE_TYPE]..." not "Research shows..."

**Last verified:** [DATE] ✓

---

### Category 5: Tool and Software References (if applicable)

| ID | Fact | Canonical Value | Source | Recheck Trigger |
|----|------|-----------------|--------|-----------------|
| V-011 | [TOOL_OR_SOFTWARE_VERSION] | [VERSION_OR_SPEC] | [SOURCE] | Annual check; [WHAT_CHANGES] |

> **Caution:** Avoid citing specific app versions in chapters — apps update faster than books.
> Cite tool categories and features, not version numbers, in main text.

**Last verified:** [DATE] ✓

---

### Category 6: Competitive Claims

| ID | Fact | Source Reference | Issue | Recheck Trigger |
|----|------|------------------|-------|-----------------|
| V-012 | [COMPETITIVE_CLAIM — e.g., "This book is the only X that does Y"] | Doc 01 unique value claim | Must remain accurate | Before each edition: verify claim is still accurate |

> **Action if any competitive claim becomes false:** Revise the relevant section of Doc 01.
> The book's value can still stand, but the framing must be updated.

**Last verified:** [DATE] ✓

---

## Recheck Cycle

| Trigger | Action |
|---------|--------|
| New edition or major revision | Full VFR audit (all items) |
| 12 months since last check | Spot-check Category 5 (tools) and Category 6 (competitive) |
| New research or industry standard publication | Check relevant category items |
| Author generates [N]+ new data points | Check Category 4 statistics |

---

*Doc Version: 1.0 | Flavor: Topic | Phase: 1 (Pending)*
