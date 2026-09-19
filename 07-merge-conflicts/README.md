# 07 — Merge Conflicts

A merge conflict happens when Git cannot automatically decide how two changes should be combined.

Don't panic.

A conflict is Git asking:

> "Which final version should this file have?"

## Create a controlled conflict

Work with a partner.

Start from the same `main` commit.

Both students create branches.

### Student A

Change the same line in `conflict-demo.txt` to:

```text
Welcome to the ISD Lab Git Masterclass.
```

Commit and push.

### Student B

Change the same original line to:

```text
Welcome to the ISD Lab GitHub Workshop.
```

Commit and push.

Merge Student A's branch first.

Then try to merge Student B's changes.

Git may report a conflict.

## Conflict markers

You may see:

```text
<<<<<<< HEAD
Welcome to the ISD Lab Git Masterclass.
=======
Welcome to the ISD Lab GitHub Workshop.
>>>>>>> feature/student-b
```

These markers show the competing versions.

## Resolve it

Decide what the final content should be.

For example:

```text
Welcome to the ISD Lab Git & GitHub Masterclass.
```

Delete the conflict markers.

Then:

```bash
git add conflict-demo.txt
git commit -m "Resolve conflict in conflict demo"
```

If the conflict happened during a merge, the merge is now completed.

## Conflict resolution checklist

```text
[ ] Read the conflict
[ ] Understand both changes
[ ] Choose/combine the correct content
[ ] Remove conflict markers
[ ] Save the file
[ ] git add
[ ] git commit
[ ] Verify with git status
```

## Important

Never blindly delete one side just because Git says there is a conflict.

Ask:

> What should the final version actually contain?
