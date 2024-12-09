# Git Basics

## Git Commands

### Configuration
`git config --global user.name "Your Name"` <br>
* Set your username in git
* Replace "Your Name" with your name

`git config --global user.email "Your email"` <br>

* Set your email in git
* Replace "Your email" with your email

`git config --list` <br>
* List all the configurations

<br></br>
### Repository
`git init` <br>
* Initialize a git repository
* Run this command in the directory where you want to create a repository
* This command will create a hidden directory named `.git` in the directory

`git clone <repository-url>` <br>
* Clone a repository from a URL
* Replace `<repository-url>` with the URL of the repository

<br></br>
### Changes

`git add <file_name>` <br>
* Add a file to the staging area
* Replace `<file_name>` with the name of the file

`git add .` <br>
* Add all the files to the staging area

`git commit -m "commit message"` <br>
* Commit the changes
* Replace `"commit message"` with the message you want to add to the commit

`git commit -am "commit message"` <br>
* Add all the files to the staging area and commit them

`git commit --amend -m "new commit message"` <br>
* Change the commit message of the last commit or add more changes to the last commit

<br></br>
### Status and Logs
`git status` <br>
* Show the status of the repository and : 
  * Files that are staged, unstaged, and untracked
  * The branch you are currently on
  * Files that are ignored <br>

**options** : -s, --short, -b, --branch, --show-stash, --ignored

`git log` <br>
* Show the commit history
* Press `q` to exit the log

**options** : --oneline, --graph, --all, --decorate, --author, --since, --until, --grep, --pretty, --stat, --patch

<br></br>
### Branching and Merging
`git branch` <br>
* List all the branches in the repository

`git branch -a` <br>
* List all the branches in the repository including the remote branches

`git branch <branch_name>` <br>
* Create a new branch

`git checkout <branch_name>` <br>
* Switch to a branch

`git checkout -b <branch_name>` <br>
* Create a new branch and switch to it

`git branch -d <branch_name>` <br>
* Delete a branch (Should be in another branch)
* use `-D` instead of `-d` to force delete a branch

`git merge <branch_name>` <br>
* Merge a branch into the current branch

`git merge --abort` <br>
* Abort the merge process

<br></br>
### Rebase
`git rebase <branch_name>` <br>
* Rebase the current branch on top of another branch
  (Moves the BASE of the current branch to the HEAD of another branch)

/* use `rebase` to re-anchor your feature branch to keep up with the latest changes. <br>
then use `merge` to move those changes back onto shared branches. */


<br></br>
### Remote Repository
`git remote` <br>
* List all the remote repositories