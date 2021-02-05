# GitCommand
Git commands and use

> Git is decentralized or distributed (DVCS) system but can be used as centralized.

> The Repository : Collection of files managed by git and all version (history)

> Folder where we initialized git or content files in our storage known as Working Directory or workspace.

> Commits : snapshot of file, create a timeline of changes in branch, git repo have atleast one branch known as master branch

> GitHub: git hosting/cloud service for unlimited public repo with no private repo but in business model, we can choose to have private repo also.

> Create GIT repo or initialized git:
##### mkdir myprojects
##### cd myprojects
##### git init demo
##### cd demo
##### ls -a  (there folder .git, that is git repo)

>Set identity to git, that recorded in version log
##### git config --global user.name “prateek.sharma”
##### git config --global user.email “prateek@gmail.com”

>Git States with Local:

Working Directory : all files present in above “demo” folder 

Staging Area : file preparing for commit, first store in staging area, then only we can commit

Repository/Commit History : committed with version or save changes to git repo

> Git States with Remote:

Remote State : repo shared to centralized system like GITHUB

> Show the current status of local repo
##### git status

> Put file in the staging area, without putting file here, we can't create commit history
##### git add test.txt


> Send file to repo/commit area, here we have created snapshot of file means version of file
##### git commit -m “first comment” text.txt

>To check all version of file, every commit they provide commit id
##### git log test.txt

> See details of log
##### git show commitID

> We can use commit id’s to see the diff in 2 version
##### git diff  id1  id2

> Remove git repo
##### rm -rf .git

> Again create git repo in existing project, go to project folder
##### git init

> Add all file in staging area
##### git add .

> Add all file in commit area
##### git -m “comment” commit .

> Create new file, that is not by default tracked by git
##### touch new.txt

> Show tracked file by git
##### git  ls-files

> Staging and Committing file in one command : Express commit
##### git commit -a -m “comment” file.txt

Note: not all version of git support this

HEAD Markers : Special Markers Like pointers, points to last commit of current branch

> How to make file untracked or removed from staging area:
##### git reset HEAD  new.txt

