# Instructor Guide

## Suggested session

| Time | Topic |
|---|---|
| 00:00–00:15 | Why Git / GitHub |
| 00:15–00:35 | Mental model |
| 00:35–00:50 | Setup |
| 00:50–01:20 | init → add → commit |
| 01:20–01:40 | GitHub → remote → push |
| 01:40–02:00 | Break |
| 02:00–02:20 | clone → pull |
| 02:20–02:50 | branches |
| 02:50–03:20 | Pull Requests |
| 03:20–03:40 | conflicts |
| 03:40–04:00 | final challenge |

## Teaching principle

Do not teach commands as isolated syntax.

Teach the state transition:

```text
Working Directory
      ↓ git add
Staging Area
      ↓ git commit
Local Repository
      ↓ git push
GitHub
```

Then introduce collaboration:

```text
Clone → Branch → Commit → Push → Pull Request → Review → Merge
```

## Live demo checklist

Before the session:

- Verify Git is installed on the instructor computer.
- Verify GitHub account.
- Have one demo repository ready.
- Test push/pull.
- Test a branch.
- Test a Pull Request.
- Prepare two branches for a controlled merge conflict.
- Keep the final challenge repository clean.

## Instructor tip

When a student asks "What command do I type?", first ask:

> "What are you trying to do right now?"

Then connect the action to the command. This encourages understanding instead of memorization.
