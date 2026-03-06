<!--
Book reference: This example supports Lab 7 (Chapter 7: Verification).
If you completed Lab 7, compare your VFR to this one.
Differences are expected — this is a different project (Short-flavor, photography guide).
Look for: volatile claim identification, recheck trigger specificity, register scope discipline.
-->

# Doc 07: VFR Lite — First Light

> **Example world model doc for *Agentic Book Writing: The Smart Way* — Chapter 7.**
> Track volatile claims that can become outdated before publication.
> "Volatile" means: versions, prices, platform features, hardware specs, install commands.
>
> **Note for agent:** Do not assert any volatile claim without a `[VERIFY]` tag unless the
> row below shows STATUS: CURRENT. Prefer ranges and qualified wording over brittle precision
> (e.g., "around $200–400 used" rather than "$299").
> *Book Lab → Lab 7 (Chapter 7). If you completed Lab 7, compare your VFR to this one — look for: volatile claim identification, recheck trigger specificity, register scope discipline.*

---

## Volatile vs Stable

- **Stable:** conceptual statements unlikely to change (exposure triangle, 500 rule, light pollution zones)
- **Volatile:** app prices, camera prices, software versions, platform features, hardware specs

Only volatile claims belong in this register.

---

## VFR-Lite Register

| ID | Claim (exact wording in manuscript) | Chapter | Source | Last Verified | Status | Action |
|----|--------------------------------------|---------|--------|---------------|--------|--------|
| V1 | "NightCap Camera is available on the App Store" | Ch 1 | App Store listing | 2026-02 | CURRENT | None |
| V2 | "NightCap costs approximately $2.99–$5.99" | Ch 1 | App Store pricing | 2026-02 | CURRENT | Use range; verify before release |
| V3 | "Lightroom Mobile includes basic RAW editing in the free tier" | Ch 7 | Adobe product page | 2026-02 | CURRENT | Verify free tier limits before release |
| V4 | "An entry-level DSLR (used) is available for approximately $150–350" | Ch 5 | Secondhand market survey | 2026-02 | CURRENT | Use range; market fluctuates |
| V5 | "The iPhone 15 and equivalent Android flagships support RAW capture" | Ch 1 | Manufacturer specs | 2026-02 | CURRENT | Check for model-specific caveats |
| V6 | "The International Dark-Sky Association certifies dark-sky parks" | Ch 3 | IDA website | 2026-02 | CURRENT | Verify website URL before release |
| V7 | "Bortle scale runs from 1 (darkest) to 9 (brightest)" | Ch 2 | Astronomy standard | 2026-02 | CURRENT | Stable — very unlikely to change |
| V8 | "Light Pollution Map (lightpollutionmap.info) shows real-time data" | Ch 3 | Site visit | 2026-02 | CURRENT | Verify URL and feature availability before release |

---

## Claims to Avoid (Too Volatile)

- Specific camera model prices — use ranges instead
- App version numbers — refer to "current version" not "v3.2"
- Subscription prices — state approximate pricing and note "verify current pricing"
- Hardware availability — models are discontinued; refer to categories not specific models

---

## Verification Cadence

Run VFR-Lite checks:
- [ ] Before release/export — ALL rows must show CURRENT or be explicitly caveated
- [ ] After a revision gap of more than 3 months
- [ ] Before sharing externally (writing groups, beta readers)

If any row shows OUTDATED or UNVERIFIED at release time, either update the claim or add a verification date caveat in the text.

---

## Starter Policy

- Prefer ranges over point values: "around $150–350" not "$249"
- Include verification dates for specific claims: "(verified February 2026)"
- When precision is required, include both the claim and its source
- Update the manuscript and this register together — never update one without the other
