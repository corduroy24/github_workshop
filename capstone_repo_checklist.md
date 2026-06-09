# Capstone Repo Checklist

## Repository Basics

- [ ] Repo has a clear name.
- [ ] README explains the project in one paragraph.
- [ ] README has setup commands.
- [ ] README has run commands.
- [ ] README lists current limitations or next steps.
- [ ] `.gitignore` excludes `.env`, `.venv/`, `__pycache__/`, and local data.
- [ ] `.env.example` lists required environment variable names with fake values.

## Commit Quality

- [ ] `git status` is clean after the commit.
- [ ] Commit message says what changed.
- [ ] Commit is small enough to review.
- [ ] No generated cache files are staged.
- [ ] No API keys, tokens, passwords, or private data are staged.

## GitHub Workflow

- [ ] Remote is set with `git remote -v`.
- [ ] Branch name describes one task.
- [ ] Branch is pushed to GitHub.
- [ ] Pull request exists, or the branch is PR-ready.
- [ ] PR description says what changed and how to test.

## Project Planning

- [ ] At least three GitHub issues exist, or three local issue bullets are ready.
- [ ] Each issue starts with a verb.
- [ ] Each issue has a clear finish condition.
- [ ] The team knows who owns the next task.

## Suggested Issues

```text
Add a README quickstart
Create .env.example and config loader
Add a sample evaluation case
Add a simple project architecture diagram
Write a smoke test for the main workflow
Document one known failure mode
```
