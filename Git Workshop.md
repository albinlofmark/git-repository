# Git Workshop
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