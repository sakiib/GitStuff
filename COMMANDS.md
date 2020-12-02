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