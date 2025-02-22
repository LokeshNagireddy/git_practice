# This document provides most of the frequently used git cli commands and its purpose.

**What is Git?**
*Answer: Git is a free and open-source distributed version control system, which is designed to
handle everything from small to very large projects with speed and efficiency*

**Git Workflow**
![Git Workflow]
(/git_practice/git_work_flow.png)

## Git commands##
**git clone**
*git clone is a command which is used to clone or copy a target repository*

syntax:

To clone a repository: `git clone <repo_url>`
To clone from a specific branch: `git clone -b <branch_name> <repo_url>`

**git branch**
*A Branch is created to do and keep your changes until they are ready to merge.*

To create a branch: `git branch <branch_name>`
To move to a branch: `git checkout <branch_name>`
To delete a branch in local: `git delete -d <branch_name>`
To delete a branch in remote: `git push origin --delete <branch_name>`

**git checkout**
*git checkout is used to know the current branch you are in and change to other branches*

To create or change to a new branch: `git checkout -b <branch_name>`
To change to a specific tag: `git checkout tag <tag_name> <branch_name>`

** git status**
*git status is mainly used to display the state of the staging area and the repository. It
helps us to track all the changes made, point out untracked files.*

Syntax: `git status`
