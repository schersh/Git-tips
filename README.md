# Git-tips

Frequently used commands:
$ git init
    Initializes new directory and tells Git to start monitoring the current folder you're in (do not use this command w/in your home directory)
$ git add .
    adds changes in working folder to be staged for next commit. You can also specify a specific path to a directory/file.
  Adds your changes to be included in your next commit
$ git commit -m "commit message here"
    Commit all staged files to the timeline.  -m option allows you to include a message describing changes
$ git push origin master
    Sends local changes to tracked remote repository
$ git push origin [name of branch]
    Sends local changes to a specific branch of the remote repository

Commands for branching:
$ git checkout [newBranch]
    starts monitoring new branch
$ git checkout -b [newBranch]
    creates and starts monitoring new branch
$ git -av
    shows all existing branches on github  
$ git status
    Shows the status of project and changes made





Helpful tutorial on synching: https://www.atlassian.com/git/tutorials/syncing/
