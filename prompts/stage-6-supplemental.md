# Stage 6: Supplemental

> Prompts: **Author Bio** | **Colophon / Technical Notes** | **Acknowledgements** | **Back Cover Blurb** | **Metadata Block**
>
> Stage 6 generates the supporting materials around the manuscript — the content that
> appears before and after the main text, plus platform metadata for publication.
>
> Run Stage 6 after the manuscript is content-complete and quality-gated.
> These materials should not be drafted during early revision cycles — they will
> need to be rewritten if the book's scope or thesis changes.
>
> **Note:** Every prompt below has a slot for your real credentials. Do not let the AI
> invent biographical details. Provide the facts; the AI shapes them into the right format.

---

## Author Bio Generator

**Use when:** Final pre-publication stage. One pass to generate; one pass to verify facts.

```
Write an author bio for this book.

Author details (facts only — do not invent):
- Name: [YOUR NAME]
- Professional background: [Relevant experience — 2-3 specific facts]
- Credentials for this specific topic: [What qualifies you to write this book]
- Any published works, public projects, or recognized work: [Specific titles or projects]
- Location (if relevant to the book's topic): [Optional]
- Contact or website: [Optional]

Book: [TITLE]
Flavor: [Short / Topic / Novel]
Platform: [print back matter / Amazon author page / press kit]

Generate:
1. SHORT BIO (50-75 words): For the book's back cover
2. MEDIUM BIO (100-150 words): For Amazon or platform author pages
3. PRESS BIO (200-250 words): For press kits and media inquiries

Do not invent credentials, awards, or experiences not listed above.
Flag any statement that cannot be verified from the facts provided.
```

---

## Colophon / Technical Notes

**Use when:** Print or PDF production. The colophon records the tools and decisions used to produce the book.

```
Generate a colophon for this book.

Production details:
- Source format: [Markdown / LaTeX / Word / other]
- Compiled with: [Pandoc / XeLaTeX / other — include version]
- Fonts: [Body font, heading font, code font if applicable]
- Page size: [e.g., 6×9 in / A5 / Crown Quarto]
- AI tools used: [Claude / ChatGPT / other — include role]
- Date: [Publication date or "First edition, [Month Year]"]

Generate:
1. BRIEF COLOPHON (2-3 sentences): suitable for the copyright page
2. EXTENDED COLOPHON (1 short paragraph): suitable for a "Production Notes"
   page if the process is part of the book's subject matter

Flag any technical claim (software version, font name) that should
be verified before printing.
```

---

## Acknowledgements

**Use when:** After manuscript is complete. Acknowledgements should name real people who contributed.

```
Draft acknowledgements for this book.

People to acknowledge (facts only):
- [Name] — [How they contributed or supported the project]
- [Name] — [How they contributed]
[List everyone; the AI will organize them appropriately]

Tone: [FORMAL / CONVERSATIONAL / WARM]
Length: [SHORT (1 paragraph) / STANDARD (3-4 paragraphs) / EXTENDED]

Generate acknowledgements that:
1. Thank contributors in a logical order (close collaborators, then broader support)
2. Are specific — "for reading the manuscript and catching inconsistencies in Chapter 4"
   not "for their support"
3. Do not thank AI tools in the same register as human contributors
4. End with a brief note about who the book is dedicated to, if applicable

Do not invent names or contributions not provided above.
```

---

## Back Cover Blurb

**Use when:** Preparing the final book file for print or platform upload.

```
Write a back cover blurb for this book.

Book details:
- Title: [TITLE]
- Premise: [2 sentences from STRUO or Doc 01]
- Target reader: [Who picks this up and why]
- What changes for the reader: [The transformation promise]
- Unique angle: [What makes this different from similar books]

Generate:
1. SHORT BLURB (75-100 words): hook + promise + call to action
2. STANDARD BLURB (150-200 words): hook + problem + solution + transformation + CTA
3. CATEGORY LINE: one sentence for the back cover positioning text
   (e.g., "Photography · Night Sky · Beginner's Guide")

The hook must not begin with a question ("Are you tired of...") or
"Discover how..." — start with a specific, concrete observation.
```

---

## Metadata Block

**Use when:** Preparing for platform upload (Amazon KDP, IngramSpark, Draft2Digital, etc.).

```
Generate the metadata block for platform upload.

Book details:
- Title: [TITLE]
- Subtitle: [SUBTITLE or "none"]
- Author: [YOUR NAME]
- Language: [English / other]
- Primary category: [e.g., Photography > Night Photography]
- Secondary category: [e.g., Astronomy > Amateur Astronomy]
- Keywords (what readers search for): [List 5-10 search terms
  your target reader would actually use]
- Target age: [All ages / Adult / Young Adult]
- Content warnings: [None / Violence / Language / etc.]
- Publication date: [Date or "TBD"]
- ISBN: [If assigned, or "pending"]

Generate:
1. TITLE ENTRY: formatted for platform metadata field
2. SUBTITLE ENTRY: formatted for platform metadata field
3. KEYWORDS LIST: 7 optimized keywords for primary platform
4. CATEGORY PATH: full category path for primary platform
5. SHORT DESCRIPTION (150 words max): for platform product page
6. LONG DESCRIPTION (300-400 words): full platform product page copy

Flag any keyword that is too competitive to rank for or too obscure
to drive traffic — suggest alternatives.
```
