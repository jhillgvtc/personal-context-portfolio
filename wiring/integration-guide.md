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
      "C:/Users/john.hill/Claude-Projects/personal-context-portfolio/portfolio"
    ]
  }
}
```

Then any MCP-compatible tool can read individual portfolio files on demand.

## System Prompts (Custom Agents)

For agents like Atlas/OpenClaw, include relevant portfolio sections in the agent's identity or system prompt. The identity.md and communication-style.md files are the most universally useful.

## Keeping It Fresh

| File | Review Cadence | Trigger |
|------|---------------|---------|
| current-projects.md | Monthly | When projects start/complete |
| goals-and-priorities.md | Quarterly | At quarter boundaries |
| team-and-relationships.md | As needed | When org changes happen |
| decision-log.md | As needed | After significant decisions |
| Everything else | Quarterly | Quick scan for accuracy |

Run `/compile-identity` to refresh identity.md from the Obsidian vault source of truth.
