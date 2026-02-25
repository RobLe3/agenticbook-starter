# Claude Code — Tier 2 Setup Guide

> **Verified:** February 2026 (repo tag v0.6.0)
> Claude Code is the Tier 2 tool used throughout *Agentic Book Writing: The Smart Way*.

---

## What Claude Code Does

Claude Code is a command-line interface to Claude that runs in your terminal and operates as an agent: it can read files, write files, run bash commands, and maintain session context through MEMORY.md. Unlike a chat interface, it operates within your project directory — your world model files and manuscript files are accessible to it directly.

The key difference from a chat interface:
- **Chat interface (Tier 1):** You copy and paste world model content into every prompt manually.
- **Claude Code (Tier 2):** The agent reads your world model files directly — once per session, not once per prompt.

---

## Prerequisites

- **macOS, Linux, or Windows (WSL):** Claude Code requires a Unix-like terminal.
- **Node.js 18+:** Required to install Claude Code via npm.
- **An Anthropic account:** Required for API access.

---

## Installation

```bash
# Install Node.js first if not already installed (nodejs.org)
# Then install Claude Code:
npm install -g @anthropic-ai/claude-code

# Verify installation:
claude --version
```

**First run — authentication:**
```bash
claude
# Claude Code will prompt for your Anthropic API key on first run.
# Your key is stored locally; you will not need to re-enter it.
```

---

## Key Settings for Book Writing

Three files control Claude Code's behavior in a book project:

| File | Purpose | Location |
|------|---------|----------|
| `CLAUDE.md` | Agent instruction file: reading order, writing rules, DO/DO NOT rules | Project root |
| `MEMORY.md` | Accumulated project knowledge: current phase, key decisions, conventions | Project root |
| `handover.md` (optional) | Session-end state transfer: what was completed, what is next | Project root |

**Claude Code reads `CLAUDE.md` automatically at the start of every session.** This is why the methodology requires CLAUDE.md to be complete before the first writing session — the agent's behavior is determined by what is in that file.

---

## Starting a Writing Session

```bash
cd ~/my-book-project
claude
# The agent reads CLAUDE.md and MEMORY.md automatically.
# Begin with: "Continue from MEMORY.md" or
# "Read docs/00_index.md and tell me what's ready to work on next."
```

**Session start discipline:**
1. Claude Code reads CLAUDE.md (agent rules)
2. You tell it to read MEMORY.md (current state)
3. You tell it which world model docs to load for this session's work
4. You begin generating or revising

Do not skip step 2 — MEMORY.md is what prevents context re-explanation overhead.

---

## Permission Modes

Claude Code asks for permission before executing commands. For book writing:

| Action | Recommended setting |
|--------|---------------------|
| Reading files | Auto-allow (agent needs this constantly) |
| Writing to `docs/` and `manuscript/` | Auto-allow for your project directory |
| Running `build.sh` or stats scripts | Approve manually (confirm each run) |
| Installing packages or running network commands | Approve manually (uncommon; require explicit authorization) |

---

## When to Use Tier 2 vs. Tier 1

| Scenario | Tier |
|----------|------|
| Single-prompt generation tasks | Tier 1 (copy context, paste output) |
| Reading multiple world model files per session | Tier 2 |
| Writing output directly to manuscript files | Tier 2 |
| Running build scripts (`build.sh`, stats) | Tier 2 |
| Maintaining state across a multi-hour session | Tier 2 |
| Multi-agent coordination, recurring pipelines | Tier 3 |

---

## Verification Test (Confirm Your Setup Works)

```bash
cd ~/my-book-project
claude
# In the Claude Code session, ask:
# "Read MEMORY.md and tell me the current project phase and next action."
# If the agent reads the file and answers correctly, your Tier 2 setup works.
```

If the agent cannot find MEMORY.md or answers generically, check:
1. You are in the correct directory (`pwd` to verify)
2. MEMORY.md exists in the current directory (`ls MEMORY.md`)
3. MEMORY.md has content (not empty)
