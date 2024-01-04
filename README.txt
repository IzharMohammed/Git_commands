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

