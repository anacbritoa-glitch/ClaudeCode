# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository

GitHub: https://github.com/anacbritoa-glitch/ClaudeCode  
This is an active workspace — a project will be built here over time.

## Git Workflow

Every meaningful change should be committed and pushed to GitHub so work can be reverted if needed.

```powershell
git add <file(s)>
git commit -m "Short description of what changed and why"
git push
```

- Commit messages should be concise and describe intent, not mechanics.
- Push after each logical unit of work, not just at end of session.
- To revert to a previous state: `git log --oneline` to find the hash, then `git checkout <hash> -- <file>` for a single file or `git revert <hash>` for a full commit undo.

## Environment

- Platform: Windows 11, PowerShell
- GitHub account: anacbritoa-glitch
- GitHub CLI (`gh`) is authenticated and available
