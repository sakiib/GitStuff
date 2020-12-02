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
| `git add -A` | adds all of the files for commiting |

### Remove files:

| Command | Description |
| ------- | ----------- |
| `git reset` | removes files to be commited |
| `git reset somefile.go` | removes somefile.go from the commit preparation |

### Committing:

| Command | Description |
| ------- | ----------- |
| `git commit -m "This is the commit message" ` | -m is used to add message |

### Check log:
| Command | Description |
| ------- | ----------- |
| `git log` | renders commit idx, authors, dates |

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

