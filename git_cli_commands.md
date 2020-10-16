# Common Git CLI commands

## create a local repository on your computer (if repository is not on GitHub yet)
1. Create a directory and give it a name
2. Cd into the repository
3. enter: git init

## Syncing your remote repository to your local repository (if you have first created a local repository on your computer and then a GitHub repository)
git remote add origin url

## Clone a repository (Take Repository from internet and download a copy onto computer)
git clone <url>


## Add a file to be tracked the next time I save
git add <filename>

##Track all of the files in a respository
git add .

## Save the state of the files that have been tracked
git commit -m "message about which changes you made"


## Track all of the files that have been changed and commit them
git commit -am "message about which changes you made"

## What is currently happening within Git repository
git status


## Push change in repository to GitHub
git push


## Download latest version of the repository that currently exists on GitHub (if GitHub ahead of local repository)
git pull


## See all the changes you have made in the repository
git log


## Reset current state of your local repository
git reset --hard <commit hash> #Reset to older version with this commit hash
or
git reset --hard origin/master #reset to version that is currently on GitHub


#Branching

## Current state of your local repository is represented by the HEAD

## Tell me which type of branch I am currently on
git branch


## Create a new branch and change HEAD to this branch
git checkout -b <new_branchname>


## Change HEAD to existing branch
git checkout <branchname>


## Merge master branch and a feature branch together
git checkout master
git merge <feature branch>

##Delete a branch locally on your computer
 git branch -d <branch>
