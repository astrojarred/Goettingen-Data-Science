# Introduction to Data Science — Day 1
### Jarred Green, Feb 19, 2018
#data #Göttingen #notes #datascience

## Introduction —
* Course times: 9:15 - 11:45, 12:45 - 17:00
* Exam: presentation + 

## Introduction to Git
* Our Jupiter hub: https://jupyter.gwdg.de/

* What is git?
	* `git` is a version control system
	* it records snapshots of a _repository_ (a directory with stuff in it
	* these snapshots are called _commits_
	* each commit records the entire state of the repository
	* a sequence of commits forms a _branch_
	* branches are encouraged and can be merged
* History and git commits
	* commits are identified by their hash
	* SHA1 protocol
	* deterministic hashes -> same input gives same hash
	* a commit contains
		* hash of entire working directory, metadata, and commit-has of its parent(s)
		* so if you change any part of the history, then all hashes of the following commits will change
	* great for writing a thesis in latex :) 
* git commands:
	* git init -> starts a repository (but there’s a more normal way)
	* git add filename.md -> adds a file to your repository
	* git status -> tells you which files have changed
	* git diff -> tells you what changed since last commit
	* git commit -> commits but opens text editor
	* git commit -m ‘your message’ -> commits without editor
* stats of files
	1. Committed files (no changes) -> not shown
		* `git add <file>` -> adds the changes of filename to the staging area
	2. Untracked files or uncommitted changes to tracked files -> red
		* `git reset`
	3. Files or changes in the staging area (part of next commit) -> green
		* `git checkout -- <file>`

TEST CHANGE