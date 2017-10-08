# Git & Github
* Install git on Ubuntu
`sudo apt-get install git`
* Create a directory, Initiate a new repository 
`git init`
* Add file to the stage, every time you modify the file and want to commit it to the repository
`git add <file>`
* Commit modified files to the master with comment, every time you modify the file and want to commit it to the repository
`git commit -m "Description"`
* Set user email, for the first use
`git config --global user.email "you@email.com"`
* Set user name, for the first use
`git config --global user.name "Your name"`

=====================
* Examine the status of the repository
`git status`
* Examine change to the file
`git diff <file>`

=====================
* Examine commit logfile [only display one line for each]
`git log [--pretty=oneline]`
* Display every command
`git reflog`
* Move master pointer the version "commit id" HEAD points to master
`git reset --hard HEAD^(commit id)`

=====================
* Go back to the version not added or committed (unstage)
`git checkout -- <file>`
* Go back from stage to unstage
`git reset HEAD <file>`

=====================
* Delete file from repository
`git rm <file>`
* Mistakenly delete file from workspace, recover from repository
`git checkout -- <file>`

=====================
* Setup relation between local repository and remote repository
`git remote add origin git@github.com:jwtty/repo-name.git`
* Push all the files in local repository to remote repository
`git push -u origin master`
* Push file to remote repository every time committing local files
`git push origin master`
* Clone a local repository from remote repository
`git clone <path>`

=====================
* List all the branches
`git branch`
* Create a branch
`git branch <name>`
* Change to branch <name>
`git checkout <name>`
* Combination of the above two commands
`git checkout -b <name>`
* Merge branch <name> to the current branch
`git merge <name>`
* Delete a branch
`git branch -d <name>`
* Do not use Fast Forward to merge 
`git merge --no-ff -m "Comment" <name>`

=====================
* push local modification to removal repository
`git push origin branch-name`
* update local repository
`git pull`
* "no tracking information"
`git branch --set-upstream branch-name origin/branch-name`
* View remote info
`git remote -v`
* Create local branch corresponding to remote branch
`git checkout -b branch-name origin/branch-name`


**Reference:**
 https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/00137583770360579bc4b458f044ce7afed3df579123eca000

