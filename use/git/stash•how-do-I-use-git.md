---
title: How do I use 'git stash'?
manual: <https://git-scm.com/docs/git-stash>
---

# `git stash <options>`
- safeguards changes while reset working tree
- equivalent to: `git stash save`
- to undo: `git stash apply`


## `git stash --include-untracked`
- Also stash newly created (untracked) files
- useful when "No local changes to save" otherwise occurs

## git stash apply
- apply stashed changes to working tree while retaining the stash
- <https://stackoverflow.com/questions/19003009/how-to-recover-stashed-uncommitted-changes/19003191>

## git stash drop
- remove a stash
- to reverse a drop: <https://stackoverflow.com/questions/89332/how-to-recover-a-dropped-stash-in-git>

# How to backup a git stash
- <https://stackoverflow.com/questions/42358448/how-to-backup-git-stash-content>