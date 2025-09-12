- git commands

status
    Shows status of the local repository. This status includes:
        number of local commits that have not been synced with remote (GitHub)
        list of files in local folder than are NOT being tracked by git
        list of files in local folder that have changes that need to be committed
    git status

log
    Returns a list of commits made to a repository, along with basic details about them.
    If a commit or commits are specified, it will list commits reachable from those commits.
    If a commit or commit is specified with a ^ before it, it will exclude those reachable from it.
    git log
clone
    Creates a local copy of the specified remote repository.
    git clone git@github.com:kairoundmountain/CEG3120.git
remote
    Sets the location of the remote repository, where commits are pushed to and pulled from.
    git remote add origin git@github.com:kairoundmountain/CEG3120.git
add
    Adds specified files to the 'index.' Any files not in the index will not be created or changed in the commit.
    git add *
rm
    Removes specified file or files from the index and the working directory unless otherwise specified.
        Will need -f if the file has updates
        --cached flag will remove it only from the index.
    git rm test -f
git commit
