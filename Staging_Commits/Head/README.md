# Git Head
The HEAD points out the last commit in the current checkout branch. It is like a pointer to any reference. The HEAD can be understood as the "current branch." When you switch branches with 'checkout,' the HEAD is transferred to the new branch.

## Git Show Head
The git show head is used to check the status of the Head. This command will show the location of the Head.

```
$ git show HEAD  
```

## Git Detached Head
GitHub keeps track of all commits or snapshots over time. If you check the 'git log' in your terminal, you can show all the previous commits up to the first commit. Detached HEAD mode allows you to discover an older state of a repository. It is a natural state in Git.

When Head doesn't point to most recent commit, such state is called detached Head. If you checkout with an older commit, it will stand the detached head condition. 
