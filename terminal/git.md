  #### Creating and interacting with Remote GitHub Repository in Terminal

  - First, create repository on github.com that is the exact name of the directory the project is in
  - While in root repository directory in terminal, enter command `git remote origin master`. This makes the current directory the origin.
  - Command `git add -p` stages parts of a changed file, instead of the entire file. More [here](https://gist.github.com/mattlewissf/9958704)
  - Command `git add --all` adds all changes in the working directory to the staging area but does not yet commit it. 
  - Command `git add file1.txt test.rb trial.py` adds only these 3 files to the staging area
  - Command `git commit -m "describe changes here"` packs all the staged files into a commit and lets you write a commit message. The commit will then be added to remote  repository once pushed.
  - Command `git push origin master` pushes all changes to the remote repository master branch.
  - Command `git clone <repo url>` will clone the entire remote repository from the URL to your local directory. You can then push back to the master, or make a separate branch and commit or push to the branch.
  - Command `git checkout -b <username>` will make a new branch for a repository. Run this in your local repository to create a new branch. You can then `git push origin <username>` to push to your remote branch rather than `git push origin master` which would overwrite the master branch.
  - Command `git pull origin master --no-edit` works the same as `git fetch <remote>` followed by `git merge <remote>/<branch>`. It will pull and merge changes from the remote repository with your local repository. In our weekly homework problems, it pulls in the new weeks directory without changing local previous and existing week directory edits.

---
  - *Some addtional commands and source [here](https://dev.to/juni/git-and-github---must-know-commands-to-make-your-first-commit-333c)*
  - *Tutorials [here](https://www.atlassian.com/git/tutorials/setting-up-a-repository)*
  - *Great StackOverflow Explanation of fetch, merge, and pull [here](https://stackoverflow.com/questions/21756614/difference-between-git-merge-origin-master-and-git-pull)*
  
