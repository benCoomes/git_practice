# all about git

## [git log](https://git-scm.com/book/en/v2/Git-Basics-Viewing-the-Commit-History)
#### git log shows commit history
* git log --patch
  * show the diffs for each commit
* git log -5
  * show only the 5 most recent commits
* git log --stat
  * show files that were changed and how much
* git log --pretty=\[options\]
  * format the output as desired. 
* git log -S \[search string\]
  * show only commits where 'search string' was added or removed
* git log --author "authorName"
* git log --oneline --graph --decorate
  * shows commits on a single line, a graph of branches, and information about branches and remotes

## git commit
#### git commit records the changes in your staging area

## [git remote](https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes)
#### git remote can be used to view and manage remote repositories
* git remote -v
  * show remote repositories and their associated URLs
* git remote add \[name\] \[\url\]
  * add a remote repository
* git remote rename \[oldname\] \[newname\]
* git remote remove \[name\]
* git remote show \[name\]
  * show details about a remote

## git pull
#### git pull fetches and merges the remote branch that your repository is tracking, if any

## git fetch \[remoteName\]
#### git fetch downloads objects and references from another repository

## git push \[remoteName\] \[branch\]
#### git push uploads your objects and references to another repository

## [git tag](https://git-scm.com/book/en/v2/Git-Basics-Tagging)
#### use git tag to specify important points in commit history, such as versioned releases. You can create annotated tags, which have metadata are are stored as full git objects, or lightweight tags that only point to a specific commit. 
* git tag
  * list the available tags
* git tag \[pattern\]
  * only list tags that match the pattern
* git tag -a \[tagName\] -m \[tagMessage\]
  * create an annotated tag with a message for the most recent commit
* git tag -a \[tagName\] \[checksum\]
  * tag the commit with the matching checksum. The provided checksum can be partial as long as it is unique.
* git show \[tag\]
  * display detailed information about the commit pointed to by the tag
* git push \[remoteName\] \[tag\]
  * push the tag to a remote server. Tags are not pushed automatically.
* git checkout \[tag\]
  * checkout a tag. This puts your repository in a detached HEAD state. 

## git branch
#### use branches to work on features or bug fixes before merging them into the main branch
* git branch \[name\]
  * create a new branch called 'name'
* git checkout \[branchName\]
  * switch to an existing branch by moving HEAD to the 'branchName' branch. You will not be able to switch if you have uncommitted changes in your working directory or staging area that conflict with the branch that you are switching to. 
* git checkout -b \[branchName\]
  * create a new branch and switch to it
* git merge \[branchName\]
  * merge branch 'branchName' with your current branch
* git branch -d \[branchName\]
  * delete a branch