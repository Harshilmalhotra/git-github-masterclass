# 04 — Clone & Pull

So far you created the repository. Now imagine someone else created it.

## Clone

`git clone` creates a local copy of an existing remote repository.

```bash
git clone <repository-url>
```

Then:

```bash
cd <repository-name>
git status
git remote -v
```

## Clone vs init

### `git init`

Use when starting a **new local Git repository**.

```text
Empty/new project
      |
   git init
```

### `git clone`

Use when an **existing repository already exists somewhere**.

```text
Existing GitHub repository
      |
   git clone
      |
Local copy
```

## Pull

If the remote repository has changes you do not have locally:

```bash
git pull
```

Think:

```text
GitHub
  |
git pull
  v
Local repository
```

## Exercise

Work with a partner.

### Person A

Clone the shared repository and add a file called:

```text
partner-a.txt
```

Commit and push.

### Person B

Before making a new change, run:

```bash
git pull
```

Confirm that `partner-a.txt` appears.

Then add:

```text
partner-b.txt
```

Commit and push.

### Success criteria

You should understand:

```text
clone = get the repository initially
pull  = update an existing local repository
push  = send local commits to the remote
```
