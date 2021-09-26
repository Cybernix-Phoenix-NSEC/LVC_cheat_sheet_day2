# Git-Learning Version Control Cheatsheet Day-2
This repository contains the cheat sheet for the Day 2 session of Git-Learning Version Control. Fork it and you are good to go 💻 !

## Advanced Git Commands

### Git log Commands
- **git log --oneline** : This command converts each commit in one line
- **git log --graph**   : Shows graph of commits. Red dotted line shows the parent commit and gren line shows child commit
- **git log --stat**    : Include which files were altered and the relative number of lines that were added or deleted from each of them.
- **git log -p**        : To show changes in file in every commit.
- **git log -n**        : To show last n number of commits
- **git shortlog**      : to check which author makes how many commits.
- **git shortlog -n**   : to sort author with their quantity of commits.
- **git shortlog -n -s**: to show summary of author with commits.
- **git shortlog -n -s -e** : to show emails of every author
- **git log --author = “author name”**   : filtering commits by author name 
- **git log --grep =”message”**          : filtering commits by message
- **git log --merges**                   : to show all merge commits
- **git log --no-merges**                : to show all non merge commits
- **git reflog**                         : to show all operations in a repositary
- **git reflog show name**               : to show all operations in a particular branch 'name'

### Git Branch Commands
- **git branch name**                    : to create a new branch 'name' in repositary.
- **git branch -d name**                 : to delete a branch 'name' from repositary.
- **git checkout name**                  : to shift HEAD pointer in 'name' branch.
- **git checkout -b name**               : to create a new branch and shift Head pointer directly in name' branch.
- **git push origin name**               : to push the changes in 'name' branch.
- **git push origin name -f**            : to push the changes in 'name' branch forcefully.

### Git reset Commands
- **git reset id**                         : resets the branch to the commit 'id'.
- **git reset --soft id**                  : resets the branch to the commit 'id' and all the files related to this commit are in staged area.
- **git reset --hard id**                  : resets the branch to the commit 'id' and all the files are totally deleted.
- **git reset HEAD~n**                     : resets last n number of commits.

### Git revert Commands
- **git revert id**                        : to perform inverse operation of this commit and create a new commit.

### Git rebase Commands
- **git rebase -i id**                     : merge commits and open a new window. In that window pick is used for main commit and squash is used for all commits which are merging.
- **git reset --hard upstream/main**       : reset all branches from upstream to origin

### Git stash commands
- **git stash**                            : it is used to store file in temporary memory.
- **git stash pop**                        : it is used to take back all files from temporary memory.
- **git stash clear**                      : it is used to delete all files from temporary memory.

### Git diff Commands
- **git diff HEAD**                        : show difference between working directory and last commit.
- **git diff --cached**                    : show difference between stagged changes and last commit.

### Git pull Commands
- **git pull name**                        : fetch the recent copy of branch 'name' and immediately merged it into the local copy.
- **git pull origin main**                 : fetch all changes from main branch to fork branch after merging.

### Git merge Commands
- **git merge name**                       : merges branch 'name' to current branch

### Git push commands
- **git push origin name**                 : to push all the file into the branch 'name' from local copy
- **git push origin name -f**              : to push all the file into the branch 'name' from local copy forcefully

### Git fetch commands
- **git fetch --all -prune**                : fetch all the branches from upstream.

### Git commit commands
- **git commit --amend -m**                 : to modify last commit.
- **git commit --amend --author**           : to modify author of last commit.
- **git cherry-pick id**                    : insert commit of commit 'id' into another branch.
