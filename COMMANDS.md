Git Command-Line Fundamentals
============

### Terminal Commands:

| Command | Description |
| ------- | ----------- |
| `ls` | lists all of the folders |
| `ls -la` | lists all of the files |
| `cd ..` | returns one directory back |
| `cd <dirname>` | enter a directory with "dirname" |
| `.` | just install in the current directory |

### On initial install:

| Command | Description |
| ------- | ----------- |
| `git --version` | checks the version of the locally installed git |
| `git config --global user.name "Your Name" ` | sets up the name of the user |
| `git config --global user.email "yourname@somemail.eu"` | sets up the mail of the user |
| `git config --list` | lists all the git configurations |

### For initializing the project:

| Command | Description |
| ------- | ----------- |
| `git init` |  initializes the git repo in the current folder           |
| `touch .gitignore` |  created a git ignore file  |
| `git status` |  check working tree - both on the git and on local |

### Add files:

| Command | Description |
| ------- | ----------- |
| `git add -A` | adds all of the files for commiting "including deleted ones" |
| `git add .` | adds all of the files for commiting |
| `git add *` | adds all of the files for commiting |
| `git add -all` | adds all of the files for commiting |
| `git add <filename>` | add specific file with the filename |
| `git add *.<extension>` | add supports regular expressions |
| `git add -u` | will stage the modified and deleted files |

### Remove files:

| Command | Description |
| ------- | ----------- |
| `git reset` | removes files to be commited |
| `git reset somefile.go` | removes somefile.go from the commit preparation |

### Committing:

| Command | Description |
| ------- | ----------- |
| `git commit -m "This is the commit message" ` | -m is used to add message |
| `git commit -am "This is the commit message"` | we don't need to git add separately |
| `git commit -a` | to commit only the modified and deleted files |
| `git commit --amend -m "new message"` | changes the last commits message & also the commit hash |
| `git checkout <filename>` | remove all the changes made to the current file |

### Check log:

| Command | Description |
| ------- | ----------- |
| `git log` | renders commit idx, authors, dates (press q or z) to get out of it |

### Clone a remote repo:

| Command | Description |
| ------- | ----------- |
| `git clone <url> <where to clone>` | clone a repo in the given directory |

### View infor about the repo:

| Command | Description |
| ------- | ----------- |
| `git remote -v` | lists infor about the repo |
| `git branch -a` | lists all of the branches |

### View changes:

| Command | Description |
| ------- | ----------- |
| `git diff` | shows the difference made in the files, green added, red removed |

### Pull before push ALWAYS:

| Command | Description |
| ------- | ----------- |
| `git pull origin master` | always pull before making new commits to remote repo |

### THEN PUSH:

| Command | Description |
| ------- | ----------- |
| `git push origin master` | <origin> name of remote repo <master> the branch that we push to |

### First time push of the branch:

| Command | Description |
| ------- | ----------- |
| `git push -u origin <name of the branch>` | -u coordinates the two branches (local and on server) |

### Create a branch:

| Command | Description |
| ------- | ----------- |
| `git branch <name of the branch>` | creates a branch with the given branch name|

### Checkout a branch:

| Command | Description |
| ------- | ----------- |
| `git checkout <name of the branch>` | current head is moved to the branch |

### Create & Checkout a branch:

| Command | Description |
| ------- | ----------- |
| `git checkout -b <name of the branch>` | created a branch & current head is moved to that branch |

### Merge a branch:

| Command | Description |
| ------- | ----------- |
| `git checkout master` | current head is moved to the master |
| `git pull origin master` | remember to pull before pushing |
| `git branch --merged ` | see which branches are merged |
| `git merge <name of the branch you want to merge>` | merge this branch to master branch |
| `git push origin master` | push the changes to remote repo |

### Delete a branch:

| Command | Description |
| ------- | ----------- |
| `git branch -d <name of the branch>` | this deletes is locally |
| `git branch -a` | check the repo branches |
| `git push origin --delete <name of the branch>` | this deletes it from the repo |

### Inspection & comparison:

| Command | Description |
| ------- | ----------- |
| `git log --summary` | view detailed changes |
| `git log --oneline` | view detailed breifly |
| `git diff [source branch] [target branch]` | preview changes before merging |
| `git diff` | show the changes in the current file |
| `git log --stat` | ome abbreviated stats for each commit |
| `git log --pretty=oneline` | changes the log output to formats other than the default |
| `git log --pretty=format:"%h - %an, %ar : %s"` | allows you to specify your own log output format |
| `git log --since=2.weeks` | limiting log output using --since, --until, --author |

### Renaming files:

| Command | Description |
| ------- | ----------- |
| `git mv <old-name> <new-name>` | renaming a file |

### Add, Rename, Remove, Replace remote url:

| Command | Description |
| ------- | ----------- |
| `git remote add <short-name> <url>` | renaming a file with a short name |
| `git remote rename <old-name> <new-name>` | renaming a remote file with new-name |
| `git remote remove <short-name>` | removing url of a remote file |
| `git remote set-url <short-name> <new.git.url>` | setting a short name for a remote url |
| `git remote set-url origin <url>` | set a new remote origin link to the given url |

### Stashing:

| Command | Description |
| ------- | ----------- |
| `git stash list ` | see stash list(s) |
| `git stash apply` | default take the top one 'stash@{0}' |
| `git stash pop` | pop = apply + drop, take the top stash changes then  delete it |
| `git stash apply stash@{1}` | get back number 2 stash changes |

### Adding .gitignore:

| Command | Description |
| ------- | ----------- |
| `* ` | is used as wildcard match |
| `/` | is used to ignore pathnames relative to the .gitignore file |
| `#` | is used to add comments to a .gitignore file |
| `*.txt` | ignore all text files |
| `git config --global core.excludesfile ~/.gitignore_global` | to add or change your global .gitignore file |

