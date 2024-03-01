<h1 align="center">Git basics 🌿</h1>
<hr>

## How to track files in git ?
- Firstly, you have to install git in your system. Then create a folder in which you are planning to put the code and files which you have to track.
- Then create a repository in your GitHub account
- open terminal in the folder and type the following commands
		1. `git init`
		2. `git status`
		3. `git add .` - to stage ever files
		4. `git add filename1 filename2` - to stage files 
		5. `git commit -m "Initial commit"`
		6. `git remote add origin <remote_repository_url>` - linking to remote repo which we created in GitHub	
		7. `git push -u origin master` - to push to master or main branch

## Why a master/main branch ??

When two individual devs are working on a single function, they should have an idea about how the current process is in, that is, they should not make random changes inside the project and make it hard for other devs working on a feature. So the master branch gives the idea about the current state of the project and if any new feature is to be added then it is made in sub-branches and after verification it is branched in to the main branch.

Pipeline is triggered whenever feature/bug fix code is merged into master and then
test ⇾ build ⇾ deploy happens.

	we should have one branch for atleast one bug fix or for feature being developed that is the best practice 

- `git branch` - to know which all branches are there currently in the repo
- `git fetch` - to know about the new  branches which are created in the remote repo
- `git remote show origin` - To see remote branches along with their tracking information

- `git checkout <branch name>` - switch working branches  ,if we do this we will have a copy of the main branch and all the changes which we make will be on the duplicate branch.

- `git checkout -b <branch name>` - creating and switching to new branch
- `git branch -m master main` - to make the master branch as main

<hr>

## Pull Request / Merge request

Suppose I have made some changes into my cloned branch, and I need that feature get added to the main/master branch. So in order to make this possible, I need to give a pull request so that the maintainers of the project could validate the code and then merge it if everything is fine. 


<hr>

## Deleting the branches

We can delete a branch from the GitHub or GitLab, and then we have to also delete it locally.
- `git branch -d <branch name>` - delete the branch (we have to do git pull if necessary)


If some changes already been made to the main branch while we were working on a feature by other developers, we have to use `git pull` before we push, because we have to fetch and merge the other changes and then push our changes.

`git pull -r` - where r means rebase, it now pushes our code on top of the previous changes which are being made to the main branch. 


<hr>

## **.gitignore**

Suppose if I have to prevent some files and folders being tracked , i can write them inside this file and it will not be tracked.

1. Create a `.gitignore` file

##### Ignore compiled files
*.class
*.jar
*.war

##### Ignore log files
*.log

##### Ignore build directories
target/
dist/
build/

##### Ignore IDE-specific files and directories
.idea/
.vscode/

##### Ignore system-specific files
.DS_Store
Thumbs.db

##### Ignore configuration files
*.properties
*.config

<hr>

`git stash` - to hide the current changes for later

`git pop` - to un hide the changes which we have stashed

`git log` - to show the commit and its details. The output display will get a commit hash, by each commit will have a unique hash and with the help of it we can go to the older version

`git checkout <hash>` - to go to specific previous version

`git push --force origin <branch-name>` - A normal push (`git push`) adds new commits to the remote branch, preserving existing history. A force push (`git push --force`) overwrites the remote branch's history with your local changes, potentially disrupting collaboration and requiring caution.

`git merge master` - to merge to master branch

### **Undoing commits**

`git reset --hard HEAD~<number of commits to undo>` - undo specific no of commits

`git reset --soft HEAD~<number of commits to undo>` - change will be there but commit is there (we also do not have to write soft, it is default) 

`git revert`- create a new commit that undoes the changes made in a previous commit.
### **Changing commits**
`git commit --amend` - to add the changes with the last done commit



