# prompts/ — Static Prompt Library

Six-stage prompt library for the Static Prompt Bootstrap (Phase 0) — generating book chapters without a world model infrastructure, using a chatbot and copy-paste.

## When to use these

**Phase 0 (before world model):** Use stages 1–2 to generate first-draft chapters with any chatbot (Claude.ai, ChatGPT, Gemini). No installation required.

**World model projects:** Use stages 3–4 as supplements after Chapter 9 (First Draft Generation) and Chapter 10 (Measurement). The prompts work alongside your world model docs — paste your docs into the context slots instead of writing the context inline.

## Stage order

| File | Stage | Prompts | Use When |
|------|-------|---------|----------|
| `stage-1-concept.md` | Concept Development | STRUO, ANALY, COMPR | Before writing — build the concept and chapter structure |
| `stage-2-writing.md` | Writing | CHDD, CHFO, SUBREF | Generating chapter prose |
| `stage-3-refinement.md` | Refinement | COREF, STRAL, COMAC, CAM | After 3+ chapters drafted — consistency and voice checks |
| `stage-4-review.md` | Review + Scoring | AASS, DARE, IRIN | Quality scoring and targeted revision |
| `stage-5-illustration.md` | Illustration | COMAC (visual), visual briefs | When chapters include figures, diagrams, or photo prompts |
| `stage-6-supplemental.md` | Supplemental | Back matter, author bio, metadata | Final pre-publication content |

## Calibration reminder

Apply **×0.85** to all AI quality scores from Stages 3–4. Apply **×0.80** to AASS scores specifically (static-prompt self-assessment inflates more than world-model-grounded review). Never treat a single scoring pass as a final determination.

## Source

These prompts are the markdown version of Appendix D (Static Prompt Library) from *Agentic Book Writing: The Smart Way*. The book version contains the full source corpus (Book-in-Book section). If this file and the book diverge, the book takes precedence.
