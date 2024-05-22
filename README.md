Steps to connect a local git repo to a remote repo:

1. git init
2. git add. / git commit -a -m "Commit message"
3. git commit -m "Commit message" //This will create a new branch "master"
4. git branch -M "main" // rename branch name to main to sync with origin branch name "main"
5. git remote add origin "url"  //link a remote repository with alisa name "origin"
6. git push -u origin main
        //tells Git to set up a tracking relationship between the local branch main and
        the remote branch main in the origin repository.
         After setting this upstream relationship, you can simply use git push or git pull without specifying
         the remote or branch names, and Git will know where to push or pull the changes from/to.

7. git reflog // to see the commit history

8. git log --all --oneline --decorate --graph

9. git reset --hard hashId_of_commit // Resets the system to that commit
10.git fetch //to just fetch the remote changes and not merge directly
11. git merge //merge the fetched changes into local repo

Branching:

1. git switch -c "New Branch Name" --> To create a new branch
2. git switch "branchName"  --> to switch to a branch
3. git merge main  --> merge the main branch into the current branch