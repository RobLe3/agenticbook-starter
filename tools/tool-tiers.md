# Tool Tiers — Current Reference

> **Verified:** February 2026 (repo tag v1.0.0)
> When this table diverges from a tool's current documentation, use the tool's documentation.

---

## The Three Tiers

| Tier | Category | Reference Tool | What It Provides | Setup required |
|------|----------|----------------|-----------------|----------------|
| **Tier 1** | Chat interface | Claude.ai Pro, ChatGPT Plus, Gemini Advanced | Conversational generation; paste-and-prompt workflow | Browser only — no installation |
| **Tier 2** | Coding agent | Claude Code (Anthropic) | Reads/writes files; executes commands; persistent sessions via MEMORY.md | Terminal + npm install |
| **Tier 3** | Orchestration | API + custom scripts | Multi-agent coordination; automated sweeps; repeatable pipelines | API key + scripting environment |

---

## Tier 1 Tool Versions (February 2026)

| Tool | Plan | Context window | Best for | Pricing |
|------|------|---------------|---------|---------|
| Claude.ai Pro | $20/month | 200K tokens | General writing, verification, consistency checks | claude.ai |
| ChatGPT Plus | $20/month | 128K tokens | Prose generation, broad tasks | chat.openai.com |
| Gemini Advanced | $20/month (Google One AI Premium) | 1M+ tokens | Very long context, research across many docs | gemini.google.com |

> Prices shown are representative as of February 2026 and change without notice.
> Verify current plans and pricing at each provider's official pricing page before subscribing.

---

## Tier 2 Tool Version (February 2026)

| Tool | Version | Install command | Documentation |
|------|---------|----------------|--------------|
| Claude Code | Latest (auto-updated via npm) | `npm install -g @anthropic-ai/claude-code` | See `claude-code.md` in this folder |

---

## Tier 3 Prerequisites

| Component | Purpose | Notes |
|-----------|---------|-------|
| Anthropic API key | Authenticate API calls | console.anthropic.com |
| Node.js 18+ | Runtime for API scripts | nodejs.org |
| Python 3.10+ | Alternative runtime | python.org |
| git | Version control for scripts | See `version-control.md` |

---

## Choosing Your Tier

**Start with the lowest tier that fits your current project scale.** Re-evaluate only when your workflow becomes the bottleneck.

- **Tier 1 fits** when: Short flavor, 15–20 sessions, copy-paste overhead is manageable
- **Tier 2 fits** when: Topic or Novel flavor, 30+ sessions, manual copy-paste has become the bottleneck
- **Add Tier 3** when: You are coordinating multiple agent roles, running recurring verification sweeps, or automating repetitive release checks

Graduate from Tier 1 to Tier 2 within the same project — you do not need to rebuild your world model.
