# Git Fetch
Git "fetch" Downloads commits, objects and refs from another repository. It fetches branches and tags from one or more repositories. It holds repositories along with the objects that are necessary to complete their histories to keep updated remote-tracking branches.

## The "git fetch"command
The "git fetch" command is used to pull the updates from remote-tracking branches. Additionally, we can get the updates that have been pushed to our remote branches to our local machines. As we know, a branch is a variation of our repositories main code, so the remote-tracking branches are branches that have been set up to pull and push from remote repository.

## How to fetch Git Repository
We can use fetch command with many arguments for a particular data fetch. See the below scenarios to understand the uses of fetch command.

### Scenario 1: To fetch the remote repository:
We can fetch the complete repository with the help of fetch command from a repository URL like a pull command does.

```
$ git fetch< repository Url> 
```

### Scenario 2: To fetch a specific branch:
We can fetch a specific branch from a repository. It will only access the element from a specific branch.

```
$ git fetch <branch URL> <branch name>  
```

### Scenario 3: To fetch all the branches simultaneously:
The git fetch command allows to fetch all branches simultaneously from a remote repository.

```
$ git fetch -all  
```

### Scenario 4: To synchronize the local repository:
Suppose, your team member has added some new features to your remote repository. So, to add these updates to your local repository, use the git fetch command.

```
$ git fetch origin  
```

The git fetch can fetch from either a single named repository or URL or from several repositories at once. It can be considered as the safe version of the git pull commands. The git fetch downloads the remote content but not update your local repo's working state. When no remote server is specified, by default, it will fetch the origin remote.

## Differences between git fetch and git pull
To understand the differences between fetch and pull, let's know the similarities between both of these commands. Both commands are used to download the data from a remote repository. But both of these commands work differently. Like when you do a git pull, it gets all the changes from the remote or central repository and makes it available to your corresponding branch in your local repository. When you do a git fetch, it fetches all the changes from the remote repository and stores it in a separate branch in your local repository. You can reflect those changes in your corresponding branches by merging.

So basically,

```
git pull = git fetch + git merge  
```
