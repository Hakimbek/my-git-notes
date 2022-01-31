# Git Reset
The term reset stands for undoing changes. The git reset command is used to reset the changes. The git reset command has three core forms of invocation. These forms are as follows.

- Soft
- Mixed
- Hard

If we say in terms of Git, then Git is a tool that resets the current state of HEAD to a specified state. It is a sophisticated and versatile tool for undoing changes. It acts as a time machine for Git. You can jump up and forth between the various commits. Each of these reset variations affects specific trees that git uses to handle your file in its content.

Additionally, git reset can operate on whole commits objects or at an individual file level. Each of these reset variations affects specific trees that git uses to handle your file and its contents.

Git uses an index (staging area), HEAD, and working directory for creating and reverting commits. The working directory lets you change the file, and you can stage into the index. The staging area enables you to select what you want to put into your next commit. A commit object is a cryptographically hashed version of the content. It has some Metadata and points which are used to switch on the previous commits.

## Git Reset Hard
It will first move the Head and update the index with the contents of the commits. It is the most direct, unsafe, and frequently used option. The --hard option changes the Commit History, and ref pointers are updated to the specified commit. Then, the Staging Index and Working Directory need to reset to match that of the specified commit. Any previously pending commits to the Staging Index and the Working Directory gets reset to match Commit Tree. It means any awaiting work will be lost.

Let's understand the --hard option with an example. Suppose I have added a new file to my existing repository. To add a new file to the repository, run the below command:
```
$ git add <file name>  
```
To check the status of the repository, run the below command:
```
$ git status  
```
To check the status of the Head and previous commits, run the below command:
```
$ git log  
```

In the above output, I have added a file named newfile2.txt. I have checked the status of the repository. We can see that the current head position yet not changed because I have not committed the changes. Now, I am going to perform the reset --hard option. The git reset hard command will be performed as:
```
$ git reset --hard  
```

The -hard option is operated on the available repository. This option will reset the changes and match the position of the Head before the last changes. It will remove the available changes from the staging area. There is a safer way to reset the changes with the help of git stash.

Generally, the reset hard mode performs below operations:
- It will move the HEAD pointer.
- It will update the staging Area with the content that the HEAD is pointing.
- It will update the working directory to match the Staging Area.

## Git Reset Mixed
A mixed option is a default option of the git reset command. If we would not pass any argument, then the git reset command considered as --mixed as default option. A mixed option updates the ref pointers. The staging area also reset to the state of a specified commit. The undone changes transferred to the working directory. 

Generally, the reset mixed mode performs the below operations:

- It will move the HEAD pointer
- It will update the Staging Area with the content that the HEAD is pointing to.

## Git Reset to Commit
Sometimes we need to reset a particular commit; Git allows us to do so. We can reset to a particular commit. To reset it, git reset command can be used with any option supported by reset command. It will take the default behavior of a particular command and reset the given commit. The syntax for resetting commit is given below:
```
$ git reset <option> <commit-sha>  
```
These options can be

- --soft
- --mixed
- --Hard
