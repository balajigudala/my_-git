# my_-git

git clone https://github.com/balajigudala/new.git                           --> for master branch 

git remote add origin https://github.com/YOUR.git                           --> to add our remote repo link.

git branch -a                                                               --> to show all the branches

git branch <name>                                                           --> to create a new branch

git branch -d <name>                                                        --> to delete the purticular branch (-D) for force deletion.

git checkout                                                                --> to move from one branch to another branch. 

git checkout <branchname>                                                   --> to move to the specific branch.

git checkout <commitid>                                                     --> to jump to specific commit.

git checkout -b <branchname>                                                --> to create a new branch and move on to the branch.

git clone -b <branch name> https://github.com/balajigudala/new.git          --> for specific branch.

git fetch --all                                                             --> to get other branches after cloning a single branch.

git add <files>                                                             --> to add the local changes to the staging area.

git commit -m <commit message>                                              --> to add our staged files to local repo.

git log                                                                     --> to show the commit history.

git log --oneline                                                           --> shows the log in one line.

git show <commit id>                                                        --> show the info of all changes for the commit

git pull                                                                    --> pulls the master branch from the local repo.

git pull origin <branch name>                                               --> to pull the branch from the local repo

git merge <brnh1> <brnh2>                                                   --> to merge the two branch data (no deletion of data is done).

git push                                                                    --> to push the master branch changes to remote repo.

git push -u origin <branchname>                                             --> to push the branch changes to the remote repo.

git push -d origin <branchname>                                             --> to push the deleted branch changes to the remote repo.

git reset --soft HEAD~                                                      --> to delete the last commit.

git restore <filename>                                                      --> restore the file as the file in local repo.

git diff <filename>                                                         --> shows the changes of file that have done after the last commit.

git format-patch -1 <commit-id>                                             --> generate the patchfile(lastcommitname.patch) based on the commit id.

git apply <patch file name>                                                 --> to apply the patchfile data to the files where ever it requires.

git apply -R <patch file name>                                              --> revert the changes made by the patch file.

git apply --check <patch file name>                                         --> to verify the patch file appliable to our files or not.

git apply --stat <patch file name>                                          --> for status of patch to our repo.

git commit --amend                                                          --> helps to modify the commit message.

git revert HEAD                                                             --> to modify the last commit changes to previous 
                                                                                https://sentry.io/answers/revert-a-git-repository-to-a-previous-commit/
                                                                                git revert HEAD~3...HEAD --> to modify the last three commits
git reset --hard HEAD~                                                      --> to delete the last commits 

git stash                                                                   --> if you modified the pulled repo and don't won't the files in working repo and not to commit it
                                                                                then we push this files to stack(a secret storage).
                                                                                git stash list --> shows the files in stack.
                                                                                git stash apply --> to add files to the working directory from stack.
