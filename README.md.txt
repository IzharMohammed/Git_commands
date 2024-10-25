1.  `git init` --> Powers your folder to be managed by git and initialises a new empty repositiry . it also crestes a .git folder that has
all relevant logic to manage versions of your project.
2.  `Working Area` --> There can be a bunch of files that are not currently handled by git. It means that changes done or to be 
done in those files are not managed by git yet. A file which is in working area is considered to be not in staging area . when we do 
`git status` and we see a bunch of `untracked files` then these are actually called to be in working area

3.  `Staging area` --> What all files are going to be a part of next version that we will create. This staging area is place where git
knows what changes will be done from last version to next version.

4. `Repository area` --> This area actually contains details of all your previous registered version and the files in this area . git 
already manages them and know their version history

5. `git add<file>` --> moves file from working area to staging area

6. `git rm --cached<file>` --> moves file back from staging area to working area 

7. `commit` --> commit is a particular version of project . It captures a snapshot of projects staged changes and creates a version
out of it.

8. `git commit` --> registers staging changes to commit 

9.  `git log` --> list down all commits of repository . if you want to exit out of git log prompt press `q`

10. git restore <file> -> it removes all files changes from the staging area to be committed. This can be useful, if we did some dirty 
piece of code and now no more want it. Instead of deleting every change line by line, we can restore it or you can say restore last clean version of the file.

11. git restore --staged <file> -> it removes file from changes from staging area to the working area. this only works if changes 
are in your staging area

12. Diff between git rm and git restore ans: if you want to move the whole file back to the untracked state, then we do git rm, otherwise if we just want the 
changes to be moved in working area or staging area then we git restore.

13. git diff commit1 commit2 -> gives the difference of all file changes between two commits

14. git commit -m "<your commit message>" -> If we want to avoid opening a text editor like vim/nano to add commit message we can use this 
following command

15. git remote -> list down all the remote connection names

16. Remote connection -> It helps you to link two git repositories for uploading and downloading changes from each otherwise

17. git remote add <name of remote> <link of the remote> : this command helps us to add a new link to the remote repo and give a name to it


18. If u r contributing to open source then firstly we have to :- 
  - fork a repo
  - git clone `the repo which u have forked in u r github`
  - Search for the issue 
  - create a branch by `git checkout -b "name of the branch"
  - contribute in the new branch and then git add . git commit -m "" and then run cmd 
  git push it will give u a cmd for pushing and then push it from the new branch 
  - Go to u r github  it shows u to compare and create pull request and create a PR.
  - If u owner of the repo merges u r code then issue will be closed but the new changes
  are not in u r main branch its in the owners repo so u have to sync the owners code 
  to u r main branch by these cmds :- 
     - see the total origins by `git remote -v`
     - copy url of the repo from the owners account and then :-  
     - git remote add upstream "copied url from owners repo" and then check the origins 
     - we have to sync the owners repo code with our local code . There are 2 ways :- 
     1:- `git pull upstream main`

     2:-   `git fetch --all`
            `git merge upstream/main`
     - `git push` to push in our local github repo





`git remote add upstream <url of the repo>
git pull upstream main

git push origin main

git checkout -b "abc"

git merge origin main`