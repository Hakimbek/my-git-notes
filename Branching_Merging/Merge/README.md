# Git Merge and Merge Conflict
In Git, the merging is a procedure to connect the forked history. It joins two or more development history together. The git merge command facilitates you to take the data created by git branch and integrate them into a single branch. Git merge will associate a series of commits into one unified history. Generally, git merge is used to combine two branches.

It is used to maintain distinct lines of development; at some stage, you want to merge the changes in one branch. It is essential to understand how merging works in Git.

## The "git merge" command
The git merge command is used to merge the branches.

The syntax for the git merge command is as:
```
$ git merge <query>  
```
It can be used in various context. Some are as follows:

## Scenario1: To merge the specified commit to currently active branch:

Use the below command to merge the specified commit to currently active branch.
```
$ git merge <commit>  
```
The above command will merge the specified commit to the currently active branch. You can also merge the specified commit to a specified branch by passing in the branch name in \<commit>.

## Scenario2: To merge commits into the master branch:

To merge a specified commit into master, first discover its commit id. Use the log command to find the particular commit id.
```
$ git log  
```

To merge the commits into the master branch, switch over to the master branch.
```
$ git checkout master  
```

Now, Switch to branch 'master' to perform merging operation on a commit. Use the git merge command along with master branch name. The syntax for this is as follows:
```
$ git merge <commit>
```

## Scenario 3: Git merge branch.

Git allows merging the whole branch in another branch. Suppose you have made many changes on a branch and want to merge all of that at a time. Git allows you to do so.
```
$ git merge <branchname>  
```

## Git Merge Conflict
When two branches are trying to merge, and both are edited at the same time and in the same file, Git won't be able to identify which version is to take for changes. Such a situation is called merge conflict. If such a situation occurs, it stops just before the merge commit so that you can resolve the conflicts manually.

In the given output, git rebase command is used to pull the repository from the remote URL. Here, it will show the error message like merge conflict in \<filename>.

## Resolve Conflict:
To resolve the conflict, it is necessary to know whether the conflict occurs and why it occurs. Git merge tool command is used to resolve the conflict. The merge command is used as follows:
```
$ git mergetool  
```

To accept the changes, use the rebase command. It will be used as follows:
```
$ git rebase --continue  
```
  
  
