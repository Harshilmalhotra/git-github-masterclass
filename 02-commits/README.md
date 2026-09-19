# 02 — Commits & History

A commit is a recorded snapshot of changes in your Git repository.

## 1. View history

```bash
git log
```

Compact view:

```bash
git log --oneline
```

## 2. Inspect changes

Edit a tracked file and run:

```bash
git diff
```

This shows changes that have not been staged.

After:

```bash
git add .
```

you can inspect staged changes with:

```bash
git diff --staged
```

## 3. Good commit messages

Prefer:

```text
Add student profile page
Fix login validation
Update installation instructions
Add RFID access documentation
```

Avoid:

```text
stuff
changes
final
asdf
update
```

A commit message should explain what changed.

## Exercise

Make three separate changes and create three separate commits.

Example:

```bash
git add .
git commit -m "Add project description"

git add .
git commit -m "Add installation instructions"

git add .
git commit -m "Update contact information"
```

Then:

```bash
git log --oneline
```

You should be able to explain what each commit did.

## Key idea

A commit is not "upload to GitHub".

A commit exists in your **local repository** first.

```text
git commit
     |
     v
LOCAL HISTORY

git push
     |
     v
GITHUB
```
