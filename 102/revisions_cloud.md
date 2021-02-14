# Revisions and the Cloud

## Version Control
* Version control allows for the recording of changes
  * Local version control (VCS) is based on a database on a hard disk that stores changes to files
  * Centralized version (CVCS) allows for version control on a local server so multiple clients       can acces it
  * Distributed version control (DVCS) is similar to CVCS but allows for back ups in multiple         locations so that a server failure does not result in a loss of all files and changes

## Git
  * Git is a form of DVCS that stores snapshots of files
  * Git relies on local operations
  * Git is able to track every single change applied to a file or directory
  * Git helps minimize the possibility of irreversible damage to files
  * Files in Git can reside in three main states: committed, modified, and staged
    * Committed means data is securely stored in a local database
    * Modified means a file has been changed but not committed
    * Staged flags a files changed version to be committed
  * Git Help can be accessed through three ways
    * ```git help command```
    * ```git command --help```
    * ```man git-command```
    
## Git Functions
  * Importing
      * ```cd test```
        ```git init```
        ```git add *.c```
        ```git add LICENSE```
        ```git commit -m "any message"```
  * Cloning
    * ``` git clone https://gihub.com/test```
  * Workflow
    * Working Directory
    * Index
    * Head
  * Saving Changes
    * Tracked 
    * Untracked
  * File Status
    * Flagged
    * Staged
    * Modified
    * To check status ```git status```

## A.C.P. Add, Commit, Push
  * ```git add filename```
  * ```git commit -a```
  * ```git push origin main```
  
## Git Functions Continued
  * Stashing changes allows for an inbetween before you commit but want to save
    * ```git stash``` followed by ```git stash apply``` when ready to retrieve       changes
  * Remote repositories
    * Cloned Repositories
    * Seeing Remote Repositories
      ```git remote``` and ```git remote -v```
  * Fetching allows for pulling data from a remote project
    * ```git fetch [remote-name]```
  * Pushing allows for adding your changes to the remote repository
    * ```git push [remote-name][branch-name]```
  * Renaming and removing remotes is possible
  * You can undo commit mistakes, unstage a file, undo a committed snapshot, or unmodifying a file
  
## Branching
  * Branches of a central repository allows for multiple people to work on a project with others without modifying the main repository
  * You can create a new branch
  * Switch between branches
  * List branches
  * Merge branches
  * Delete branches
  * Merge conflicts
  * Preview changes
  * See latest commits for any branch

## Rebasing
  * Rebasing is an alternative to merging branches
  * Allows for polishing of commit histories

## Logs, Tagging, Aliases
  * Logs allow you to see committed snapshot histories
  * Tagging allows for marking important points in a project
    * Tags can be lighweight or annotated
    * Tags must be pushed to be shared
  * Aliases allows for easier navigation and can be set up using git config

[Home](README.md)
    
  
        
  
