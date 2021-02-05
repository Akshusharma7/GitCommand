# BRANCH

### Branching:
> Timeline of commits, by default branch is master, we can create several branch from master branch

### Merge:
> Merge other branch to master

### Fast forward merge:
> Simplest case, like never branched , commits on destination, can be disabled

### Automatic merge:
> Non-conflicting merge detected, preserves both timelines, merge commit on destination

#### Manual Merge:
> Automatic merge not possible, conflicting merge state, changes saved in merge commit

> List of all branches: Note: “*” here means current branch name
##### git branch


##### cat > web.txt
First line

##### git add .
##### git commit -m comment1 .

> Create new branch “dev2” and its pull all file data from master branch
##### git checkout -b dev2
##### cat >> web.txt
Second line

> Commit data in current branch “dev2”
##### git commit -m comment2 .

> Switch to master branch
##### git checkout master

##### Note: 
> You wont able to see, data commit in “dev2” branch. If you want to pull data from “dev2” branch and merge in master branch. Its will do fast forward merge
##### git merge dev2

> Delete branch:
##### git branch -d dev2

##### -------------------------
> Manual Merge - Conflicting merge resolution:

##### cat > app.txt
Data1

Data2

##### git add .
##### git commit -m com1 .

##### git checkout -b dev2
##### vim app.txt

Changes data1 to newdata(in first line)

##### git commit -m com2 .

##### git checkout master
##### vim app.txt
Changes data1 to masterdata(in first line)

##### git commit -m com3 .

##### git merge dev2
Its shows error auto merging conflict

### Note: For this we have to do manual merge, for this we can use any merge tool like p4merge, etc

### ------------------------------------------------------------------

> Setup SSH protocol to github for authentication, that give u passwordless authentication:
  At workstation, where we have local git repo, create private and public ssh key :
#### ssh-keygen

