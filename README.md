All that's missing is the fork. Heh.

SU ITS OPSS SPIDERS git / GitHub Tutorial
=========================================

This is a simple tutorial covering the spiders usage of git and github.

Please view the diagrams in this repo which explain aspects of this tutorial.

Concept:
--------

git: http://en.wikipedia.org/wiki/Git_%28software%29

Is a revision control system and a program/protocol that runs on your local machine.

GitHub: 

Is a website, which provides a nice graphical interface and social interaction for users of git. GitHub runs git on its servers, and stores code/projects on the web for us to access.

Tutorial:
---------

Requirements:
=============

An individual GitHub account.
git installed on your dev environment.


Welcome! First! 

1. Navigate to the repo on GitHub https://github.com/su-its-op/fork-spoon

	-This is the 'web-view' for the tutorial repository.
	


	

2. Fork the repo to your individual GitHub Account.

	-Click the "Fork" button in the top right of the page.

	-It will ask for confirmation, then create a new repo associated with your account, and copy the exact contents of the original repo into it.

	-*NOTE* Find the Git-Read-Only address of the repo, it should look like this: https://github.com/USERNAME/fork-spoon.git

	All said and done, you have an exact copy of the original, except for the fact that it is seperate and distinct.

	With this repo you can modify the file contents, and not worry about modifying the original repo.

	At this point the repo only exists on GitHub.

	
	
	
3. Clone the repo onto your local machine.

	-open a terminal

	-navigate to a directory where you want your repo in this example we'll use the desktop, but often it will be your wp-content folder if you're developing a theme or plugin.

	-in the terminal type: cd ~/Desktop
	(you are now at the Desktop.)

	-type: mkdir git_demo
	(this creates a folder on the desktop called git_demo)

	-type: cd git_demo
	(you are now in that folder)

	-type: git clone [the url of your git repo]
	(see note in step 2 example: https://github.com/knotdvn/fork-spoon.git ) 
	(git refers to the unix command which runs the git program, clone and the url are paramaters passed to the program)
	(the git program parses its paramaters and decides to "clone the url repo into the current local directory")
	
	-this downloads the repo into your current directory, you now have the repo files on your machine.
	


	
	
4. Modify and save changes to your repo.

	-open the fork-spoon folder in the file browser.
	(from your desktop click on the git_demo folder, then the fork-spoon folder)

	-open the proof folder
	
	-create a new text file in this folder
	(right click add new document, YOURNAME.txt, see others for example)

	-open this text file, add some text to it, save file
	(example: "I did it!")

	-back in the terminal, get to the proof folder in fork-spoon type: cd ~/Desktop/git_demo/fork-spoon/proof
	(you're now in the proof folder)

	-type: git add YOURNAME.txt
	(whatever your file was called,)
	this adds the file to gits list of file which belong in the repo.

	-type: git stage YOURNAME.txt
	this tells git to include your files changes in the repo

	-type: git commit -m "I added my file"
	(-m stands for message) its a useful tag for identifying what the commit did, you will have lots of commits in a repo

	-at this point your local git repo on you machine is saved and up to date,  

	-type: git push origin master
	you will have to provide your GitHub username and password
	this sends your local repo "origin" to the repo you cloned it from "master" 
	
	-navigate your web browser to your GitHub page for the fork-spoon repo you forked.
	example: https://github.com/knotdvn/fork-spoon (use your page not knotdvn!)
	check the file in proof and verify that it exists and was modified.
	
	Congratulations, You can now: [Fork] [Clone] [Add] [Stage] [Commit] and [Push]!
	
	This is the essence of git and GitHub. But there is so much more, Now lets update the
	SU-ITS-OP Repo so it too stores our proof file.
	




5. Update SU-ITS-OP with your individual Forked repo
	
	-Navigate with the web browser to the GitHub page for your individual forked repo
	example: https://github.com/knotdvn/fork-spoon (use your page not knotdvn!)
	
	-Click on the pull request button,
	(top of page next to unwatch)
	
	-Make sure that the two repos are positioned like this:
	SU-ITS-OP/fork-spoon  <-  knotdvn/fork-spoon (use your page not knotdvn!)
	(this indicates the flow, from your fork back to the original)
	
	-Give your pull request a TITLE, and write a little message.
	this message will be seen by a senior developer who will approve the request
	try to give a meaning full message if necessary, list any major functional modifcations,
	features added, or bugs fixed.
	
	-You can view info about your pull request
	use the Commits tab and the Files Changed tab.
	this is a history of your changes and a color coded representation of the difference between the two repos.
	
	-Click Send Pull Request
	When a senior developer approves your pull request, the SU-ITS-OP repo will contain your
	"proof file". We will know you have completed the tutorial, and are git-competent.
	
	Congratulations! You can now contribute with all of SU-ITS-OP!
	
	
	
Tutorial Timeline	
=================

Try and view the tutorial_timeline.html file. Try and add yourself onto the timeline!


Concepts and Commands
=====================
	
	Here is a short-list of commands and concepts and a short description
	note to read an extensive all text manual type: man git
	
	origin || Your local repo, on your local filesystem
	master || Wherever you cloned your repo from, almost always a ".git" url to GitHub
	fork   || creates a repo just for you on GitHub from a pre-existing repo
	clone  || creates a repo on your local machine from a GitHub ".git" url
	push   || sends changes from one repo to another
	pull   || accept changes sent from another repo
	pull request || ask for a repo to accept changes you made on your fork 
	
	git add -A   || Adds every file in the directory to the git repo, useful when creating a project
	git stage -A || Stages every file in the directory to be ready for commit
	
	git commit -m || updates your local repo with local filesystem changes
	
	git push origin master || updates the master repo with your local repo
	
	git fetch || this updates your origin with any changes found in the master (update)
	
	git fetch ".git url" || this updates your local repo with a GitHub repo 
	
	
	
	
	
	
	
	
	


	
	


	

	









