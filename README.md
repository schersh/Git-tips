# Git-tips

##Frequently used git commands:
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

##Common git commands for branching:
$ git checkout [newBranch]
    starts monitoring new branch
$ git checkout -b [newBranch]
    creates and starts monitoring new branch
$ git -av
    shows all existing branches on github  
$ git status
    Shows the status of project and changes made

##Common git commands for collaborating on a repo:
$ git clone http://path/to/repo
    creates a new local git repo copied from a remote one
$ git remote add origin / upstream master [url]
    adds a remote or upstream master so that can pull in new changes to keep your local copy up-to-date
$ git pull upstream master
    pulls updates from upstream repo
$ git merge master
    This command can be used while you are working in the feature branch to merge feature into master. (The "master" branch should always be the most updated, perfect, version of the project, so if working on a group project, you wouldn't merge a feature into master without a code review/consultation with your collaborators.)
$ git merge "name of branch"
    This command can be used while you are working while you are on the master branch, to merge in changes from other branch
Note: A pull request is like a merge that requires permission from the repo's administrator. You can push your feature branch up, and then submit a pull request via github.

##The scenario: You're starting a new app. You create a local repo and a repo on Github, create a readme file, and put it on Github. Then you run into Juan, who's already done a lot of the work you were planning to do. You want to pull his code down and include it in your repo, and put your combined code up on your Github repo.

$ git init project-repo
$ cd project-repo
$ git remote add origin git@github.com/username/project-repo.git
$ touch README.md
$ git add .
$ git commit -m "initial commit"
$ git push origin master
$ git remote add juan git@github.com/juan/project-repo.git
$ git fetch juan
$ git merge juan/feature
$ git push origin master

##Helpful tutorial on git workflow: https://guides.github.com/introduction/flow/

##Helpful tutorial on synching: https://www.atlassian.com/git/tutorials/syncing/

##Helpful link on working with remote repositories: https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes
