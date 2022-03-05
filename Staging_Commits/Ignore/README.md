# Git Ignore
In Git, the term "ignore" is used to specify intentionally untracked files that Git should ignore. It doesn't affect the Files that already tracked by Git.

Sometimes you don't want to send the files to Git service like GitHub. We can specify files in Git to ignore.

The file system of Git is classified into three categories:
### Tracked:
  - Tracked files are such files that are previously staged or committed.
### Untracked:
  - Untracked files are such files that are not previously staged or committed.
### Ignored:
  - Ignored files are such files that are explicitly ignored by git. We have to tell git to ignore such files.

Generally, the Ignored files are artifacts and machine-generated files. These files can be derived from your repository source or should otherwise not be committed. Some commonly ignored files are as follows:

- dependency caches
- compiled code
- build output directories, like /bin, /out, or /target
- runtime file generated, like .log, .lock, or .tmp
- Hidden system files, like Thumbs.db or.DS_Store
- Personal IDE config files, such as .idea/workspace.xml

## Git Ignore Files
Git ignore files is a file that can be any file or a folder that contains all the files that we want to ignore. The developers ignore files that are not necessary to execute the project. Git itself creates many system-generated ignored files. Usually, these files are hidden files. There are several ways to specify the ignore files. The ignored files can be tracked on a .gitignore file that is placed on the root folder of the repository. No explicit command is used to ignore the file.

There is no explicit git ignore command; instead, the .gitignore file must be edited and committed by hand when you have new files that you wish to ignore. The .gitignore files hold patterns that are matched against file names in your repository to determine whether or not they should be ignored.
