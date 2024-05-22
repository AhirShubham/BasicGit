Steps to connect a local git repo to a remote repo:

1. git init
2. git add. / git commit -a -m "Commit message"
3. git commit -m "Commit message" //This will create a new branch "master"
4. git branch -M "main" // rename branch name to main to sync with origin branch name "main"
5. git remote add origin "url"
6. git push -u origin main
        //tells Git to set up a tracking relationship between the local branch main and
        the remote branch main in the origin repository.
         After setting this upstream relationship, you can simply use git push or git pull without specifying
         the remote or branch names, and Git will know where to push or pull the changes from/to.

7. git reflog // to see the commit history
8. git reset --hard hashId_of_commit // Resets the system to that commit
9.git fetch //to just fetch the remote changes and not merge directly
10. git merge //merge the fetched changes into local repo