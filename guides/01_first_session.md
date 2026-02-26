# First Session (60-120 Minutes)

This is the fastest clean on-ramp from "blank project" to "first controlled output".

## 1. Clone and orient

```bash
git clone https://github.com/RobLe3/agenticbook-starter.git starter
cd starter
```

Read in this order:

1. [`../README.md`](../README.md)
2. [`00_reader_routes.md`](00_reader_routes.md)
3. your flavor card in [`../quickstart/`](../quickstart/README.md)

## 2. Choose flavor and copy blanks

- Short -> copy from [`../blank/`](../blank/)
- Topic -> copy from [`../topic-blank/`](../topic-blank/)
- Novel -> copy from [`../novel-blank/`](../novel-blank/)

## 3. Fill minimum docs before generation

Short minimum:
- index/concept/readers/architecture/glossary/case study

Topic minimum:
- content docs + style guide + canon rules

Novel minimum:
- premise + character/location + architecture + style/canon

## 4. Generate first controlled chapter

Use the prompt library:

- concept pass: [`../prompts/stage-1-concept.md`](../prompts/stage-1-concept.md)
- writing pass: [`../prompts/stage-2-writing.md`](../prompts/stage-2-writing.md)

## 5. Verify before continuing

- review pass: [`../prompts/stage-4-review.md`](../prompts/stage-4-review.md)
- short verification docs: [`../docs/06_verification_lite.md`](../docs/06_verification_lite.md), [`../docs/07_vfr_lite.md`](../docs/07_vfr_lite.md)

Do not continue chapter-by-chapter if contradictions already appear. Expand model first.

## 6. End-of-session checkpoint

Before ending session:

- update `MEMORY.md`
- record one next action
- mark unresolved verification flags
