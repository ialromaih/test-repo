##GIT COMMANDS:
* `git config --global user.name ialromaih`
* `git config --global user.email ialromaih@gmail.com`

##Create_a_repository
* https://github.com/new
* `mkdir ~/test-repo`
* `cd ~/test-repo`
* `git init`
* `git remote add origin https://github.com/ialromaih/test-repo.git`

##To fork:
* fork from the website* `git clone https://github.com/ialromaih/test-repo`

##Create a file
* `add (-u)`: index the file to be monitored
* `commit`: commit the indexed file to your local repo
* `commit -a`: commit a file to local repo without indexing
* `push`: move the file from local repo to github
* `fetch`: move changes from github to local repo
* `pull` or `rebase`: move files from github to workplace
* `Checkout HEAD`: revert changes in local repo
* `checkout`: revert changes for indexed file
* `diff HEAD`: compare local repo with workplace
* `diff`: compared indexed and workplace

##Add these files to be indexed (tracked for changes)
* `git add .`: adds all files.
* `git add -u`: updates tracking for all files that changed name or were deleted.
* `git add -A`: does both the previous.#Commit these changes
* `git commit -m "message"`#Push changes to github:
* `git push`#Create a branch to make changes without affecting others:
* `git checkout -b branchname` --creates a branch
* `git branch` --to see what branch you are on
* `git checkout master` --to switch back to master branch
