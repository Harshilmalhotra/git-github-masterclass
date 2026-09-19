# 01 — Git Basics

## Objective

Understand what Git is and perform your first local Git workflow.

### You will learn

- Git repository
- Working directory
- Staging area
- Commit
- `git init`
- `git status`
- `git add`
- `git commit`

## 1. Check Git

```bash
git --version
```

If Git is installed, you will see its version.

## 2. Configure your identity

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

Check it:

```bash
git config --global --list
```

Git uses this information to identify who created a commit.

## 3. Create a project

```bash
mkdir my-first-git-project
cd my-first-git-project
```

## 4. Initialize Git

```bash
git init
```

You have created a local Git repository.

Check:

```bash
git status
```

## 5. Create a file

Create `hello.txt`:

```text
Hello, Git!
```

Then:

```bash
git status
```

Git should report the file as untracked.

## 6. Stage the file

```bash
git add hello.txt
git status
```

The file is now staged.

## 7. Commit

```bash
git commit -m "Add hello world file"
```

Then:

```bash
git status
git log --oneline
```

## The mental model

```text
Create/Edit File
      |
   git add
      v
Staging Area
      |
 git commit
      v
Local Repository
```

## Exercise

Modify `hello.txt` to:

```text
Hello, Git and GitHub!
```

Then:

1. Run `git status`.
2. Run `git diff`.
3. Stage the change.
4. Commit it.
5. Check the history.

Expected command sequence:

```bash
git status
git diff
git add .
git commit -m "Update greeting"
git log --oneline
```

## Challenge

Without copying the commands above:

1. Create `about-me.txt`.
2. Put your name and one project idea inside it.
3. Check the status.
4. Stage it.
5. Commit it.
6. Verify the commit.

If you can do that, you understand the basic Git workflow.
