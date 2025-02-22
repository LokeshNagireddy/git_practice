# This document provides the frequently used git cli commands and their purpose.

**What is Git?**
*Git is a free and open-source distributed version control system, which is designed to
handle everything from small to very large projects with speed and efficiency*

**Git Workflow**
![Git Workflow]
/git_practice/git_work_flow.png

## Git commands
**git clone**
*git clone is a command which is used to clone or copy a target repository*

syntax:

To clone a repository: `git clone <repo_url>`
To clone from a specific branch: `git clone -b <branch_name> <repo_url>`

**git branch**
*A Branch is created to do and keep your changes until they are ready to merge.*
```
To create a branch: `git branch <branch_name>`
To move to a branch: `git checkout <branch_name>`
To delete a branch in local: `git delete -d <branch_name>`
To delete a branch in remote: `git push origin --delete <branch_name>`
```

**git checkout**
*git checkout is used to know the current branch you are in and change to other branches*
```
To create or change to a new branch: `git checkout -b <branch_name>`
To change to a specific tag: `git checkout tag <tag_name> <branch_name>`
```

**git status**
*git status is mainly used to display the state of the staging area and the repository. It
helps us to track all the changes made, point out untracked files.*

Syntax: `git status`

**git commit**
*Git commit is used to record all the changes in the repository.The git commit will
commit all the changes and make a commit-id for the same for tracking down the changes.*
```
To commit with a meaningful message (unstaged files): `git commit -m "message"`
To commit with a message for staged files: `git commit -am "message"`
To edit the last commit : `git commit -amend`
```

**git rm**
*Git rm is used to remove a collection of files from working tree or index*

Syntax: `git rm <file-name>

**git merge**
*git merge allows you to merge branches from Git. It preserves the
complete history and chronological order and maintains the context of the branch.*

Syntax: `git merge <branch_name>`

**git rebase**
*git rebase is a process of combining a sequence of commits to a new base commit*
> The primary reason for rebasing is to maintain a linear project history.
> When you rebase, you ‘unplug’ a branch and ‘replug’ it on the tip of another branch(usually main).
> The goal of rebasing is to take all the commits from a feature branch and put it on the main branch.

Syntax: `git rebase <branch_name>`

**git fetch**
*git fetch is only downloads new data from a remote repository, but it doesn’t integrate
any of the downloaded data into your working files. All it does is provide a view of this data.*

Syntax: `git fetch <branch_name>`

**git pull**
*git pull command will pull the changes from remote repository to local repository and immediately updates the content in local*

Syntax: 
```
To pull from current branch: git pull
To pull from a different branch to current branch: git pull <remote-name><branch_name>
```

**git stash**
*git stash allows you to move to a different branch without commiting on current branch.*
Syntax: 
```
To create the stash: git stash
To view all the stashed changes: git stash list
To drop a stash: git stash drop <stash_id
To delete all the stashes : git stash clear
```

**git ignore**
*At times, there are some files that we might want Git to ignore while commiting. For
example, private files or folders containing passwords, APIs etc. These files are userspecific and hence, we can ignore these using the .gitignore.
.gitignore is generated automatically inside the project directory and ignores the files to get committed to the repositories.*

## Advanced Concepts.
`git pull --rebase`
*With git pull --rebase , the unpublished changes will be again applied on the published changes and no new commit will be added to history.*

**git merge --squash**
*The squash along with git merge produces the working tree. It indexes in the same way as that of the real merge but discards the merge history.*

`git merge --squash origin/main`
