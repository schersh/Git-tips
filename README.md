# Git-tips

GitHub is a great resource for version control and collaborating with teams! The following offers a brief index of frequently used commands, as well as links for further learning.

##Frequently used git commands:
$ git init
* Initializes new directory and tells Git to start monitoring the current folder you're in (do not use this command w/in your home directory)

$ git add .
* adds changes in working folder to be staged for next commit. You can also specify a specific path to a directory/file. Some refer to adding your changes as "staging" them for a commit.

$ git commit -m "commit message here"
* Commit all staged files to the timeline.  -m option allows you to include a message describing changes. You can think of a commit as a "snapshot" of your project at that specific moment in time. Git logs allow you to "time travel" back to a specific commit of your code, which can be very helpful for debugging!

$ git push origin master
* Sends local changes to tracked remote repository

$ git push origin [name of branch]
* Sends local changes to a specific branch of the remote repository

##Common git commands for branching:
$ git checkout [newBranch]
* starts monitoring new branch

$ git checkout -b [newBranch]
* creates and starts monitoring new branch

$ git -av
* shows all existing branches on github  

$ git status
* Shows the status of project and changes made

##Common git commands for collaborating on a repo:
$ git clone http://path/to/repo
* creates a new local git repo copied from a remote one

$ git remote add origin / upstream master [url]
* adds a remote or upstream master so that can pull in new changes to keep your local copy up-to-date

$ git remote -v
* shows a list of all the existing remote repositories for the working directory

$ git pull upstream master
* pulls updates from upstream repo

$ git merge master
* This command can be used while you are working in the feature branch to merge feature into master. (The "master" branch should always be the most updated, perfect, version of the project, so if working on a group project, you wouldn't merge a feature into master without a code review/consultation with your collaborators.)

$ git merge "name of branch"
* This command can be used while you are working while you are on the master branch, to merge in changes from other branch

* Note: A pull request is like a merge that requires permission from the repo's administrator. You can push your feature branch up, and then submit a pull request via github.


##Helpful Links:

#GitHub Desktop:
* Provides a desktop application interface for users who prefer not to use their terminal command line. Could also be a good resource for PC/Windows users.
https://desktop.github.com/

#Tutorial on Git workflow:
https://guides.github.com/introduction/flow/

#Comparing methods for Git workflow with teams:
https://www.atlassian.com/git/tutorials/comparing-workflows

#Using branches:
https://www.atlassian.com/git/tutorials/using-branches/

#Interactive tutorial on Git branching:
http://pcottle.github.io/learnGitBranching/

#Tutorial on synching:
https://www.atlassian.com/git/tutorials/syncing/

#Working with remote repositories:
https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes

#Merging versus Rebasing:
https://www.atlassian.com/git/tutorials/merging-vs-rebasing/conceptual-overview
