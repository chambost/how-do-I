---
title: How do I use 'git commit-tree'?
manual: <https://git-scm.com/docs/git-commit-tree>
---

# git commit-tree <options>
- ???

# Example
- empty ophan root  

```bash
tree=`git hash-object -wt tree --stdin < /dev/null`
commit=`git commit-tree -m 'root commit' $tree`
git rebase --onto $commit --root master```
  - <https://stackoverflow.com/questions/645450/insert-a-commit-before-the-root-commit-in-git?noredirect=1&lq=1>