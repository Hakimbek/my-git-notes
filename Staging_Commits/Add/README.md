# Git Add
The git add command is used to add file contents to the Index (Staging Area). This command updates the current content of the working tree to the staging area. It also prepares the staged content for the next commit. Every time we add or update any file in our project, it is required to forward updates to the staging area.

The git add command is a core part of Git technology. It typically adds one file at a time, but there some options are available that can add more than one file at once.

The "index" contains a snapshot of the working tree data. This snapshot will be forwarded for the next commit.

The git add command can be run many times before making a commit. These all add operations can be put under one commit. The add command adds the files that are specified on command line.

The git add command does not add the *.gitignore* file by default. In fact, we can ignore the files by this command.

## Git add files
Git add command is a straight forward command. It adds files to the staging area. We can add single or multiple files at once in the staging area. It will be run as:
```
$ git add <File name>  
```
The above command is added to the git staging area, but yet it cannot be shared on the version control system. A commit operation is needed to share it.

## Git Add All
We can add more than one files in Git, but we have to run the add command repeatedly. Git facilitates us with a unique option of the add command by which we can add all the available files at once. To add all the files from the repository, run the add command with -A option. We can use '.' Instead of -A option. This command will stage all the files at a time. It will run as follows:
```
$ git add -A  
```
Or
```
$ git add .  
```
The above command will add all the files available in the repository. 

## Add all New and Updated Files Only:
Git allows us to stage only updated and newly created files at once. We will use the ignore removal option to do so. It will be used as follows:
```
$ git add --ignore-removal .  
```

## Add all Modified and Deleted Files
Git add facilitates us with a variety of options. There is another option that is available in Git, which allows us to stage only the modified and deleted files. It will not stage the newly created file. To stage all modified and deleted files only, run the below command:
```
$ git add -u  
```

## Add Files by Wildcard
Git allows us to add all the same pattern files at once. It is another way to add multiple files together. Suppose I want to add all java files or text files, then we can use pattern *.java* or *.txt*. To do so, we will run the command as follows:
```
$ git add *.java  
```
The above command will stage all the Java files. The same pattern will be applied for the text files.
