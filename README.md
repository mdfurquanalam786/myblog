# myblog

### Checking git version
```git
git --version
```

### Setting up user name
```git
git config --global user.name 
```
**Note:** Name must be written under `double brackets` if it contains any space between them, if not then write them without quotes.

### Setting up user email
```git
git config --global user.email
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
**Note:** 
- By default, our editor is Vim : when you type the only command before double quotes it will give you nothing which means that our default editor is Vim
- Here this is the wait floag '--wait' to tell the terminal to wait until we close vs code instance (that particular tab).

### To edit all the global settings
```git
git config --global -e
```
**Note:** It will open .gitconfig file in vs code







