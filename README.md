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
- Message: Initialized empty Git repository in 'path'
- .git sub directory will be hidden by default

### To list files and directories 
```git
ls
```
- It will only list all files and directories which are visible

### To list all files and directories
```git
ls -a
```
- Output: ./  ../  .git/
- It will list all files and directories even the hidden one i.e. .git folder

### To open a directory in file explorer
```git
open (folder name)
```
or you can also use 
```git
explorer (folder name)
```

### To delete folder
```git
rm -rf (folder name)
```

### To delete files
```git
rm (file name)
```

### To add files in staging area
```git
git add (file name)
```
- You can add multiple files separated by space
- You can also use patterns: *.txt --> all the files with .txt extension
- You can also use command 'git add .' to add all files in staging area
- Staging area is either the reflection of what we currently have in production, or the next version that is going to go in the production.
- Even after deletion of a file in working directory you need to stage it so that it can also get deleted from the staging area.

### commit command
```git
git commit -m "(commit message)"
```
- To write description: If you only write the command: git commit and press Enter then COMMIT_EDITMSG will get opened in the default editor which is vs code for now where in first line you can write the commit message and then after one line gap you can write its description.

### making and writing in a file
```git
echo (content) > (name of file)
```
- You can use command to append message after creating the file for the first time: echo (content) >> (name of file). This will add (content) in a new line or insertion.
- you can also run this command: echo hello > logs/dev.log It will create a file with dev.log under logs folder only when log folder is previously available.

### Status of the working directory
```git
git status
```

### to change lf to crlf 
```git
unix2dos (file name)
```

### commiting file without staging 
```git
git commit -a -m "(message)"
```
or
```git
git commit -am "message"
```

### Files in staging area
```git
git ls-files
```

### Removing a file from the working directory and staging area
```git
git rm (file name)
```
- you can put multiple files name also and use pattern even.

### Rename/Move a file or directory
```git
mv (old file name) (new file name)
```
### Git command for renaming and moving files
```git
git mv (old file name) (new file name)
```
- After this you not need to run the command : git add . to add new file in your staging area but it will get automatically added with this command.
- So when we use this command (git then after that use of any unix command) the changes get applied to both working directory and the staging area.

### Prevent a folder from tracking
- create a .gitignore file and write the directory or files name which you want to prevent from tracking from the command: echo logs/ > .gitignore
- Open the file in vs code and add file and folders you want to add. You can alsouse patterns.
- .gitignore method only works if we make it before tracking any files or directory means before staging them. Once you stage them adn then add to the .gitignore file it will not work as when you make changes in the file it will see you modified message so in this case you need to unstage them and then add into .gitignore directory.

### Opening a file using VS Code
```git
code (file name)
```

### For help regarding a commah
```git
git rm -h
```

### Removing a file from the staging area
```git
git rm --cached -r (file name)
