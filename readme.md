# Git & Github
Install git on Ubuntu
	sudo apt-get install git
git init // Create a directory, Initiate a new repository 
git add <file> // Add file to the stage, every time you modify the file and want to commit it to the repository
git commit -m "Description" //Commit modified files to the master with comment, every time you modify the file and want to commit it to the repository
(git config --global user.email "you@email.com") // Set user email, for the first use
(git config --global user.name "Your name") // Set user name, for the first use

git status // Examine the status of the repository
git diff <file> // Examine change to the file

git log [--pretty=oneline] // Examine commit logfile [only display one line for each]
git reflog // Display every command
git reset --hard HEAD^(commit id) // Move master pointer the version "commit id" HEAD points to master

git checkout -- <file> // Go back to the version not added or committed (unstage)
git reset HEAD <file> // Go back from stage to unstage

git rm <file> // Delete file from repository
git checkout -- <file> // Mistakenly delete file from workspace, recover from repository

git remote add origin git@github.com:jwtty/repo-name.git // Setup relation between local repository and remote repository
git push -u origin master // Push all the files in local repository to remote repository
git push origin master // Push file to remote repository every time commiting local files

git clone <path> // Clone a local repository from remote repository

git branch // List all the branches
git branch <name> // Create a branch
git checkout <name> // Change to branch <name>
git checkout -b <name> // Combination of the above two commands
git merge <name> // Merge branch <name> to the current branch
git branch -d <name> // Delete a branch
git merge --no-ff -m "Comment" <name> // Do not use Fast Forward to merge 

git push origin branch-name // push local modification to removal repository
git pull // update local repository
git branch --set-upstream branch-name origin/branch-name //"no tracking information"
git remote -v // View remote info
git checkout -b branch-name origin/branch-name // Create local branch corresponding to remote branch


Reference: https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/00137583770360579bc4b458f044ce7afed3df579123eca000
