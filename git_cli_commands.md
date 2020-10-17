# Common Git CLI commands

## 1. create a local repository on your computer (if repository is not on GitHub yet)
1. Create a directory and give it a name
2. Cd into the repository
3. enter: `git init`

## 2. Syncing your remote repository to your local repository (if you have first created a local repository on your computer and then a GitHub repository)
`git remote add origin <url>`

## 3. Clone a repository (Take Repository from internet and download a copy onto computer)
`git clone <url>`

## 4. Track and Commit Files
### Add a file to be tracked the next time I save
`git add <filename>`

### Track all of the files in a respository
`git add .`

### Save the state of the files that have been tracked
`git commit -m "message about which changes you made"`

### Track all of the files that have been changed and commit them
`git commit -am "message about which changes you made"`

## 5. What is currently happening within Git repository
`git status`

## 6. Push change in repository to GitHub
`git push`


## 7. Download latest version of the repository that currently exists on GitHub (if GitHub ahead of local repository)
`git pull`


## 8. See all the changes you have made in the repository
`git log`


## 9. Reset current state of your local repository
`git reset --hard <commit hash>` #Reset to older version with this commit hash
or
`git reset --hard origin/master` #reset to version that is currently on GitHub


## 10. Branching

### Current state of your local repository is represented by the HEAD

### Tell me which type of branch I am currently on
`git branch`


### Create a new branch and change HEAD to this branch
`git checkout -b <new_branchname>`


### Change HEAD to existing branch
`git checkout <branchname>`


### Merge master branch and a feature branch together
`git checkout master`
git merge <feature branch>

### Delete a branch locally on your computer
 git branch -d <branch>
