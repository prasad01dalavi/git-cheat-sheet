# Git Tutorial
Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later.

 Git has three main states that your files can reside in: committed, modified, and staged:
 1. Committed means that the data is safely stored in your local database.
 2. Modified means that you have changed the file but have not committed it to your database yet.
 3. Staged means that you have marked a modified file in its current version to go into your next commit snapshot.


``` bash
# Know about the git version
git --version

# Setting user for git
git config --global user.name "Prasad Dalavi"
git config --global user.email prasad01dalavi@gmail.com

# Checking your settings
git config --list

# Know the current user
git config user.name
git config user.email

# Help in detail
git help checkout
git help <cmd>

# Quick help
git <cmd> -h

# Initialize the git VCS (Version Control System) 
git init

# Add all files to staging area
git add . 
git add -A
git add --all

# Add particular file or folder to staging area
git add filename
git add foldername

# Untrack the added files (Remove git added files)
git rm --cached <files>

# Commit the files/folder which are at staging area
git commit -m "commit message"

# Get the log of commits 
git log

# Get the graphical representation
git log --graph

# Gives me the commits for the particular author
git log --author="Prasad Dalavi"

# Show me the changes made before adding to staging area 
git diff

# If I want to discard the changes (before going to staging area)
git checkout second.txt
git checkout -- second.txt

# Status of git
git status
git status -s

# Git branching 
git branch  # Shows branches (default is master which is main branch)
git branch branch_name         # Creating new branch
or
git checkout -b branch_name    # Also creates branch
git checkout branch_name       # Switching to branch_name
git checkout master            # Switch back to master branch (to merge other branches)
git merge branch_name          # merge the changes in branch to master branch
git branch -D branch_name      # Delete the branch


```
Good Link for Git Concepts:
https://git-scm.com/book/en/v2
