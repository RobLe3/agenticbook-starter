# Stage 5: Illustration

> Prompts: **Visual Brief** (figure and diagram specification) | **COMAC-Visual** (visual accessibility check) | **Caption Generator**
>
> Stage 5 applies to chapters with figures, diagrams, photographs, or any visual element.
> For text-only chapters, skip this stage.
>
> **World model equivalent:** In a world model project, visual elements are specified in
> the architecture doc (Doc 03) alongside the chapter outline — what goes where, what it
> illustrates, and what caption it needs. Stage 5 does this inline per chapter.

---

## Visual Brief — Figure Specification

**Use when:** Planning which visual elements a chapter needs before writing (or after, to spec visuals for an existing draft).

```
Generate visual element specifications for this chapter.

Chapter: "[CHAPTER TITLE]"
Chapter intent: [what reader should be able to do after reading]
Target reader: [knowledge level]

For each concept in this chapter that would benefit from
a visual:

1. VISUAL TYPE: [diagram / photograph / chart / screenshot /
   step-sequence / comparison table]
2. WHAT IT SHOWS: [specific content — not "a diagram of X"
   but "a diagram showing how ISO, shutter speed, and aperture
   interact in the exposure triangle, with values for a
   typical night sky shot at ISO 3200"]
3. WHERE IT APPEARS: [after which paragraph or section]
4. CAPTION: [one sentence — what the reader should notice]
5. ALTERNATIVE TEXT: [for accessibility — what is depicted
   for a reader who cannot see the image]

Also: flag any concept where a visual would replace 200+
words of explanation more effectively than prose.
```

---

## COMAC-Visual — Visual Accessibility Check

**Use when:** After adding visuals to a chapter — verify they are accessible and necessary.

```
Review the visual elements in this chapter.

For each figure, diagram, or image in this chapter:

[DESCRIBE EACH VISUAL — what it shows, its caption,
its position in the chapter]

Check for:
1. NECESSITY: does this visual replace explanation that
   prose cannot do as well, or is it decorative?
2. SELF-CONTAINED: can the visual be understood without
   reading surrounding text? (It should be.)
3. CAPTION ACCURACY: does the caption direct the reader
   to what they should notice?
4. ACCESSIBILITY: is there sufficient alt-text or
   descriptive prose for readers who cannot see the image?
5. INTRODUCTION: is the visual introduced in the preceding
   paragraph? (Never present a figure without a lead sentence.)

For each: [KEEP / REVISE / REMOVE] — [reason]
```

---

## Caption Generator

**Use when:** You have a visual but need a concise, accurate caption.

```
Write a caption for this visual element.

Visual type: [diagram / photograph / chart / screenshot]
Visual content: [describe specifically what is depicted —
  include any labels, values, or data points visible]
Chapter context: [what the surrounding text is discussing]
Target reader: [knowledge level]

Generate:
1. SHORT CAPTION (1 sentence, <20 words): what the visual
   shows and what the reader should notice
2. EXTENDED CAPTION (2-3 sentences, optional): if the visual
   requires context to interpret correctly, add 1-2 sentences
   of explanation after the core caption.

Do not begin the caption with "This figure shows..." or
"The diagram above..." — start with the specific content.
```
