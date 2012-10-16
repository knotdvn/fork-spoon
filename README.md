All that's missing is the fork. Heh.

SU ITS OPSS SPIDERS git / GitHub Tutorial
=========================================

This is a simple tutorial covering the spiders usage of git and github.

Please view the visual reference folders, to see diagrams which explain aspects of this tutorial.

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

	-type: mkdir git
	(this creates a folder on the desktop called git)

	-type: cd git
	(you are now in that folder)

	-type: git clone [the url of your git repo]
	(see note in step 2 example: https://github.com/knotdvn/fork-spoon.git ) 

	-this downloads the repo into your current directory, you now have the repo files on your machine.


4. Modify and save changes to your repo.

	-open the fork-spoon folder in the file browser.
	(from your desktop click on the git folder, then the fork-spoon folder)

	-open the proof folder

	- create a new text file in this folder
	(right click add new document, YOURNAME.txt, see others for example)

	-open this text file, add some text to it, save file
	(example: "I did it!")

	-back in the terminal, type: cd proof
	(you're now in the proof folder)

	- type: git add YOURNAME.txt
	(whatever your file was called,)
	this adds the file to gits list of file which belong in the repo.

	-type: git stage YOURNAME.txt
	this tells git to include your files changes in the repo

	-type: git commit -m "I added my file"
	(-m stands for message) its a useful tag for identifying what the commit did, you will have lots of commits in a repo

	-at this point your local repo on you machine is saved 

	-type: git push origin master
	this sends your local repo "origin" to the repo you cloned  


	

	









