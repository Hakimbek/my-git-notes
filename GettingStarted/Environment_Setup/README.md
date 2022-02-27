# Git Environment Setup
The environment of any tool consists of elements that support execution with software, hardware, and network configured. It includes operating system settings, hardware configuration, software configuration, test terminals, and other support to perform the operations. It is an essential aspect of any software.

## The Git *config* command
Git supports a command called git config that lets you get and set configuration variables that control all facets of how Git looks and operates. It is used to set Git configuration values on a global or local project level.

Setting **user.name** and **user.email** are the necessary configuration options as your name and email will show up in your commit messages.

### Setting username
The username is used by the Git for each commit.
```
$ git config --global user.name "Hakimbek Bahramov"  
```

### Setting email id
The Git uses this email id for each commit.
```
$ git config --global user.email  "abduhakim.bahramov@gamil.com"  
```

### Setting editor
You can set the default text editor when Git needs you to type in a message. If you have not selected any of the editors, Git will use your default system's editor.

```
$ git config --global core.editor Vim  
```

### Checking Your Settings
You can check your configuration settings; you can use the **git config --list** command to list all the settings that Git can find at that point.

```
$ git config --list  
```
![config list](/my-git-notes/GettingStarted/Environment_Setup/image/config-list.png)

# Git configuration levels
The git config command can accept arguments to specify the configuration level. The following configuration levels are available in the Git config.

- local
- global
- system

## --local
It is the default level in Git. Git config will write to a local level if no configuration option is given. Local configuration values are stored in **.git/config** directory as a file.

## --global
The global level configuration is user-specific configuration. User-specific means, it is applied to an individual operating system user. Global configuration values are stored in a user's home directory.

## --system
The system-level configuration is applied across an entire system. The entire system means all users on an operating system and all repositories. The system-level configuration file stores in a gitconfig file off the system directory.

The order of priority of the Git config is local, global, and system, respectively. It means when looking for a configuration value, Git will start at the local level and bubble up to the system level.
