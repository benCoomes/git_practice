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
## git pull
#### git pull fetches and merges the remote branch that your repository is tracking, if any

## git fetch \[remoteName\]
#### git fetch downloads objects and references from another repository

## git push \[remoteName\] \[branch\]
#### git push uploads your objects and references to another repository