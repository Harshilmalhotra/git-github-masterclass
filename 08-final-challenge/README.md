# 08 — Final Challenge

## Mission

You are joining a real software project.

Your task is to complete the entire Git + GitHub workflow.

## Scenario

Create a repository called:

```text
student-profile
```

It should contain:

```text
student-profile/
├── README.md
├── projects.md
└── skills.md
```

## Part 1 — Local Git

Create the project locally.

```bash
git init
```

Create the files.

Then:

```bash
git status
git add .
git commit -m "Initial student profile"
```

Check:

```bash
git log --oneline
```

## Part 2 — GitHub

Create the GitHub repository.

Connect it:

```bash
git remote add origin <repository-url>
```

Push:

```bash
git push -u origin main
```

## Part 3 — Feature branch

Create:

```bash
git switch -c feature/add-project
```

Add a new project to `projects.md`.

Commit:

```bash
git add .
git commit -m "Add project to student profile"
```

Push:

```bash
git push -u origin feature/add-project
```

## Part 4 — Pull Request

Open a Pull Request:

```text
feature/add-project
        ↓
       main
```

Write a useful title and description.

## Part 5 — Review

Ask a partner to review your Pull Request.

Respond to their feedback.

## Part 6 — Merge

Once approved, merge the Pull Request.

## Part 7 — Update local main

Return to your terminal:

```bash
git switch main
git pull
```

Confirm your merged changes are present.

## Final checklist

```text
[ ] Git configured
[ ] Local repository created
[ ] At least 2 commits created
[ ] GitHub repository created
[ ] Remote configured
[ ] Changes pushed
[ ] Feature branch created
[ ] Branch pushed
[ ] Pull Request created
[ ] Pull Request reviewed
[ ] Pull Request merged
[ ] Local main updated with git pull
```

## Bonus challenge

Create a merge conflict with a partner and resolve it.

If you can complete the full workflow without copying commands from the previous modules, you are ready to start contributing to a real GitHub project.
