#Git Practice

You will be practicing git commands and how you should use git to work on a project.


1. Fork this repository.  Once it is forked, you have a copy that is all yours.


2. In your workspace, clone your repository.  Find the `Clone or download` green button on your repository in GitHub.  Hit Copy to clipboard.  Go to command line.  Type `git clone ` and hit paste.

	`git clone git@github.com:username/some_repository_name.git`

	You should be pulling down these files locally.

	Open up this README locally and read along.


3. Checkout and create a new branch.

	`git checkout -b variable`

4. Open the variables.md file.  Type in an example of a variable.  Save and close the file.

5. Now use git to save this difference.

	`git add .` to stage all files for committing.
	`git commit -m "Adds an example of a variable"` to commit the change

6. To see your commit, type `git log`, and you should see your commit and the difference you made to the file.

7. Now pull down master, in case there were changes.  Then merge with master.  Checkout master.  And merge your new branch with master.

	`git pull origin master`
	`git merge variable-example master`
	`git checkout master`
	`git merge master variable-example`

8. Push your changes up to GitHub, on both branches.

	`git push origin master`
	`git push origin variable-example`

9.  Awesome!  You are a Git ninja!  Now, do steps 3-8 for the rest of the Core4!  The last Core4 element is missing!  Create that file yourself. :)

	loops.md
	functions.md







#Core4 practice




#Example Workflow

1. Clone a repository

	`git clone git@github.com:username/some_repository_name.git`

2. Create and checkout a branch

	`git checkout -b myBranch`

3. Make a change and save it.

4. Add the changed files

	`git add .`

5. Commit the change.

	`git commit -m "Made my first change"`

6. Repeat steps 4-5 until your a small day's work is done and tested.

7. Pull down changes.

	`git pull origin master`

8. Merge your branch with any changes you pulled down from master.

	`git merge myBranch master`

9. Checkout master.

	`git checkout master`

10. Merge master with your branch to close your branch.

	`git merge master myBranch`

11. Push your changes so that others can see them.

	`git push origin master`
	`git push origin myBranch`



#Glossary

The commands you will learn today are:


 - git clone

	`git clone git@github.com:username/some_repository_name.git`

	This command allows you to copy a repository that you already have on GitHub and copy it locally.


 - git status

	`git status`

	This command allows you to see the status of your local files and whether they have changed or are staged for a commit.


 - git add

	 `git add .` or `git add file.js`

	 This command will allow you to stage the changes to all files, so that they are _ready_ to commit.  It will not commit any files.


 - git commit

	`git commit -m "Centers heading 1 text"

	This command will _commit_ the changes you have made.  It will create a _commit message_ that says 'Centers heading 1 text', so that people can see what you were doing.  


 - get checkout

	 `git checkout -b newBranch` to create a new branch or `git checkout newBranch` if it already exists.

	 Master is the default branch.  But you should create and work on new branches, so that you don't inject code that is not tested into Master for other people.  Each person works on a branch.  Then you merge your branch into master when your code is tested and ready.


  - git pull

	 `git pull origin branch_name`

	Before you do a merge, you should pull down changes from GitHub to make sure you aren't missing any changes.  You must _pull_ before you _push_.


  - git merge

	`git merge newBranch master` when you are merging master _into_ your branch (newBranch is checked out).
	`git merge master newBranch` when you are _closing_ your branch (master is checked out).

  - git push

	`git push origin branch_name`


