# Pre-Setup Repo

1. Create a 'Demo1' repo in your GitHub repo.
1. Open a PowerShell windows and clone the repo to your local machine. (git clone Repo).
1. Switch to the repo folder (cd Demo1)
1. Open the repo in VS Code. (code .)
1. Create & open three new files 'NoConflict1.txt', 'Conflict1.txt', 'Conflict2.txt'
1. Add a single line to each file 'Code from main 1'.
1. Save and commit the file and push the change to the remote repository.
1. Create a new branch 'feature1' and checkout the branch. (git checkout -b feature1)
1. Edit the first line in the 'Conflict1.txt' file to 'Code from feature 1'
1. Edit the first line in the 'Conflict2.txt' file to 'Code from feature 1'
1. Save and commit the files to the new branch and push to the remote repository.
1. Switch back the main branch. (git switch main)
1. Edit the first line in the 'Conflcit1.txt' and 'Conflict2.txt' files to 'Code from main 2'
1. Save and commit the files to the main branch and push to the new repo.

# Demo Setup

1. If needed clone the repo 'Demo 1' from GitHub. The repository contains three filees: NoConflict.txt, Conflict1.txt, and Conflict2.txt with conflicting changes in the 'main' and ‘feature1’ branches.
1. Open VS code to the cloned repo and switch to the 'main' branch. (code ., git switch main)

# Merge

1. Merge the 'feature1' branch to the 'main' branch. (git merge feature1) (Note: To see what conflicts are there w/o commiting use the --no-commit option).
1. Under 'Merge files' Conflict1.txt and Conflict2 are listed. Open the files and resolve the conflicts. Notice that the code from main is listed as 'HEAD' and 'Current' change, code from feature1 is 'Incoming'. Resolve the conflict by keeping the code in main and then save the files.
1. Stage Conflict2.txt and Conflict2.txt (git add .)
1. Complete the merge (git commit).
1. To abort the merge use (git merge --abort)
