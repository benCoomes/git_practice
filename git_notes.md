# all about git

## [git log](https://git-scm.com/book/en/v2/Git-Basics-Viewing-the-Commit-History)
#### git log shows commit history
* git log --patch
  * show the diffs for each commit
* git log -5
  * show only the 5 most recent commits
* git log --stat
  * show files that were changed and how much
* git log --pretty=\<options\>
  * format the output as desired. 
* git log -S \<search string\>
  * show only commits where 'search string' was added or removed
* git log --author "authorName"