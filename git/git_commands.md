** git config user name and user email : **
git config –global user.name “[name]”
git config –global user.email “[email address]” 

** create a new repo **
git init

** fetch existing repo from url **
git clone <repo_url>

** display all existing branches in repo **
git branch

** display all existing branches with information **
git branch -vv

** delete feature branch **
git branch -d <branchname>

** checkout existing branch or create if not exist **
git checkout -b <branchname>

** checkout non existing branch **
git checkout <branchname>

** switch to local branch **
git switch <branchname>

** get the status of files in local **
git status

** get the difference which are not staged **
git diff -staged

** add file to staging **
git add <file>
git add *

** commit with message **
git commit -m "message"

** removes the file from working directory and stages deletion **
git rm <file>

** get the version history for the current branch. **
git log

**  metadata and content changes of the specified commit **
git show

** add tag to commit **
git tag <commitid>

** merge specic branch into the current branch **
git merge <branchname>

** push committed changes of local branch to remote branch **
git push origin master 
git push -u origin <branch>
git push -all 

** pull changes of remote to local **
git pull 

** to store the tracked files in temp location **
git stash save

** to get the files which are stored in temp location **
git stash pop
git stash apply

** get list of all stashed changes **
git stash list

** delete stashed changes **
git stash drop

** reset the commit but keeps the data **
git reset <commit hash>
git reset --HARD (discard the last commit with data)
git reset --MIXED (discarding the last commit and file will be in local not in stage)
git reset --SOFT ( discarding last commit, but files will be present in the stage)

**Git cherry-pick is a helpful command. It's a robust command and allows you to pick any commit from any branch and apply it to any other branch **

git cherry-pick <commit-hash>

References :

https://dzone.com/articles/top-20-git-commands-with-examples