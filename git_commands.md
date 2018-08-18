# Git Commands

## Create
### To create a new git repository
`git init`

### To configure git
This will track your changes as coming from you.  
`git config --global user.email "your@email.com"`  
`git config --global user.name "Your Name"`
## Add
### To add a new file to the staging environment
`git add <file name>`  
Example -  `git add git_commands.md` will add the file *git_commands.md* to the staging environment
### To add all of the files to the staging environment
`git add .`

## View
### View status of repository
`git status`

### To see the commits that have been made
This will allow you to see who made the commit, when the commit was made, a special hash (sequence of random numbers) for each commit, and the message attached to the commit.  
`git log`

### Exit git log
`q`    


## Commit
### To commit a change
`git commit -m "initial commit"`  
`-m` will allow you to add a message to your commit. Add your message in quotes. This should be a description of the changes you made.

## Roll back
### To revert to an old commit state
`git checkout <desired commit number>`

## Branching
 Branches are basically an alternate reality for your work, separate from the main "master" branch. You can create a branch to experiment with some changes without it affecting your main "master" branch.
### To create a new branch
This will create a new branch as a snapshot of the current state of the branch you are in when you create it. Any changes you make in this branch moving forward will only exist here until you actively merge them somewhere else.  
`git branch <name of branch>`

### To see the branches that currently exist
`git branch`  
The asterisk in the response (if you have more than one branch) denotes which branch you are currently in

### To move between branches
`git checkout <name of branch you want to work on>`

### To merge branches
Navigate to the branch you want to add the commits to  
`git checkout <name of branch you want to push commits to>`

Then, merge in the changes from the branch you want to take the commits from  
`git merge <name of branch you want commits from>`

### Rename branch
`git branch -m <original name> <new name>`

## Remove
### To delete staged changes (or revert back to previous saved state)
This will move your changes from being staged to just being tracked.
`git checkout <file name>` for single document
`git checkout .` for all documents

### To remove changes from staging area
This will make it as if you never staged those changes.
`git reset HEAD <file name>`

### To delete a file completely
This will delete the file, as well as push the deletion into the staging environment
`git rm <file name>`

### To delete a branch
`git branch -d <name of branch you want to delete>`


## Work with Remotes
### To share share (or "push") your local changes to the remote server

---

# Terminal Commands
## To see what directory (folder) you are currently in
`pwd` which stands for "print working directory"
## To see the items in a directory
`ls`

## To see all items in a directory, including hidden items
`ls -la`

## To empty the screen
`clear`
