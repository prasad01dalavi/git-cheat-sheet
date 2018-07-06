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

# Git help in detail
git help checkout
git help <cmd>

# Git quick help
git <cmd> -h



# Initialize the git VCS (Version Control System) 
git init

# Add all files to staging area
git add . 
git add -A

# Add particular file or folder to staging area
git add filename
git add foldername

# Commit the files/folder which are at staging area
git commit -m "commit message"

# Get the log of commits 
git log

# Gives me the commits for the particular author
git log --author="Prasad Dalavi"

# Show me the changes made before adding to staging area 
git diff

# If I want to discard the changes (before going to staging area)
git checkout second.txt
git checkout -- second.txt

# 

```
Good Link for Git Concepts:
https://git-scm.com/book/en/v2
