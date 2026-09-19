# 05 — Branches

Branches let you work on changes without directly changing the stable branch.

## Why branches?

Imagine:

```text
main
 |
 ●
 |
 ●
```

You want to build a new feature.

Instead of experimenting directly on `main`:

```text
main
 |
 ●
 |\
 | \
 |  ● feature/login
 |  ●
 |
 ●
```

## List branches

```bash
git branch
```

## Create and switch to a branch

Modern Git:

```bash
git switch -c feature/login
```

Check:

```bash
git branch
```

## Make a change

Edit a file.

Then:

```bash
git add .
git commit -m "Add login feature"
```

## Switch back

```bash
git switch main
```

Your feature changes are not necessarily present on `main`.

## Merge

From `main`:

```bash
git merge feature/login
```

Now the feature branch's changes have been incorporated into `main`.

## Push a branch

```bash
git push -u origin feature/login
```

## Important vocabulary

- **main** — commonly the stable/default branch
- **feature branch** — a branch used to develop a change
- **merge** — combine changes from one branch into another

## Exercise

Create:

```bash
git switch -c feature/about
```

Add an `about.md` file.

Commit it:

```bash
git add .
git commit -m "Add about page"
```

Push the branch:

```bash
git push -u origin feature/about
```

Then create a Pull Request on GitHub.

Do **not** merge immediately. Continue to the Pull Request module.
