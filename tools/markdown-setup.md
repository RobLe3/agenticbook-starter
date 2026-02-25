# Pandoc Setup — Short and Topic Flavor Build Guide

> **Verified:** February 2026 (repo tag v0.6.0)
> Short and Topic-flavor projects use Markdown as the primary source format, compiled by Pandoc.
> Novel-flavor projects use XeLaTeX — see `latex-setup.md`.

---

## What You Need

| Tool | Purpose |
|------|---------|
| Pandoc | Markdown → PDF / EPUB / DOCX compiler |
| wkhtmltopdf | PDF engine for Pandoc (via `--pdf-engine=wkhtmltopdf`) — optional |
| LaTeX | Required for PDF output via Pandoc's default `pdflatex` engine |
| epubcheck | EPUB validation after export (Java required) |

---

## macOS Installation

```bash
# Install via Homebrew (recommended):
brew install pandoc

# Optional: install LaTeX for PDF output
# (BasicTeX is sufficient — see latex-setup.md)

# Verify:
pandoc --version
```

---

## Linux Installation (Ubuntu/Debian)

```bash
sudo apt-get install pandoc

# For PDF output, you also need a LaTeX engine:
sudo apt-get install texlive-latex-base texlive-xetex

# Verify:
pandoc --version
```

---

## Windows Installation

Download the installer from pandoc.org/installing.html. Run the .msi file. Pandoc will be available in PowerShell or Command Prompt.

For PDF output, install MiKTeX from miktex.org.

---

## Compile Commands

### PDF (print layout)

```bash
pandoc manuscript.md \
  --pdf-engine=xelatex \
  --metadata title="Your Book Title" \
  --metadata author="Your Name" \
  --variable geometry:margin=1in \
  --variable fontsize=11pt \
  --variable mainfont="Libertinus Serif" \
  -o output/manuscript.pdf
```

### EPUB (ebook)

```bash
pandoc manuscript.md \
  --metadata title="Your Book Title" \
  --metadata author="Your Name" \
  --metadata lang="en-US" \
  --epub-cover-image=cover.jpg \
  -o output/manuscript.epub
```

### DOCX (Word, for editor submissions)

```bash
pandoc manuscript.md \
  --metadata title="Your Book Title" \
  -o output/manuscript.docx
```

---

## Metadata File (Recommended)

Instead of passing `--metadata` flags on every compile, create a `metadata.yaml` file in your project root:

```yaml
---
title: "Your Book Title"
subtitle: "Your Subtitle"
author: "Your Name"
date: "2026"
lang: "en-US"
description: |
  One-paragraph description of the book.
subject: "Photography"
rights: "© 2026 Your Name. All rights reserved."
---
```

Then compile with:
```bash
pandoc metadata.yaml manuscript.md --pdf-engine=xelatex -o output/manuscript.pdf
```

---

## EPUB Validation

```bash
# After generating the EPUB, validate it:
epubcheck output/manuscript.epub

# All output should be: No errors or warnings detected
# Any CRITICAL or ERROR results must be fixed before submission to retailers.
```

---

## Multi-Chapter Projects

For books with separate chapter files, create a `build.sh` that concatenates them:

```bash
#!/bin/bash
# build.sh — Run from project root
echo "=== Building manuscript ==="

# Concatenate chapters in order:
cat manuscript/introduction.md \
    manuscript/ch01.md \
    manuscript/ch02.md \
    manuscript/ch03.md \
    > manuscript/combined.md

# Build PDF:
pandoc metadata.yaml manuscript/combined.md \
  --pdf-engine=xelatex \
  --variable geometry:margin=1in \
  -o output/manuscript.pdf

echo "Build complete: output/manuscript.pdf"
```

---

## Common Issues

| Issue | Likely cause | Fix |
|-------|-------------|-----|
| `pdflatex not found` | LaTeX not installed | Install TeX distribution (see `latex-setup.md`) |
| Font not found in PDF output | Font not installed on system | Use a system font name or install the font |
| EPUB validation errors | Malformed metadata or missing cover | Verify metadata.yaml fields; ensure cover image is JPEG |
| Tables not rendering in PDF | Complex Markdown table | Simplify table or use `--variable tables=true` |
