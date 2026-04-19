# Learning git and version control on github

📌 What is Git?  
Git is a distributed version control system that lets you save snapshots of your code.

📌 What is GitHub?  
GitHub is a cloud-based platform to store Git repositories and collaborate with developers.

🛠️ Basic Git Commands (with Examples)

1️⃣ git init  
Initialize a Git repo in your project folder.
git init

2️⃣ git status  
Check what changes are untracked or modified.
git status

3️⃣ git add  
Add files to staging area (preparing them for commit).
git add index.html
git add.     # Adds all files

4️⃣ git commit  
Save the snapshot with a message.
git commit -m "Added homepage structure"

5️⃣ git log  
See the history of commits.
git log

🌐 Using GitHub

6️⃣ git remote add origin  
Connect your local repo to GitHub.
git remote add origin https://github.com/yourusername/repo.git

7️⃣ git push  
Push your local commits to GitHub.
git push -u origin main

8️⃣ git pull  
Pull latest changes from GitHub.
git pull origin main

🪫 Collaboration Basics

🔀 Branching & Merging
git branch feature-navbar
git checkout feature-navbar
# Make changes, then:
git add.
git commit -m "Added navbar"
git checkout main
git merge feature-navbar

🔵 Pull Requests  
Used on GitHub to review & merge code between branches.