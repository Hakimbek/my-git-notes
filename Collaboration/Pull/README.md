# Git Pull / Pull Request
The term pull is used to receive data from GitHub. It fetches and merges changes from the remote server to your working directory. The git pull command is used to pull a repository.

Pull request is a process for a developer to notify team members that they have completed a feature. Once their feature branch is ready, the developer files a pull request via their remote server account. Pull request announces all the team members that they need to review the code and merge it into the master branch.

## The "git pull" command
The pull command is used to access the changes (commits)from a remote repository to the local repository. It updates the local branches with the remote-tracking branches. Remote tracking branches are branches that have been set up to push and pull from the remote repository. Generally, it is a collection of the fetch and merges command. First, it fetches the changes from remote and combined them with the local repository.

```
$ git pull <option> [<repository URL> <refspec>...]  
```

### \<option\>: 
Options are the commands; these commands are used as an additional option in a particular command. Options can be -q (quiet), -v (verbose), -e(edit) and more.

### \<repository URL\>:
Repository URL is your remote repository's URL where you have stored your original repositories like GitHub or any other git service.
  
### \<Refspec\>: 
A ref is referred to commit, for example, head (branches), tags, and remote branches. You can check head, tags, and remote repository in .git/ref directory on your local repository.

## Default git pull:
We can pull a remote repository by just using the git pull command. It's a default option. 

```
$ git pull  
```

## Git Pull Remote Branch
Git allows fetching a particular branch. Fetching a remote branch is a similar process, as mentioned above, in git pull command. The only difference is we have to copy the URL of the particular branch we want to pull.

```
$ git pull <remote branch URL>  
```

## Git Force Pull
Git force pull allows for pulling your repository at any cost. Suppose the below scenario:

If you have updated any file locally and other team members updated it on the remote. So, when will you fetch the repository, it may create a conflict.

We can say force pull is used for overwriting the files. If we want to discard all the changes in the local repository, then we can overwrite it by influentially pulling it. Consider the below process to force pull a repository:

### Step1: Use the git fetch command to download the latest updates from the remote without merging or rebasing.

```
$ git fetch -all  
```

### Step2: Use the git reset command to reset the master branch with updates that you fetched from remote. The hard option is used to forcefully change all the files in the local repository with a remote repository.

```
$ git reset -hard <remote>/<branch_name>  
$ git reset-hard master  
```

## Git Pull Origin Master
There is another way to pull the repository. We can pull the repository by using the git pull command.

```
$ git pull <options><remote>/<branchname>  
$ git pull origin master  
```

In the above syntax, the term origin stands for the repository location where the remote repository situated. Master is considered as the main branch of the project.
