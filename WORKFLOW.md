# Git Workflow Reflection

## 1. Rejected Push Error

The rejected push said that the remote contained work that I did not have locally and that I needed to fetch the changes first. This happened because another clone had pushed changes to the same feature branch before I tried to push my local commit. My local branch was therefore behind the remote branch.

## 2. Merge vs. Rebase

In Task 3, I used merge to combine the changes from the remote feature branch with my changes. This created a merge commit and preserved both branch histories.

In Task 4, I used rebase to place my local commit on top of the updated remote branch. This created a new commit with a different hash and resulted in a cleaner, linear history.

## 3. Habit to Avoid Rejected Pushes

One habit that can avoid rejected pushes is to fetch the latest remote changes before starting new work or pushing a commit. This helps me know if another person has already updated the branch.

## 4. Merge or Rebase on a Shared Team Branch

For a shared team branch, I would use merge as the safer default because it preserves the history of different contributors and does not rewrite existing shared commits. Rebase can still be useful for cleaning up my own local commits before sharing them.