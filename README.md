GIT commands
==========

##### Reset all changes to remote master
    git fetch --all
    git reset --hard origin/master

##### Stage changed files
    git add . (stages new and modified, without deleted)
    git add -u (stages modified and deleted, without new)
    git add -A (stages All)

    git reset (removes added)

    git config core.safecrlf false

##### Show content of .gitconfig
    git config --global --edit 

##### Rollback origin master (remove unwanted commits to master, return to commit e3f1e37)
    git reset --hard e3f1e37
    git push --force origin master

##### Overwrite content in branched config.js file with content from config.js on remote master
    git checkout origin/master -- config.js

##### Update branch names from remote
    git fetch origin
    git branch -v -a
