# Git Rebase
Rebasing is a process to reapply commits on top of another base trip. It is used to apply a sequence of commits from distinct branches into a final commit. It is an alternative of git merge command. It is a linear process of merging.

In Git, the term rebase is referred to as the process of moving or combining a sequence of commits to a new base commit. Rebasing is very beneficial and it visualized the process in the environment of a feature branching workflow.

It is good to rebase your branch before merging it.

Generally, it is an alternative of git merge command. Merge is always a forward changing record. Comparatively, rebase is a compelling history rewriting tool in git. It merges the different commits one by one.

Suppose you have made three commits in your master branch and three in your other branch named test. If you merge this, then it will merge all commits in a time. But if you rebase it, then it will be merged in a linear manner.

Merging is the most straightforward way to integrate the branches. It performs a three-way merge between the two latest branch commits.

## How to Rebase
When you made some commits on a feature branch (test branch) and some in the master branch. You can rebase any of these branches. Use the git log command to track the changes (commit history). Checkout to the desired branch you want to rebase. Now perform the rebase command as follows:

Syntax:
```
$ git rebase <branch name>  
```
If there are some conflicts in the branch, resolve them, and perform below commands to continue changes:
```
$ git status  
```
It is used to check the status,

$git rebase --continue  
The above command is used to continue with the changes you made. If you want to skip the change, you can skip as follows:
```
$ git rebase --skip  
```

## Rebase Branch
If we have many commits from distinct branches and want to merge it in one. To do so, we have two choices either we can merge it or rebase it. It is good to rebase your branch.
