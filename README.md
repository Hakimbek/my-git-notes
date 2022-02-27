
# Git
Git is a modern and widely used distributed version control system in the world. It is developed to manage projects with high speed and efficiency. The version control system allows us to monitor and work together with our team members at the same workspace. Git is foundation of many services like GitHub and GitLab. Git can be used privately and publicly.

## Features of Git
### Open Source
  - Git is an open-source tool. It is released under the GPL (General Public License) license.
### Scalable
  - Git is scalable, which means when the number of users increases, the Git can easily handle such situations.
### Distributed
  - One of Git's great features is that it is distributed. Distributed means that instead of switching the project to another machine, we can create a "clone" of the entire repository. Also, instead of just having one central repository that you send changes to, every user has their own repository that contains the entire commit history of the project. We do not need to connect to the remote repository; the change is just stored on our local repository. If necessary, we can push these changes to a remote repository.
### Security
  - Git is secure. It uses the SHA1 (Secure Hash Function) to name and identify objects within its repository. Files and commits are checked and retrieved by its checksum at the time of checkout. It stores its history in such a way that the ID of particular commits depends upon the complete development history leading up to that commit. Once it is published, one cannot make changes to its old version.
### Speed
  - Git is very fast, so it can complete all the tasks in a while. Most of the git operations are done on the local repository, so it provides a huge speed. Also, a centralized version control system continually communicates with a server somewhere.
### Supports non-linear development
  - Git supports seamless branching and merging, which helps in visualizing and navigating a non-linear development. A branch in Git represents a single commit. We can construct the full branch structure with the help of its parental commit.
### Branching and Merging
  - Branching and merging are the great features of Git, which makes it different from the other SCM tools. Git allows the creation of multiple branches without affecting each other. We can perform tasks like creation, deletion, and merging on branches, and these tasks take a few seconds only. Below are some features that can be achieved by branching:
    - We can create a separate branch for a new module of the project, commit and delete it whenever we want.
    - We can have a production branch, which always has what goes into production and can be merged for testing in the test branch.
    - We can create a demo branch for the experiment and check if it is working. We can also remove it if needed.
    - The core benefit of branching is if we want to push something to a remote repository, we do not have to push all of our branches. We can select a few of our branches, or all of them together.
### Data Assurance
  - The Git data model ensures the cryptographic integrity of every unit of our project. It provides a unique commit ID to every commit through a SHA algorithm. We can retrieve and update the commit by commit ID. Most of the centralized version control systems do not provide such integrity by default.
### Staging Area
  - The Staging area is also a unique functionality of Git. It can be considered as a preview of our next commit, moreover, an intermediate area where commits can be formatted and reviewed before completion. When you make a commit, Git takes changes that are in the staging area and make them as a new commit. We are allowed to add and remove changes from the staging area. The staging area can be considered as a place where Git stores the changes.
Although, Git doesn't have a dedicated staging directory where it can store some objects representing file changes (blobs). Instead of this, it uses a file called index.
Another feature of Git that makes it apart from other SCM tools is that it is possible to quickly stage some of our files and commit them without committing other modified files in our working directory.
### Maintain the clean history
  - Git facilitates with Git Rebase; It is one of the most helpful features of Git. It fetches the latest commits from the master branch and puts our code on top of that. Thus, it maintains a clean history of the project.

## Benefits of Git
A version control application allows us to keep track of all the changes that we make in the files of our project. Every time we make changes in files of an existing project, we can push those changes to a repository. Other developers are allowed to pull your changes from the repository and continue to work with the updates that you added to the project files.

Some significant benefits of using Git are as follows:

### Saves Time
  - Git is lightning fast technology. Each command takes only a few seconds to execute so we can save a lot of time as compared to login to a GitHub account and find out its features.
### Offline Working
  - One of the most important benefits of Git is that it supports offline working. If we are facing internet connectivity issues, it will not affect our work. In Git, we can do almost everything locally. Comparatively, other CVS like SVN is limited and prefer the connection with the central repository.
### Undo Mistakes
  - One additional benefit of Git is we can Undo mistakes. Sometimes the undo can be a savior option for us. Git provides the undo option for almost everything.
### Track the Changes
  - Git facilitates with some exciting features such as Diff, Log, and Status, which allows us to track changes so we can check the status, compare our files or branches.


## Getting Started
 - [Git Environment Setup](GettingStarted/Environment_Setup/README.md)
 - [Git Tools](GettingStarted/Tools/README.md)
 - [Git Terminology](GettingStarted/Terminology/README.md)
 - [Git Flow](GettingStarted/Flow/README.md)

## Staging and Commits
 - [Init](Staging_Commits/Init/README.md)
 - [Add](Staging_Commits/Add/README.md)
 - [Commit](Staging_Commits/Commit/README.md)
 - [Clone](Staging_Commits/Clone/README.md)
 - [Stash](Staging_Commits/Stash/README.md)
 - [Git ignore](Staging_Commits/Ignore/README.md)
 - [Fork](Staging_Commits/Fork/README.md)
 - [Repository](Staging_Commits/Repository/README.md)
 - [Index](Staging_Commits/Index/README.md)
 - [Head](Staging_Commits/Head/README.md)
 - [Origin Master](Staging_Commits/Origin_Master/README.md)
 - [Remote](Staging_Commits/Remote/README.md)
 - [Tags](Staging_Commits/Tags/README.md)

## Undoing changes
 - [Checkout](Undoing/Checkout/README.md)
 - [Revert](Undoing/Revert/README.md)
 - [Reset](Undoing/Reset/README.md)
 - [Git Rm](Undoing/RM/README.md)
 - [Cherry-pick](Undoing/Cherry_Pick/README.md)

## Inspecting Changes
 - [Log](Inspecting_Changes/Log/README.md)
 - [Diff](Inspecting_Changes/Diff/README.md)
 - [Status](Inspecting_Changes/Status/README.md)

## Branching and Merging
 - [Branch](Branching_Merging/Branch/README.md)
 - [Merge](Branching_Merging/Merge/README.md)
 - [Rebase](Branching_Merging/Rebase/README.md)
 - [Squash](Branching_Merging/Squash/README.md)
