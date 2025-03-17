Here’s a simplified guide on common Git operations, including push and pull, along with some additional important operations:

⸻

Git Basic Operations:

1. Clone a Repository

To make a local copy of a remote repository:

git clone <repository_url>

Example:

git clone https://github.com/username/repository.git

2. Check the Current Status

To see the status of your repository (untracked, modified, staged files):

git status

3. Add Changes to Staging

To add modified files to the staging area before committing:
	•	Add a single file:

git add <file_name>


	•	Add all modified files:

git add .



4. Commit Changes

After staging the files, you commit the changes:

git commit -m "Your commit message here"

5. Push Changes to Remote Repository

To upload your local commits to a remote repository (like GitHub, GitLab):

git push origin <branch_name>

Example for pushing to the main branch:

git push origin main

6. Pull Changes from Remote Repository

To fetch and merge changes from the remote repository to your local branch:

git pull origin <branch_name>

Example for pulling from the main branch:

git pull origin main

7. Create a New Branch

To create a new branch:

git checkout -b <new_branch_name>

Example:

git checkout -b feature/new-feature

8. Switch Between Branches

To switch to an existing branch:

git checkout <branch_name>

Example:

git checkout main

9. View Commit History

To view the commit history of your repository:

git log

You can use --oneline for a simplified view:

git log --oneline

10. Merge Branches

To merge changes from one branch into another (e.g., merging feature into main):
	1.	First, switch to the branch you want to merge into (e.g., main):

git checkout main


	2.	Then, merge the changes from the feature branch:

git merge feature



11. Remove a File from Git

To remove a file from Git’s tracking, but not from the local file system:

git rm <file_name>

After running git rm, remember to commit the changes:

git commit -m "Removed file"

12. Stash Changes

To temporarily save changes that are not yet committed (for when you want to switch branches):

git stash

To apply stashed changes later:

git stash apply

13. View Remote Repository Information

To view information about your remotes:

git remote -v



⸻

Workflow Example:
	1.	Clone the repo (if you haven’t already):

git clone https://github.com/username/repository.git


	2.	Create a new branch for your work:

git checkout -b feature/awesome-feature


	3.	Make your changes to files (edit, add new ones, etc.).
	4.	Stage the changes:

git add .


	5.	Commit the changes:

git commit -m "Added awesome feature"


	6.	Push the changes to your remote repository:

git push origin feature/awesome-feature


	7.	Create a Pull Request (PR) (on GitHub or GitLab):
	•	Go to the repository’s page on GitHub.
	•	Click on “Pull Requests” > “New Pull Request”.
	•	Choose your branch and submit the PR for review.
	8.	Pull changes from the remote repo (if there are updates):

git pull origin main



⸻

Summary of Common Git Commands:
	•	git clone <repo_url> — Clone a remote repository.
	•	git status — Check the status of your files.
	•	git add <file_name> — Stage files for commit.
	•	git commit -m "message" — Commit staged changes.
	•	git push origin <branch_name> — Push commits to remote.
	•	git pull origin <branch_name> — Pull updates from remote.
	•	git checkout <branch_name> — Switch branches.
	•	git merge <branch_name> — Merge a branch into the current branch.
	•	git log — View commit history.

⸻

Let me know if you need further clarification or examples for any of these!