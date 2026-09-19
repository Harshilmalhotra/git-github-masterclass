# 06 — Pull Requests

A Pull Request (PR) is a request to merge changes from one branch into another, usually `main`.

## Typical workflow

```text
main
 |
 +---- feature/my-change
             |
          commit
             |
           push
             |
           GitHub
             |
      Pull Request
             |
          Review
             |
           Merge
             |
            main
```

## Create a Pull Request

After pushing:

```bash
git push -u origin feature/my-change
```

Go to GitHub.

Open a Pull Request from:

```text
feature/my-change
        ↓
       main
```

## A good PR contains

### Title

Clearly describe the change.

Good:

```text
Add student profile section
```

Bad:

```text
Update
```

### Description

Explain:

- What changed?
- Why was it changed?
- How can someone test it?

## Review

A reviewer can:

- Read the changed files
- Leave comments
- Request changes
- Approve the PR

## Exercise — Team workflow

Work in groups.

Each student must:

1. Clone the repository.
2. Create a feature branch.
3. Make a small change.
4. Commit it.
5. Push the branch.
6. Open a Pull Request.
7. Review another student's PR.
8. Respond to at least one review comment.
9. Merge the approved PR.

### Rule

**Do not push directly to `main` during this exercise.**

This is the workflow you are likely to encounter in real software projects.
