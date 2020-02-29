  #### Creating and interacting with Remote GitHub Repository in Terminal

  - First, create repository on github.com that is the exact name of the directory the project is in
  - While in root repository directory in terminal, enter command `git remote origin master`. This makes the current directory the origin.
  - Command `git add -p` stages parts of a changed file, instead of the entire file. More [here](https://gist.github.com/mattlewissf/9958704)
  - Command `git add --all` adds all changes in the working directory to the staging area but does not yet commit it. 
  - Command `git add file1.txt test.rb trial.py` adds only these 3 files to the staging area
  - Command `git commit -m "describe changes here"` packs all the staged files into a commit and lets you write a commit message. The commit will then be added to remote  repository once pushed.
  - Command `git push origin master` pushes all changes to the remote repository



  *Some addtional commands and source [here](https://dev.to/juni/git-and-github---must-know-commands-to-make-your-first-commit-333c)*
