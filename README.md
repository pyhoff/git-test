# Learning how GIT works

## Commands we learned about
- git init: Creates the repo
- git status: Compares the working directory, staging area and current branch
- git add: adds changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: Sets or gets the git config.
- git log: Shows history of project commits
- git branch -b: Create branch, and checks out to the new branch

## What is a branch?

A branch is a ref(erence) to a commit. When HEAD points to a branch, we say we are "on" that branch. When a commit is performed on the branch, the is updated to ref(er) to th new commit.

## What is HEAD?

Head is a ref(erenece) to the "current" branch (or sometimes a commit). Git commands such as `status`, `log` and `branch` use HEAD. `git checkout` updates the HEAD to ref(er) to a different branch.

## Commit messags
Uses the default editor for OS, on OSX it's `VIM` on Ubuntu it's `nano` and it can be changed.
- `i` to enter *insert* mode
- Type commit message
- `esc` -> `:wq` -> `Enter` to write message and quit.
to avod opening editor, use `git commit -m "<message>"`
- Line should contain info that is concise and accurate, of what is being committed.
- Try to use proper spelling, grammar and punctuation
- Do not end with a `.`
