# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository

GitHub: https://github.com/anacbritoa-glitch/ClaudeCode  
This is an active workspace — a project will be built here over time.

## Git Workflow

**Commit and push to GitHub regularly throughout every session.** This is not optional — it ensures work is never lost and any state can be restored.

```powershell
git add <file(s)>
git commit -m "Short description of what changed and why"
git push
```

### When to commit

- After completing any discrete piece of work (new file, feature, fix, refactor)
- Before and after making risky or large changes
- At the end of every session, even if work is mid-flight — commit with a `WIP:` prefix rather than leaving uncommitted changes

### Commit message rules

- Describe intent and effect, not the mechanics ("add login form validation" not "edit auth.js")
- Use present tense imperative ("add", "fix", "remove", "update")
- Keep the subject line under 72 characters
- If the why is non-obvious, add a short body after a blank line

### Reverting

- `git log --oneline` — find the target commit hash
- `git checkout <hash> -- <file>` — restore a single file
- `git revert <hash>` — undo a commit while preserving history

## Environment

- Platform: Windows 11, PowerShell
- GitHub account: anacbritoa-glitch
- GitHub CLI (`gh`) is authenticated and available
