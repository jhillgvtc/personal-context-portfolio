# Refresh Playbook

15-minute biweekly Monday ritual. Walks the state files, commits the diff, pushes to `github.com/jhillgvtc/personal-context-portfolio`.

## When to run

- Every other Monday, ~8:00 AM (Todoist recurring task: "Refresh personal-context portfolio").
- Ad-hoc after any of: title change, direct-report change, new tool added to daily workflow, project shipped or killed.
- If a refresh is skipped 2x in a row, retire the biweekly cadence and shift to event-driven only.

## Checklist

### 1. Sync first (1 min)

```bash
cd C:/Users/john.hill/Claude-Projects/3-resources/personal-context
git pull
git status
```

If `git status` shows uncommitted changes from a prior session (this happened May 7 → May 19), surface them — they should be folded into this refresh, not stranded.

### 2. Diff prompt for each state file (10 min)

For each file, ask the question. Edit only if the answer changes.

| File | Diff question |
|------|---------------|
| `portfolio/now.md` | Always rewrite. New open questions, recent reading, loading-up items. |
| `portfolio/current-projects.md` | Any project started or killed since last refresh? Any project status materially changed? |
| `portfolio/goals-and-priorities.md` | Any Q-deliverable shipped or slipped? Any priority shifted? |
| `portfolio/team-and-relationships.md` | Any name change, role change, new direct report, new external relationship? |
| `portfolio/tools-and-systems.md` | Any new MCP added or retired? Any tool moved from "evaluating" to "daily"? |

**Inputs to scan (pick 2-3 that feel productive that day):**
- `git log --since="2 weeks ago" --pretty=format:"%h %ad %s" --date=short -- 1-projects/ 2-areas/` from `Claude-Projects/` root — shows project activity
- Tail of `~/.claude/projects/.../memory/MEMORY.md` — new memories often signal name/role/tool changes
- Recent session notes in `2026_Brain_Engine/60_System/Claude-Sessions/`
- Recent Todoist completed tasks (project tag filter)

### 3. Pattern files — append only (1 min)

`decision-log.md` is the only pattern file that should regularly change between quarterly reviews. If a significant decision landed in the last 2 weeks, add an entry. Otherwise skip.

Pattern files (identity, role, communication-style, preferences, domain-knowledge) only update at quarterly review or after a triggering event (title change, life event, new domain).

### 4. Commit + push (1 min)

```bash
git add .
git commit -m "Refresh YYYY-MM-DD to YYYY-MM-DD"
git push
```

Date range = last refresh date to today (read from `git log -1 --format=%cd --date=short`).

### 5. Verify (1 min)

- `git log -1` shows the new commit.
- Open `github.com/jhillgvtc/personal-context-portfolio` and confirm the commit pushed.

## Retire criteria

The 5/7 decision-log entry framed this as a deliberate experiment. Retire the biweekly ritual if either:

- Two consecutive scheduled refreshes lapse (the cadence didn't fire — same failure as April 27 → May 19), **OR**
- Three consecutive refreshes produce zero meaningful diffs across all state files (the cadence is firing but isn't paying for itself).

Replacement: event-driven refresh only — org change, new project, post-promotion, role transition.

## Promote criteria

If this playbook runs cleanly twice manually (next: 2026-06-02 and 2026-06-16), promote to a `/refresh-context` slash command that runs the playbook autonomously and surfaces a diff for John to approve.
