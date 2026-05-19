# Integration Guide

How to load the portfolio into different AI tools and contexts.

## Claude Code (Already Wired)

The portfolio lives alongside existing Claude Code configuration. Key files already feed into Claude Code sessions:

| Portfolio File | Existing Claude Code Source |
|---|---|
| identity.md | `~/.claude/IDENTITY.md` (auto-loaded) |
| communication-style.md | `~/.claude/writing-style/voice-dna.md` (loaded via writing-content.md rule) |
| preferences-and-constraints.md | `~/.claude/working-preferences.md` (auto-injected at session start) |
| domain-knowledge.md | CLAUDE.md domain terms section (auto-loaded) |

To load additional portfolio files into a Claude Code session, reference them in a project CLAUDE.md or read them at session start.

## Claude Projects (claude.ai)

Upload 2-4 files that match the use case. Don't upload all 10 -- irrelevant context dilutes useful context.

**Recommended bundles:**

| Use Case | Files to Upload |
|----------|----------------|
| General work assistant | identity, role-and-responsibilities, communication-style, preferences-and-constraints |
| Writing assistant | identity, communication-style, domain-knowledge |
| Data analysis | identity, role-and-responsibilities, tools-and-systems, domain-knowledge |
| Meeting prep | identity, team-and-relationships, current-projects |
| Strategic advisor | identity, goals-and-priorities, decision-log, current-projects |
| Career coaching | identity, goals-and-priorities, decision-log, preferences-and-constraints |

## ChatGPT / Other AI Tools

Same approach as Claude Projects. Copy the relevant files into the system prompt or custom instructions. Most tools have context limits, so pick 2-4 files max.

## MCP Resource (Advanced)

Point a filesystem MCP server at the `portfolio/` directory to make all files available as MCP resources:

```json
{
  "filesystem": {
    "command": "cmd",
    "args": ["/c", "npx", "-y", "@anthropic-ai/mcp-filesystem"],
    "env": {},
    "allowedDirectories": [
      "C:/Users/john.hill/Claude-Projects/3-resources/personal-context/portfolio"
    ]
  }
}
```

Then any MCP-compatible tool can read individual portfolio files on demand.

## System Prompts (Custom Agents)

For agents like Atlas/OpenClaw, include relevant portfolio sections in the agent's identity or system prompt. The identity.md and communication-style.md files are the most universally useful.

## Keeping It Fresh

The state vs pattern split (from the 5/7 decision-log entry): state-heavy files decay in 2-3 weeks, pattern-heavy files hold for a quarter.

| File | Type | Review Cadence | Trigger |
|------|------|---------------|---------|
| now.md | State | Weekly (Monday) | Always |
| current-projects.md | State | Biweekly | Projects start/complete |
| goals-and-priorities.md | State | Biweekly | Quarter boundaries |
| team-and-relationships.md | State | Biweekly | Org changes |
| tools-and-systems.md | State | Biweekly | New MCP / tool retirement |
| decision-log.md | Pattern | Append-only | After significant decisions |
| identity.md | Pattern | Quarterly | Life events |
| role-and-responsibilities.md | Pattern | Quarterly | Role/title change |
| communication-style.md | Pattern | Quarterly | New voice rule |
| preferences-and-constraints.md | Pattern | Quarterly | Schedule change |
| domain-knowledge.md | Pattern | Quarterly | New domain |

**Refresh ritual:** run `REFRESH-PLAYBOOK.md` at the personal-context root every other Monday. 15-min checklist that walks the state files and commits + pushes the diff to `github.com/jhillgvtc/personal-context-portfolio`.

Run `/compile-identity` to refresh identity.md from the Obsidian vault source of truth.
