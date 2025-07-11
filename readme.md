description of spork
md stands for markdown

#Heading: Personal Notes I Took While Learning Github
##Subheading 

"git clone git@github.com:hicazi2/spork.git" creates a copy of the repository in the folder we are working on.
"git status" command shows all of the files that were been updated or created or deleted. 
"git add ." tracks all files before commiting 
Alternatively, we can use "git specific.extension" command for tracking a specific file. 
' git commit -m "title" -m "description" ' is the command for commitment. There has to be a title.
e.g. 'git commit -m "title of the message" -m "second -m is for the description of the message"'

Note: Commitment is done locally. The changes aren't live on github yet. use "git push" to push the changes online.

##Git Branching
Main Branch: Main branch you are working on
Feature Branch: Something like a sandbox area that you are experimenting something unfinished.
Hotfix Branch: A bug fix branch that comes from the main branch and merges back to it.

"git branch" shows the branch status. It should return something like "* main". * Means you are currently on that branch.

"git checkout BRANCHNAME" allows you to switch between branches but it won't work if the modified file isn't commited.
To create a new branch, we can use 'git checkout -b "title-of-the-branch" '
"git merge master" pulls the updates of the main branch from online repository because it is better to not get too far behind to not make merging harder each time.

##Merging
"git diff BRANCHNAME" shows the difference between branches 
...

##Undoing in git

"git reset HEAD~1" allows you to delete last commit.
There is no direct way to undo more than one commit in github.
But it is possible to see the commit log with "git log"
Commits are differentiated with hashes.
"git reset HASHNUMBER" unstages all of the commits after the HASHNUMBER commit log. 

Note: PR stands for pull request.
Note: -u is a shortcut for "--set-upstream"

"git branch -d BRANCHNAME" deletes the BRANCHNAME branch after merging because usually previous branches won't be used in the future.

'git commit -am "message" ' can be usd for both adding and commiting with a message. This works only for modified files and not for newly created files.

##Forking in git
If we want to work on other repositories that we don't have full authorization, we fork that repository from the owner to our profile.

