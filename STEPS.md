Steps to start a new project on github with node.js
===================================================

Dependency
----------
git - a distributed version control system.
node.js - An evented non-blocking javascript for serverside.
npm - package manager for node.js.


Steps for dummies
-----------------

Create a directory to hold a project structure.
	mkdir wordgame
Go into the project directory and initialize the git repository.
	cd wordgame
	git init
Create some files using `touch` command. Here, we have created a README.md file,that will have basic information about the project for anybody interested.
	touch README.md
Once again we are listing out all the steps in STEPS.md, in order to get a project started.
	touch STEPS.md
Use vi or your fav text editor to put the content inside your files.
	vi README.md

After the changes you should, ritually, check what has been changed and hence, probabbly, worth saving (aka a commiting) in your code repository.
	git status
You should get a output which is similar to this ...
	# On branch master
	#
	# Initial commit
	#
	# Untracked files:
	#   (use "git add <file>..." to include in what will be committed)
	#
	#	README.md
	#	STEPS.md
	nothing added to commit but untracked files present (use "git add" to track)
The outout is saying that there are two files, README.md and STEPS.md which are not tracked for changes by git. But, we know these file are very much part of our project and worthy of being versioned.So, let's tell git to start tracking 'em.
	git add README.md STEPS.md

Once, we have added the files, lets check back what would be the output of for the command `git status`. Type in 
	git status
The output should be now ...
	# On branch master
	#
	# Initial commit
	#
	# Changes to be committed:
	#   (use "git rm --cached <file>..." to unstage)
	#
	#	new file:   README.md
	#	new file:   STEPS.md
	#










