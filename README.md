# Git Tutorial
Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later.

 Git has three main states that your files can reside in: committed, modified, and staged:
 1. Committed means that the data is safely stored in your local database.
 2. Modified means that you have changed the file but have not committed it to your database yet.
 3. Staged means that you have marked a modified file in its current version to go into your next commit snapshot.


``` bash
# Basics
git --version                                             # Know about the git version
git config --global user.name "Prasad Dalavi"             # Set User name
git config --global user.email prasad01dalavi@gmail.com   # and email
git config --list                                         # Checking your settings
git config user.name                                      # Know the current user name
git config user.email                                     # Know the current user email
git help <cmd>                                            # Help in detail
git <cmd> -h                                              # Quick help
git config --global alias.co checkout                     # Can use co instead of checkout as a short form of checkout

# Using the git VCS (Version Control System) 
git init                              # Initialize the directory as git repo
git status                            # Get detail status of git repo
git status -s                         # Get short status
git add . or -A or --all              # Add all files to staging area
git add -u                            # Add only unstaged files to staging area
git add filename or foldername        # Add particular file or folder to the staging area
git rm --cached <files>               # Untrack the added files (Remove git added files from staging area)
git commit -m "commit message"        # Commit the files/folder which are at staging area
git add forgotten_file                # Redo the commit with forgotten additional changes
git commit --amend                    # Apply the last commit message
git log                               # Get the log of commits 
git log --graph                       # Get the graphical representation
git log --author="Prasad Dalavi"      # Gives me the commits for the particular author
git diff                              # Show me the changes made before adding to staging area 
git checkout second.txt               # If I want to discard the changes (before going to staging area)

# Git Remote
git remote -v                         # Shows the urls for shortnames
git remote show <remote>              # More Info about particular remote
git remote add <shortname> <url>      # Add short names for urls
git remote rename <oldname> <newname> # Rename the remote short name
git fetch <remote>                    # Pulls down all the data from remote doesn’t automatically merge
git push <remote> <branch>            # Push it to upstream
git remote remove or rm <remote>      # Removes all related remote-tracking branches and configuration settings

# Git branching 
git branch                     # Shows branches (default is master which is main branch)
git branch branch_name         # Creating new branch
or
git checkout -b branch_name    # Creates branch and switch to that branch
git checkout branch_name       # Switching to branch_name
git checkout master            # Switch back to master branch (to merge other branches)
git merge branch_name          # merge the changes in branch to master branch
git branch --merged            # Shows merged branches
git branch --no-merged         # Shows not merged branches
git branch -d branch_name      # Delete the branch safely
git branch -D branch_name      # Delete the branch forcefully (when it is not merged so that data will get lost)
git branch -v                  # See the last commit of all branches

# Git Advance
git stash                      # when want to switch branches, but don’t want to commit what have been working on yet 
git stash list                 # See list of stored stashes
git stash apply <stash name>   # Apply the stash


```
Good Link for Git Concepts:
https://git-scm.com/book/en/v2
