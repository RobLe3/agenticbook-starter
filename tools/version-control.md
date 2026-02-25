# Version Control — Git Setup for Book Projects

> **Verified:** February 2026 (repo tag v0.6.0)

---

## Why Version Control for Books

The methodology uses git for two specific purposes:

1. **Safe experimentation:** Commit before a major revision pass. If the pass makes things worse, you can revert to the previous commit without losing work.
2. **Meaningful milestones:** Each commit marks a coherent state — world model complete, Chapter 3 first draft, revision pass 2 — not individual file saves.

You are not required to learn advanced git. You need five commands.

---

## The Five Commands You Actually Use

```bash
git status          # What has changed since last commit?
git add [files]     # Stage specific files for the next commit
git commit -m "..."  # Record a milestone with a message
git log --oneline   # See your commit history
git diff [commit]   # See what changed since that commit
```

---

## Initial Setup

```bash
# Install git (if not already installed):
# macOS: git is included with Xcode Command Line Tools
# Linux: sudo apt-get install git
# Windows: git-scm.com/download/win

# Configure your identity (required for commits):
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

---

## Project Setup

```bash
cd ~/my-book-project

# Initialize git:
git init

# Create a .gitignore file:
cat > .gitignore << 'EOF'
# Build artifacts
output/
archive/
*.pdf
*.epub

# LaTeX build files
*.aux
*.log
*.fdb_latexmk
*.fls
*.synctex.gz
*.toc
*.out

# System files
.DS_Store
Thumbs.db

# Secrets (never commit these)
.env
*_secret*
*_credentials*
EOF

# Stage and commit the world model:
git add docs/ CLAUDE.md MEMORY.md
git commit -m "Initial world model — Phase 1 complete"
```

---

## Commit Discipline for Books

Commit at **meaningful milestones**, not at every file save.

| When to commit | Example message |
|----------------|----------------|
| World model doc complete | `docs: complete Doc 03 book architecture` |
| Chapter first draft | `ch04: first draft complete (3,200 words)` |
| After a verification pass | `verify: CFR pass — 3 issues resolved` |
| After a revision pass | `revision: Pass 2 complete (score: 7.4 calibrated)` |
| Before a major experiment | `snapshot: pre-restructure state` |
| After a build validates | `build: v0.3.2 — 147 pages, 0 errors` |

Do not commit partial work (a half-written chapter, a note to yourself). Each commit should be a state you could return to.

---

## Safe Experimentation Protocol

Before any major revision pass:

```bash
# 1. Commit current state:
git add docs/ manuscript/
git commit -m "snapshot: pre-[revision name] state"

# 2. Run the revision pass.

# 3a. If the pass improved the work:
git add docs/ manuscript/
git commit -m "revision: [pass name] — [result]"

# 3b. If the pass made things worse:
git log --oneline  # Find the snapshot commit hash
git diff [snapshot-hash]  # Review what changed
# Then either selectively restore files or fully revert:
git checkout [snapshot-hash] -- manuscript/ch05.tex
```

---

## What NOT to Commit

- **PDF and EPUB files:** Generated output; rebuild from source. Large binaries bloat the repo.
- **API keys or credentials:** Never. Add them to `.gitignore` immediately.
- **Work in progress that cannot compile:** Only commit states that build cleanly (for LaTeX projects).
- **Every individual file change:** Commit coherent sets of work.

---

## Remote Backup (Optional but Recommended)

```bash
# Create a private repository on GitHub or GitLab
# (Your manuscript is your intellectual property — use a private repo)

git remote add origin git@github.com:yourusername/your-book.git
git push -u origin main
```

Push after each major milestone commit, not after every commit.
