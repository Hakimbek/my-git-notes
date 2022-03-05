# Git Index
The Git index is a staging area between the working directory and repository. It is used to build up a set of changes that you want to commit together. To better understand the Git index, then first understand the working directory and repository.

There are three places in Git where file changes can reside, and these are working directory, staging area, and the repository. To better understand the Git index first, let's take a quick view of these places.

### Working directory
When you worked on your project and made some changes, you are dealing with your project's working directory. This project directory is available on your computer's filesystem. All the changes you make will remain in the working directory until you add them to the staging area.

### Staging area
The staging area can be described as a preview of your next commit. When you create a git commit, Git takes changes that are in the staging area and make them as a new commit. You are allowed to add and remove changes from the staging area. The staging area can be considered as a real area where git stores the changes.

Although, Git doesn't have a dedicated staging directory where it can store some objects representing file changes (blobs). Instead of this, it uses a file called index.

### Repository
In Git, Repository is like a data structure used by GIt to store metadata for a set of files and directories. It contains the collection of the files as well as the history of changes made to those files. Repositories in Git is considered as your project folder. A repository has all the project-related data. Distinct projects have distinct repositories.

You can check what is in the index by the git status command. The git status command allows you to see which files are staged, modified but not yet staged, and completely untracked. Staged files mean, it is currently in the index. 

As we mentioned earlier index is a file, not a directory, So Git is not storing objects into it. Instead, it stores information about each file in our repository. This information could be:

- mtime: It is the time of the last update.
- file: It is the name of the file.
- Wdir: The version of the file in the working directory.
- Stage: The version of the file in the index.
- Repo: The version of the file in the repository.

And finally, Git creates your working directory to match the content of the commit that HEAD is pointing.
