# Git Checkout
In Git, the term checkout is used for the act of switching between different versions of a target entity. The git checkout command is used to switch between branches in a repository. Be careful with your staged files and commits when switching between branches.

The git checkout command operates upon three different entities which are files, commits, and branches. Sometimes this command can be dangerous because there is no undo option available on this command.

It checks the branches and updates the files in the working directory to match the version already available in that branch, and it forwards the updates to Git to save all new commit in that branch.

## Operations on Git Checkout
We can perform many operations by git checkout command like the switch to a specific branch, create a new branch, checkout a remote branch, and more. The git branch and git checkout commands can be integrated.

## Checkout Branch
You can demonstrate how to view a list of available branches by executing the git branch command and switch to a specified branch.

To demonstrate available branches in repository, use the below command:
```
$ git branch  
```
Now, you have the list of available branches. To switch between branches, use the below command.
```
$ git checkout <branchname>  
```

## Create and Switch Branch
The git checkout commands let you create and switch to a new branch. You can not only create a new branch but also switch it simultaneously by a single command. The git checkout -b option is a convenience flag that performs run git branch \<new-branch>operation before running git checkout \<new-branch>.
  
```
$ git checkout -b <branchname>  
```

## Checkout Remote Branch
Git allows you to check out a remote branch by git checkout command. It is a way for a programmer to access the work of a colleague or collaborator for review and collaboration. Each remote repository contains its own set of branches. So, to check out a remote branch, you have first to fetch the contents of the branch.
```
$ git fetch --all  
```

In the latest versions of Git, you can check out the remote branch like a local branch.

```
$ git checkout <remotebranch>  
```
