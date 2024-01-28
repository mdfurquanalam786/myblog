# Git and Github

### Checking git version
```git
git --version
```

### Setting up user name
```git
git config --global user.name "name of user"
```
Name must be written under `double brackets` if it contains any space between them, if not then write them without quotes.

### Setting up user email
```git
git config --global user.email "email of user"
```

### How to Add VS Code to the system PATH
1. Go to C:\Program Files\Microsoft VS Code (Here, you will find code.exe)
2. Copy the path
3. Paste it in Enviroment VAriables System PATH

### How to open VS Code from git bash
```git
code
```

### Setting up the default editor: VS Code
```git
git config --global core.editor "code --wait"
```
- By default, our editor is Vim : when you type the only command before double quotes it will give you nothing which means that our default editor is Vim
- Here this is the wait floag '--wait' to tell the terminal to wait until we close vs code instance (that particular tab).

### To edit all the global settings
```git
git config --global -e
```
It will open .gitconfig file in vs code

### Configuring End of Lines
```git
git config --global core.autocrlf true
```
- As we know that in Windows we have Carriage Return(cr) and Line Feed(lf) at the end of a line but only Line Feed(lf) in macos and linux so when differenct operating system work together we need to configure our end of lines so that we won't get any error in future.
- and need to set to input for macos system

### Git help
```git
git config --help
```
- It will open a html help page for you.

```git
git config -h
```
- It will open : short summary of commands on git bash

### Creating a directory
```git
mkdir (directory name)
```

### Changing Directory
```git
cd (directory name)
```

### Changing Drive
```git
cd (Drive:)
```

### To initialize new git repository
```git
git init
```
Message: Initialized empty Git repository in 'path'

### To list all files and directories
```git
ls
```





