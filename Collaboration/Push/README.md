# Git Push
The push term refers to upload local repository content to a remote repository. Pushing is an act of transfer commits from your local repository to a remote repository. Pushing is capable of overwriting changes; caution should be taken when pushing.

Moreover, we can say the push updates the remote refs with local refs. Every time you push into the repository, it is updated with some interesting changes that you made. If we do not specify the location of a repository, then it will push to default location at origin master.

The "git push" command is used to push into the repository. The push command can be considered as a tool to transfer commits between local and remote repositories. 

```
$ git push <option> [<Remote URL><branch name><refspec>...]
```

Push command supports many additional options. Some options are as follows under push tags.

## Git Push Tags
### \<repository\>: 
The repository is the destination of a push operation. It can be either a URL or the name of a remote repository.

### \<refspec\>: 
It specifies the destination ref to update source object.

### --all:
The word "all" stands for all branches. It pushes all branches.

### --prune:
It removes the remote branches that do not have a local counterpart. Means, if you have a remote branch say demo, if this branch does not exist locally, then it will be removed.

### --mirror:
It is used to mirror the repository to the remote. Updated or Newly created local refs will be pushed to the remote end. It can be force updated on the remote end. The deleted refs will be removed from the remote end.

### --dry-run:
Dry run tests the commands. It does all this except originally update the repository.

### --tags:
It pushes all local tags.

### --delete:
It deletes the specified branch.

### -u:
It creates an upstream tracking connection. It is very useful if you are going to push the branch for the first time.

## Git Push Origin Master
Git push origin master is a special command-line utility that specifies the remote branch and directory. When you have multiple branches and directory, then this command assists you in determining your main branch and repository.

Generally, the term origin stands for the remote repository, and master is considered as the main branch. So, the entire statement "git push origin master" pushed the local content on the master branch of the remote location.

```
$ git push origin master  
```

## Git Force Push
The git force push allows you to push local repository to remote without dealing with conflicts. It is used as follows:

```
$ git push <remote><branch> -f  
```

Or

```
$ git push <remote><branch> -force  
```

## Delete a Remote Branch
We can delete a remote branch using git push. It allows removing a remote branch from the command line.

```
$ git push origin -delete edited 
```
