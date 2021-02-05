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

