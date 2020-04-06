# Pull Changes from a Remote Repository

If you are working on a project which is served from a remote repository, it is likely that you or someone has made changes to the remote copy. In order to incorporate those changes into your local copy of the repository, you need to _pull_ them down.

💡 _It is always good practice to pull down the changes made to the remote repository to your local copy before starting work. This will save you from creating unpleasant merge conflicts!_

To pull down the changes made to the remote copy of the repository, run the following command:

	git pull origin branch-name
	
Here, replace `branch-name` with the branch that you are working on. 

For instance, a good practice is to start on the `master` branch, run `git pull origin master`, then create a new branch for your new work.