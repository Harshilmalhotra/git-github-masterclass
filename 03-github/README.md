# 03 — GitHub & Remotes

Now connect your local repository to GitHub.

## Git vs GitHub

**Git** is the version control system.

**GitHub** is a platform for hosting Git repositories and collaborating around them.

## 1. Create a GitHub repository

On GitHub, create a new repository.

For this exercise, use a simple name such as:

```text
my-first-github-repository
```

If you already have a local project, avoid initializing the GitHub repository with another README for this exercise. We will connect the existing local repository.

## 2. Add the remote

Copy your repository URL and run:

```bash
git remote add origin <repository-url>
```

Check:

```bash
git remote -v
```

`origin` is simply the conventional name for the remote repository.

## 3. Check your branch

```bash
git branch
```

If your local branch is called `master` and you want `main`:

```bash
git branch -M main
```

## 4. Push

```bash
git push -u origin main
```

Refresh GitHub.

Your local project is now on GitHub.

## What happened?

```text
Your computer
     |
 Local Git repository
     |
 git push
     v
GitHub repository
```

## Exercise

Make another local change:

```bash
git add .
git commit -m "Add GitHub exercise content"
git push
```

Refresh GitHub and verify the commit appears.

## GitHub UI task

On GitHub:

1. Open `README.md`.
2. Edit one line.
3. Commit the change using the web interface.
4. Return to your terminal.
5. Run:

```bash
git pull
```

Verify that the change is now local.

This demonstrates that changes can originate from both your computer and GitHub.
