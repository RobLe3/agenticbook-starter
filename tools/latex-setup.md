# XeLaTeX Setup — Novel-Flavor Build Guide

> **Verified:** February 2026 (repo tag v0.6.0)
> Novel-flavor projects use XeLaTeX as the manuscript compiler.
> Short and Topic-flavor projects use Pandoc — see `markdown-setup.md`.

---

## What You Need

| Tool | Purpose |
|------|---------|
| XeLaTeX | Compiler (part of a TeX distribution) |
| Pandoc | Optional: convert Markdown source to LaTeX before compiling |
| pdffonts | Font embedding verification (part of poppler-utils) |
| epubcheck | EPUB validation (Java required) |

---

## macOS Installation

**Option A: MacTeX (full installation, recommended)**
```bash
# Download MacTeX from tug.org/mactex (approximately 4GB)
# Install the .pkg file — XeLaTeX is included.

# Verify:
xelatex --version
```

**Option B: BasicTeX (minimal installation, ~100MB)**
```bash
# Download BasicTeX from tug.org/mactex/morepackages.html
# After install, add missing packages as needed:
sudo tlmgr update --self
sudo tlmgr install [package-name]

# Common packages for book projects:
sudo tlmgr install memoir libertinus-otf sourcesanspro \
  inconsolata tcolorbox fontawesome5 pgf xcolor \
  mdframed enumitem microtype setspace
```

---

## Linux Installation (Ubuntu/Debian)

```bash
sudo apt-get install texlive-xetex texlive-fonts-extra \
  texlive-latex-extra poppler-utils

# Verify:
xelatex --version
```

---

## Windows Installation

Install MiKTeX from miktex.org. MiKTeX auto-installs missing packages on first compile. After installation, run the MiKTeX Console to update packages.

For command-line use, install WSL (Windows Subsystem for Linux) and follow the Linux instructions above.

---

## Compiling a Book Project

```bash
cd ~/my-book-project/manuscript

# First compile (generates .aux files):
xelatex main.tex

# Second compile (resolves cross-references):
xelatex main.tex

# Third compile (resolves any remaining references):
xelatex main.tex

# Or use latexmk for automatic compilation:
latexmk -xelatex main.tex
```

**Expected output:** `main.pdf` in your manuscript directory.

---

## Common Error Messages

| Error | Likely cause | Fix |
|-------|-------------|-----|
| `! LaTeX Error: File 'memoir.cls' not found.` | memoir class not installed | `sudo tlmgr install memoir` |
| `! Font ... not found.` | Font not installed on system | Install the font, or check `\setmainfont{}` in preamble |
| `! Undefined control sequence.` | Typo in a LaTeX command or missing package | Check the specific command name; add missing package to preamble |
| `! Package fontspec Error` | Font not found by XeLaTeX | Verify font name with `fc-list | grep [font-name]` |
| Infinite compile loop | Circular cross-reference | Run `latexmk -xelatex main.tex` instead; it resolves automatically |

---

## Font Embedding Verification (Before Print Submission)

```bash
pdffonts output/manuscript.pdf
# All fonts should show "yes" in the Emb column.
# If any font shows "no", the PDF will be rejected by print-on-demand services.
```

---

## Build Script Template

```bash
#!/bin/bash
# build.sh — Run from project root
cd manuscript/

echo "=== Building manuscript ==="
xelatex -interaction=nonstopmode main.tex > /dev/null 2>&1
xelatex -interaction=nonstopmode main.tex > /dev/null 2>&1

# Check for errors:
if grep -q "^!" main.log; then
    echo "BUILD FAILED — errors in main.log"
    grep "^!" main.log
    exit 1
fi

# Get page count:
PAGES=$(grep "Output written" main.log | grep -o "[0-9]* page" | grep -o "[0-9]*")
echo "Build complete: $PAGES pages"
cp main.pdf ../output/manuscript_$(date +%Y%m%d).pdf
```

Make executable: `chmod +x build.sh`
