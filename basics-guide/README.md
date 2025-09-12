git commands

status
* Shows status of the local repository. This status includes:
    * number of local commits that have not been synced with remote (GitHub)
    * list of files in local folder than are NOT being tracked by git
    * list of files in local folder that have changes that need to be committed
* git status


log
* Returns a list of commits made to a repository, along with basic details about them.
* If a commit or commits are specified, it will list commits reachable from those commits.
* If a commit or commit is specified with a ^ before it, it will exclude those reachable from it.
* git log

clone
* Creates a local copy of the specified remote repository.
* git clone git@github.com:kairoundmountain/CEG3120.git

remote
* Sets the location of the remote repository, where commits are pushed to and pulled from.
* git remote add origin git@github.com:kairoundmountain/CEG3120.git

add
* Adds specified files to the 'index.' Any files not in the index will not be created or changed in the commit.
* git add *

rm
* Removes specified file or files from the index and the working directory unless otherwise specified.
    * Will need -f if the file has updates
    * --cached flag will remove it only from the index.
* git rm test -f

git commit
* stages all files in the current index as a commit, ready to be pushed to remote.
* git commit -m "Demonstrating multiple commits"

git push
* Sends staged commit to the remote. May encounter merge conflicts.
* git push

git pull
* Gets the latest version of the current branch from the remote. Should be done before beginning any work to ensure local copy is up to date.
* git pull

git branch
* Perform a variety of operations to do with branches.
    * No options: Lists branches.
    * -d: delete a branch
    * -m: move or rename a branch
    * branch name: create a new branch.
* git branch example-branch

git checkout
* Can switch the current branch.
* Can also restore specified files to the state held in the specified branch.
* git checkout example-branch

git fetch
* updates the local histories and branches from the specified repository.
* Does not mess with your working files.
* Must be done before a merge.
* git fetch

git merge
* with no options, mostly equivalent to git push but without the included git fetch.
* Essentially incorporates commits into the current branch.
* Also used to combine or 'merge' branches.
* git merge example-branch
