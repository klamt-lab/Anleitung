# Anleitung
Anleitung zur Benutzung unserer Github Organisation

## Using git from the command line

### Accessing the Repository
* Launch a terminal.
* Navigate to your projects directory `cd ~/MyProjects`.
* If your repository already exist on GitHub, get the clone link from the "Clone or Download" button on the GitHub Repository.
![Clone or Download Button on GitHub](http://i.imgur.com/uScb8xx.png)
* Then, clone your repository by using `git clone [your-copied-url]`
* Once your repository has cloned, you can change to your project directory `cd [your-repository-name]`

### Preparing the Repository
* Now, make sure you are on the correct branch. You can check this branch using `git branch` and looking at which branch is marked with an asterisk.
* **NOTE**: Updating the project from master
  * If you have worked on your project on multiple machines, it is a good idea to update from master before working. To do this, checkout master using `git checkout master`.
  * Now, make sure your master branch is up to date using `git pull`.
  * Checkout your working branch using `git checkout [working-branch-name]`
  * Make sure this branch is up to date with its remote self using `git pull`
  * You can update your working branch from master using `git rebase master`
  * You are now up to date and ready to work!
* To create AND checkout a new working branch, use `git checkout -b [working-branch-name]`
* Now, if your working branch is shown as your active branch, you're ready to get to work!

### Working in the Repository
* Open the code in your editor and begin working. Once you have made a _single logical change_ to the code, it is time to make a commit!
* _Save_ your work before switching to your terminal
* Now, stage your changes using `git add .`
* Commit your changes locally using `git commit -m "[your-commit-message]"`
  * Type a _brief_ (55 characters or less) description of the change you made. 
  * Example: `git commit -m "Create toString method in Student class"`
* Now that your commit is made, you can push these changes to the remote GitHub repository using `git push`
* Repeat this process until your code is complete!

See also [Understanding the GitHub flow](https://guides.github.com/introduction/flow/) and the [Git learning game](https://learngitbranching.js.org/).
