# Git Status
The git status command is used to display the state of the repository and staging area. It allows us to see the tracked, untracked files and changes. This command will not show any commit records or information.

Mostly, it is used to display the state between **Git Add** and **Git commit** command. We can check whether the changes and files are tracked or not.

Let's understand the different states of status command.

Status when Working Tree is cleaned
Before starting with git status command, let's see how the git status looks like when there are no changes made. To check the status, open the git bash, and run the status command on your desired directory. It will run as follows:
```
$ git status 
```

Since there is nothing to track or untrack in the working tree, so the output is showing as the working tree is clean.

## Status when a new file is created
When we create a file in the repository, the state of the repository changes. Let's create a file using the touch command. 

## Status when an existing file is modified
Let's check the status when an existing file is modified. To modify file, run the echo command as follows:
```
$ echo "Text"> Filename  
```
The above command will add the text to the specified file, now check the status of the repository. Consider the below output:

Status when a file is deleted
Let's check the status when a file is deleted from the repository. To delete a file from the repository, run the rm command as follows:
```
$ git rm < File Name>  
```
The above command will delete the specified file from the repository. Now, check the status of the repository. Consider the below output:
The current status of the repository has been updated as deleted.
