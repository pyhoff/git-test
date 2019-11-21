# Learning how GIT works

## Commands we learned about
- git init: Creates the repo
- git status: Compares the working directory, staging area and current branch
- git add: adds changes from working directory to staging area
- git commit: Commit changes from staging area to current branch
- git config: Sets or gets the git config.
- git log: Shows history of project commits
- git show: Show a single commit
- git diff: Show the difference between commits, the working directory and the staging area.
- git checkout: Check out branch ( update HEAD and apply changes to working directory)

## Commit messags
Uses the default editor for OS, on OSX it's `VIM` on Ubuntu it's `nano` and it can be changed.
- `i` to enter *insert* mode
- Type commit message
- `esc` -> `:wq` -> `Enter` to write message and quit.
to avod opening editor, use `git commit -m "<message>"`
- Line should contain info that is concise and accurate, of what is being committed.
- Try to use proper spelling, grammar and punctuation
- Do not end with a `.`
