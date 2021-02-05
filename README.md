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


