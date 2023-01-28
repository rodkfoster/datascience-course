# Using git to manage your Intuit class materials

Git is a version control system that tracks changes and versions across your files. GitHub is a company that follows git protocol to easily enable team collaboration on coding projects (akin to the "Dropbox for code").

This guide walks you through the steps you need to take to manage your class materials, as well as submit your projects.

# Step-by-step for obtaining new class materials
## Step 1: Identify the repository of interest

Using your browser, navigate to the GitHub repository that contains the materials you are seeking. This may be the current day's lesson or a given project/assignment.

## Step 2: Open a Terminal, navigate to your local course materials location

Now, on your own computer, open a new Terminal. (Within JupyterLab, launch Terminal by clicking on `+` in the upper-left then selecting Terminal. Or, launch a native Windows terminal by pressing Win-R and typing `cmd`.) Using the command line, navigate to the location on your own machine to where you want to have your local copy of the class materials. Recall that you will use `cd` to navigate between directories. (You will likely do something like `cd ds_class`) Remember to use `dir` (or `ls` on Mac) to check out the current files/folders as you navigate on your local machine.

## Step 3: Clone the repository

To edit the class materials, you must move these materials from their remote location (which is GitHub) to a local location (your own computer). 

So, return to your browser to see your newly created repository. The upper left should say something like 'danielwilhelm/CURRENT_LESSON_NAME'.

Click the "Clone or download" green button. Copy the URL available to you.

Now, run the following command in your Terminal: `git clone REPO_URL`, where REPO_URL is what you are pasting. If you want to store the repo in a directory other than the default, run: `git clone REPO_URL DIRECTORY_NAME`.

## Step 4: Open the day's materials

Now, in your Terminal, `cd` into the new folder you recently cloned to your local machine. Launch Jupyter Lab by typing `jupyter lab`. (Or, you can launch Jupyter Notebook by typing `jupyter notebook`.) Voila!


# Step-by-step for saving your changes locally
At the conclusion of class (or a working session), you will need to save, commit, and push your changes. That is, you want to save the changes you made and be sure those changes are reflected on a remote location so that you can easily use them in the future.

## Step 1: Click 'Save' in your Jupyter Notebook

In the notebook where you're currently working, click the Save icon in the upper left corner (ish) area. Alternatively, use the keyboard shortcut Ctrl-S (or Cmd-S on Mac).

## Step 2: Add materials to the staging area

Open a new Anaconda prompt. Navigate to the materials on your local machine that you are currently working on. (This may look something like `cd ds_class\NAME_OF_CURRENT_LESSON`). It is important that you navigate into the folder of the current material's lessons.

Once inside the folder that contains the file (a Jupyter notebook, likely) you are working on, we tell git to take a look at the file's changes via adding that file to the staging area. To add a file to the staging area: `git add NAME_OF_FILE`.

## Step 3: Commit these changes to the git log

Now that the file of interest is in the staging area, we want to commit the changes we have made to our log of changes using git. When we commit these changes, we also want to provide a short note describing the changes we have made.

To do so, we type `git commit -m "DESCRIBED CHANGES"`, where you describe the changes you're making inside the quotations. The file's changes have now been logged.


# Step-by-step for submitting your work (projects)
To submit your work, you will complete what is called a "pull request". In typical development cycles, it is commmon that you would be submitting your changes back to the central project. (Imagine if you created a new feature but did not edit the rest of the broader application. You wish to have this feature incorporated back to the larger project.) The process by which you submit changes back to the master directory is called a "pull request".

In our case, your pull request will be you saying, "Hey! Check out the changes I made to the project", where your changes will be the completed exercises. Unlike a real world development cycle, your instructors will not incorporate your pull request (known as "merging"), but instead simply close your pull request. Your instructors are not incorporating your changes because we do not seek to incorporate your answers into the GA materials -- rather, we want to check your answers, and then close (or deny) your pull request. Nonetheless, the pull request you created is a signal that says, "I'm done! Take a look"

Submitting a pull request is all conducted through the browser.

## Step 1: Fork the project
Instead of cloning the project repo directly to your computer, you must first make a copy of the repo into your own Github account. This is called making a "fork". This will allow you to store your commits back to Github.

In the upper-right corner of a given repository you are viewing (i.e. a project repo), you should see three buttons: Watch, Star, Fork. You want to click "Fork" on the repository. GitHub will then ask you where you want to fork, and your given GitHub username should appear as the only option. Select this, and proceed.


## Step 2: Clone your fork of the repository
Now return to your browser to see your newly created repository. The upper-left should say something like 'YOURGITHUBUSERNAME/CURRENT_LESSON_NAME' and below that "FORKED FROM danwilhelm/CURRENT_LESSON_NAME". It is essential that you are about to clone **your fork of the materials** rather than the GA copy of the materials. Now run `git clone` as described above and edit the materials as needed.


## Step 3: Be sure all your changes are pushed to GitHub
Once you've made some progress on your project, follow the process above to commit your work to your local git repo. To push all of your local commits (completed exercises) to Github, run `git push`.


## Step 4: Navigate to the repo of interest
In your browser, navigate to your fork of the repository of interest. For example, if you are submitting project one, you will login into GitHub, navigate to YOUR profile (upper righthand corner of GitHub), and select the repository "unit-1_project". (Because you navigated to this project via your collection of repositories, this is your fork.)


## Step 5: Open the pull request
In the upper lefthand portion of the repository, there is a button that says "Pull requests". Select it.

You will then see a green button in the upper righthand corner that says "New Pull request". Click this button.


## Step 6: Add a comment and submit!
Add a comment in the space that appears (e.g. "Completed the project!") and then click Submit. You're done! Your instructors will now receive a notifcation that you completed the project, review your work, and close the pull request after they have done so.
