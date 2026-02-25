# Doc 06: Verification Lite — First Light

> **Example world model doc for *Agentic Book Writing: The Smart Way* — Chapter 7.**
> This document provides a minimal verification gate for a Short-flavor project.
> It is not the full production verification stack.
>
> **Note for agent:** Run a CFR-Lite pass after every two chapters. Run a full Verification pass
> before each revision cycle. Run the complete starter pass before release.

---

## What This Covers

1. **CFR-Lite:** Consistency of key facts, key terms, and fixed claims across chapters
2. **Basic Consistency:** Internal contradictions within and across chapters
3. **Cross-Reference Check:** Broken chapter/section/figure pointers

---

## When To Run

- After every two new chapter drafts (CFR-Lite pass — 15 minutes)
- Before each revision cycle (Basic Consistency pass — 30 minutes)
- Before release/export (full starter pass — 45 minutes)

---

## CFR-Lite Check

Track only critical invariants — the facts that, if inconsistent, break the reader's trust. *First Light* invariants:

| Item | Canon Value | Last Checked | Status | Fix Needed |
|------|-------------|-------------|--------|-----------|
| Book's gear progression start | Smartphone (Ch 1) | 2026-02 | PASS | — |
| Book's gear progression end | DSLR (Ch 7) | 2026-02 | PASS | — |
| Telescope scope rule | Explicitly out of scope | 2026-02 | PASS | — |
| Word count target | 22,000–28,000 words | 2026-02 | PASS | — |
| Chapters + Introduction | 7 chapters + Introduction = 8 total | 2026-02 | PASS | — |
| Chapter lab output requirement | Every chapter produces one photograph | 2026-02 | PASS | — |
| Urban-first assumption | Light-polluted environment assumed in Ch 1–3 | — | UNVERIFIED | Check Ch 1–3 drafts |
| ISO definition (first use) | "sensitivity setting that determines how your sensor responds to light" | — | UNVERIFIED | Check Ch 1 or 2 draft |
| Shutter speed definition (first use) | Duration the sensor is exposed to light | — | UNVERIFIED | Check Ch 1 draft |
| Milky Way core visibility | Seasonal — best May–October in Northern Hemisphere | — | UNVERIFIED | Check Ch 6 draft + `[VERIFY]` tag |

> **Rule:** If any row shows FAIL, fix the source-of-truth doc first, then fix the chapter prose.
> Do not fix chapter prose without updating the source doc.

---

## Basic Consistency Check

After each revision pass, confirm:

- [ ] "World model" or "methodology" terms not slipping into chapters where they don't belong (this is a photography guide, not a writing guide)
- [ ] Gear level is consistent within each chapter (smartphone chapters don't mention DSLR settings)
- [ ] Chapter summary claims match what the chapter body actually teaches
- [ ] Terminology is consistent: "aperture" not "f-stop" in some chapters and "aperture" in others (pick one; define it in Doc 04)
- [ ] The "one skill per chapter" rule is not violated (no chapter teaches two new skills)

Issue log:

| # | Location | Issue | Severity | Fix |
|---|----------|-------|----------|-----|
| — | — | No issues logged yet | — | — |

---

## Cross-Reference Check

Before release, scan for internal references:

- [ ] "In Chapter N..." — verify Chapter N exists and covers the referenced topic
- [ ] "As described earlier..." — verify the earlier section exists
- [ ] "See the appendix..." — verify appendix exists (if applicable)
- [ ] Technique names are consistent (e.g., "500 rule" appears with the same name in Ch 2 and Ch 4)

---

## Release Decision (Starter Gate)

- **GREEN:** No HIGH issues; all CFR-Lite critical invariants PASS
- **YELLOW:** 1–2 unresolved MED issues (release only if low risk)
- **RED:** Any HIGH issue unresolved — do not release

Current status: UNVERIFIED (manuscript not yet drafted)
