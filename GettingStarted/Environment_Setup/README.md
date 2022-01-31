# Git Environment Setup
The environment of any tool consists of elements that support execution with software, hardware, and network configured. It includes operating system settings, hardware configuration, software configuration, test terminals, and other support to perform the operations. It is an essential aspect of any software.

# The Git config command
Git supports a command called git config that lets you get and set configuration variables that control all facets of how Git looks and operates. It is used to set Git configuration values on a global or local project level.

## Setting username and email id
Setting **user.name** and **user.email** are the necessary configuration options as your name and email will show up in your commit messages.

The username is used by the Git for each commit.
```
$ git config --global user.name "Hakimbek Bahramov"  
```

The Git uses this email id for each commit.
```
$ git config --global user.email  "abduhakim.bahramov@gamil.com"  
```

## Setting editor
You can set the default text editor when Git needs you to type in a message. If you have not selected any of the editors, Git will use your default system's editor.

```
$ git config --global core.editor Vim  
```

## Checking Your Settings
You can check your configuration settings; you can use the **git config --list** command to list all the settings that Git can find at that point.

```
$ git config --list  
```

# Git configuration levels
The git config command can accept arguments to specify the configuration level. The following configuration levels are available in the Git config.

- local
- global
- system
