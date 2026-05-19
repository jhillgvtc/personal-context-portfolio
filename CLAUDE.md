# Personal Context Portfolio

Structured set of 10 markdown files that describe who John is, how he works, and what he prefers. Portable across any AI system.

## Structure

```
portfolio/
  identity.md              -- Who I am, one-paragraph intro
  role-and-responsibilities.md  -- How I spend time, what I own
  current-projects.md      -- Active initiatives and status
  team-and-relationships.md -- Key people and interaction patterns
  tools-and-systems.md     -- Daily tools, data sources, integrations
  communication-style.md   -- Writing voice, audience adaptations, banned phrases
  goals-and-priorities.md  -- Near-term priorities, career goals, anti-goals
  preferences-and-constraints.md -- Schedule, strong opinions, frustrations
  domain-knowledge.md      -- Telco expertise, mental models, learning areas
  decision-log.md          -- How I decide, recent examples, self-awareness
wiring/
  integration-guide.md     -- How to load portfolio into AI tools
```

## Maintenance

- Run `REFRESH-PLAYBOOK.md` at root every other Monday — 15-min checklist that walks the state files and pushes the diff.
- `now.md` is the weekly state file — refresh every Monday (5 min).
- `current-projects.md`, `goals-and-priorities.md`, `team-and-relationships.md`, `tools-and-systems.md` are biweekly state files.
- `decision-log.md`, `identity.md`, `role-and-responsibilities.md`, `communication-style.md`, `preferences-and-constraints.md`, `domain-knowledge.md` are pattern files — quarterly scan.
- `identity.md` stays in sync with `~/.claude/IDENTITY.md` (source of truth is Obsidian vault).
- `communication-style.md` stays in sync with `~/.claude/writing-style/voice-dna.md`.
- `decision-log.md` is append-only — add entries after significant decisions.

## Key Principle

Be specific, not aspirational. These files describe how John actually works, not how he wishes he worked.
