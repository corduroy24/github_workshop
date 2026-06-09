# Git/GitHub Command Sheet


Testing commit

## Check Your Setup

```bash
git --version
git config --global user.name
git config --global user.email
```

Set name and email if needed:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## Start Or Open A Repo

```bash
cd path/to/your/project
git init
git status
```

If the repo already exists:

```bash
git status
git log --oneline -5
```

## Ignore Local Files

Create or edit `.gitignore`:

```text
.env
.venv/
__pycache__/
*.pyc
.DS_Store
```

Never commit API keys. Keep real values in `.env`; commit only `.env.example`.

## Make A Small Commit

```bash
git status
git diff
git add README.md .env.example .gitignore
git diff --staged
git commit -m "docs: add capstone repo setup notes"
git status
```

## Branch For A Task

```bash
git switch -c improve-readme
```

Older Git fallback:

```bash
git checkout -b improve-readme
```

## Connect To GitHub

Create an empty GitHub repo in the browser first. Do not add a README there if
your local repo already has one.

Then connect the local repo:

```bash
git remote add origin https://github.com/YOUR-USER/YOUR-REPO.git
git remote -v
git push -u origin main
```

If your default branch is named `master`:

```bash
git branch -M main
git push -u origin main
```

## Push A Branch

```bash
git push -u origin improve-readme
```

Open the pull request from the GitHub browser prompt.

## Useful Recovery Commands

See unstaged changes:

```bash
git diff
```

Undo an unstaged change to one file:

```bash
git restore path/to/file
```

Unstage a file:

```bash
git restore --staged path/to/file
```

See recent commits:

```bash
git log --oneline --decorate -5
```
