# Git Workshop

**Task 1: Initialize a New Repository, Create Files, and Make Commits**
1. Create a new project folder and initialize a Git repository.
 - Change directory to desired folder. For example: cd C:\Users\cowbo\OneDrive\Dokument
 - Make a directory to store files: mkdir "Programing"
 - Change to directoty where you want to store the files: cd Programing
 - Initialize a Git repository: git init

2. Create a few files with different content.
 - Make a .md file to edit in VSCode: code "Git Workshop.md"

3. Stage and commit the files with descriptive messages.
 - Edit it how you want in VSCode then save it and add it to the staging area: git add "Git Workshop.md"
 - Commit the changes to the repository and a "commit message": git commit -m "File Updated"

4. Make additional changes to the files and commit them.
 - Edit the file in VSCode and save the file. Then you can add it to the staging area and commit it at the same time: git commit -a -m "Update 2"

5. Restore one of the files to a specfic verision in the repository.
 - Use "git log" to see the different commit and then copy the first 5 or 6 characters of the first commit and restore it: git restore --source=c924ad Git Workshop.md

**Task 2: Connecting to a Remote Repository**
1. Create a remote repository on a Git hosting service.
 - Go to GitHub on your browser and create a new repository, give it a name and a description.

2. Add the remote repository to your local project.
 - Copy the SSH link of your remote repository in GitHub and connect it to your local repository: git remote add origin git@github.com:albinlofmark/git-repository.git

3. Push all local changes to the remote repository.
 - Make sure you have commited everything you want to push to your remote repository then use the following command: git push origin master 
 - "Master" in the command above could also be "Main" if you are on a newer version of Git.

**Task 3: Working with Branches**
1. Create a new branch called feature-branch.
 - To create a new branch you use the following command: git branch feature-branch

2. Switch to the new branch.
 - To switch to the new branch you write: git switch feature-branch

3. Make changes and commit them.
 - To make changes you simple edit the desired .md file and use the following command to add the changes to the staging area and commiting them: git commit -a -m "branch update"
 - You can also merge the branch with main/master by first switching back to the main/master branch then using the following command: git merge -m "info regarding branch merge with master" feature-branch
 - When you are done with the merge you can delete the feature-branch by using the following command: git branch -d feature-branch

4. Push the new branch to the remote repository.
 - To push the new branch to the remote repository you can must first make sure the changes are added to the staging area and commited then you can use the following command: git push origin feature-branch

**Task 4: Cloning and Updating a Remote Repository**
 1. Clone the following repository: https://github.com/Lexicon-Smaland/Hello-World
 - Click the link above and press "Code" then copy the HTTPS link.
 - To clone the remote repository use the following command: git clone https://github.com/Lexicon-Smaland/Hello-World

*Now you have got a feel for the basics of Git as well as local and remote repositories!*