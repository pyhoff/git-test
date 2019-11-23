# Learning how GIT works

## Commands we learned about
- git init: Creates the git repo
- git status: Compares the working directory, staging area and current branch
- git add: adds changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: Sets or gets the git config.
- git log: Shows a history (aka log) of project commits
- git checkout: Check out branch ( update HEAD and apply changes to working directory)
- git branch -c: Create a branch
- git branch -b: Create branch, and checks out to the new branch
- git merge: Merge changes from different branches.

## What is a branch?

A branch is a ref(erence) to a commit. When HEAD points to a branch, we say we are "on" that branch. When a commit is performed on the branch, the is updated to ref(er) to th new commit.

## What is HEAD?

Head is a ref(erenece) to the "current" branch (or sometimes a commit). Git commands such as `status`, `log` and `branch` use HEAD. `git checkout` updates the HEAD to ref(er) to a different branch.

## Commit messages
Uses the default editor for OS, on OSX it's `VIM` on Ubuntu it's `nano` and it can be changed.
- `i` to enter *insert* mode
- Type commit message
- `esc` -> `:wq` -> `Enter` to write message and quit.
to avod opening editor, use `git commit -m "<message>"`
- Line should contain info that is concise and accurate, of what is being committed.
- Try to use proper spelling, grammar and punctuation
- Do not end with a `.`

## Merging
Merging means to bring changes from one branches into another

- A fast-forward merge happens when the target branch was branched  from current one, an the are no new changes to the current branch since then.
- An Automatic merge happens when the two histories have diverged, but git is able t reconcile then into one set of changes. This Creates a new commit on the current branch.
