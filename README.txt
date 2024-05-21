Steps to connect a local git repo to a remote repo:

1. git init
2. git add. / git commit -a -m "Commit message"
3. git commit -m "Commit message" //This will create a new branch "master"
4. git branch -M "main" // rename branch name to main to sync with origin branch name "main"
5. git remote add origin "url"
6. git push -u origin main //Push the main branch to remote repository