# Git

**STEP 0: Create a folder (local project)**


**STEP 1: Open Git Bash in that folder**


**STEP 2: Create a file**

     command : echo "# Folder Name" > fileName.txt

     command : ls        (for checking files)


**STEP 3: Initialize Git (local repository)**

     command : git init 

     Creates a hidden .git folder
     Turns this normal folder into a local Git repository
     Git starts tracking changes from now on


**STEP 4: Tell Git which files to track**

     command : git add .                      (adds all file)
               git add FileName.txt           (add specific file)
               git add File1.py File2.md      (add any 2 files)    

    Adds all files in this folder to the staging area
    Prepares them for a commit

     command : git status     (check status)


**STEP 5: Save a snapshot (commit)**

     command : git commit -m "Chnges done Message"

     Creates a checkpoint of your files
     -m adds a message explaining what changed
     This commit exists only on your laptop for now


**STEP 6: Create an EMPTY repo on GitHub**


**STEP 7: Connect local repo to GitHub (one-time)**

     command : git remote add origin git@github.com:YOUR_USERNAME/demo-project.git

     Links your local repo → GitHub repo
     origin = nickname for GitHub
     SSH URL ensures password-less access

     command : git remote -v      (verify process)


**STEP 8: Upload (push) the file**

     command : git branch -M main
               git push -u origin main

     git branch -M main → ensures branch name is main
     git push → uploads commits to GitHub
     -u → remembers this branch for future pushes
