Example Workflow
====
This is the example we went though during the git revisited seminar.  

###Getting started:
***>>>fork VIC repo***

    git clone git@github.com:{your_user_name}/VIC.git
    cd VIC

### Review the repo that you just cloned

    git status
    git branch
    git branch -a
    git log

### Add the upstream repo
    git remote -v
    git remote add upstream git@github.com:UW-Hydro/VIC.git
    git remote -v

### Fetch the upstream branches
    git fetch upstream
    git branch -a

### Merge in the changes from the upstream develop branch
    git checkout develop
    git merge upstream/develop  -X theirs

### create a new feature branch
    git checkout -b feature/testing
    git branch -a
    git status

### make changes to repo
    vim .gitignore 

### do a git stash to move around a dirty repo
    git stash
    git pull upstream develop
    git stash apply
    git log

### stage some changes
    git add .gitignore

### review the changes
    git status
    git diff

### commit the changes
    git commit -m "Sample commit message"

### Review the commit
    git status
    git log

### push to github
    git push origin feature/testing

### go to github
- look for new branch
- submit pull request


