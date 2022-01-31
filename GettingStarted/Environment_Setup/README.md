# Git Environment Setup
The environment of any tool consists of elements that support execution with software, hardware, and network configured. It includes operating system settings, hardware configuration, software configuration, test terminals, and other support to perform the operations. It is an essential aspect of any software.

# The Git config command
Git supports a command called git config that lets you get and set configuration variables that control all facets of how Git looks and operates. It is used to set Git configuration values on a global or local project level.

## Setting username and email id
Setting **user.name** and **user.email** are the necessary configuration options as your name and email will show up in your commit messages.

The username is used by the Git for each commit.
```git
$ git config --global user.name "Hakimbek Bahramov"  
```

The Git uses this email id for each commit.
```git
$ git config --global user.email  "abduhakim.bahramov@gamil.com"  
```
