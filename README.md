# ISD Lab — Git & GitHub Masterclass

Welcome to the **ISD Lab Git & GitHub Masterclass**.

This repository is a hands-on course for students who are new to Git and GitHub. You will learn the concepts first, then use the Git CLI and GitHub UI to complete a real collaborative workflow.

## What you will learn

- Git vs GitHub
- Local repositories and the Git mental model
- `git init`, `git status`, `git add`, `git commit`
- Commit history and `git diff`
- GitHub repositories and remotes
- `git push`, `git pull`, and `git clone`
- Branches with `git branch` and `git switch`
- Merging
- Pull Requests and code review
- Merge conflicts
- A complete team workflow

## The core workflow

```text
Working Directory
       |
     git add
       v
Staging Area
       |
   git commit
       v
Local Repository
       |
    git push
       v
GitHub
```

## Collaborative workflow

```text
Clone
  |
Create Branch
  |
Make Changes
  |
Commit
  |
Push
  |
Pull Request
  |
Review
  |
Merge
  |
main
```

## Learning path

1. [Git Basics](./01-git-basics/README.md)
2. [Commits & History](./02-commits/README.md)
3. [GitHub & Remotes](./03-github/README.md)
4. [Clone & Pull](./04-clone-pull/README.md)
5. [Branches](./05-branches/README.md)
6. [Pull Requests](./06-pull-requests/README.md)
7. [Merge Conflicts](./07-merge-conflicts/README.md)
8. [Final Challenge](./08-final-challenge/README.md)

## Playground

The `playground/` directory contains tiny exercises where you are encouraged to experiment. You cannot permanently damage Git by trying normal Git commands in your own practice repository.

## Essential commands

```bash
git init
git status
git add .
git commit -m "Your message"
git log --oneline
git diff
git branch
git switch -c feature-name
git switch main
git merge feature-name
git clone <repository-url>
git pull
git push
```

## Golden rule

Do not memorize commands blindly. Understand the state transition:

```text
EDIT -> ADD -> COMMIT -> PUSH
```

and, when collaborating:

```text
CLONE -> BRANCH -> EDIT -> COMMIT -> PUSH -> PR -> REVIEW -> MERGE
```

## Final outcome

By the end of this repository, you should be able to join an existing project, make a change safely on a branch, publish it to GitHub, open a Pull Request, respond to review, resolve a conflict, and get your work merged.

**Start here:** [01 — Git Basics](./01-git-basics/README.md)
