# Git & GitHub Cheat Sheet

## Setup

```bash
git --version

git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## Repository

```bash
git init
git status
```

## Changes

```bash
git diff
git add filename
git add .
git diff --staged
```

## Commits

```bash
git commit -m "Describe the change"
git log
git log --oneline
```

## Branches

```bash
git branch
git switch -c feature-name
git switch main
git merge feature-name
```

## Remote

```bash
git remote -v
git remote add origin <repository-url>
```

## GitHub

```bash
git push
git push -u origin branch-name
git pull
git clone <repository-url>
```

## The everyday workflow

```bash
git status
git add .
git commit -m "Describe what changed"
git push
```

## The team workflow

```bash
git pull
git switch -c feature/my-change
# make changes
git add .
git commit -m "Add my change"
git push -u origin feature/my-change
# open Pull Request on GitHub
```

## Remember

```text
init   = start a repository
clone  = copy an existing repository
add    = stage changes
commit = save a version locally
push   = send commits to remote
pull   = bring remote changes locally
branch = create an independent line of work
merge  = combine branches
```
