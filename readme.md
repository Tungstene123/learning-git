# Git & GitHub Learning

## What is Git
Git is a distributed version control system that tracks changes in your code and lets you manage history.

## What is GitHub
GitHub is a cloud platform for hosting Git repositories and collaborating with others.

***

## Initial Setup (First Time Only)

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --global init.defaultBranch main
```

Check config:
```bash
git config --list
```

***

## Create or Initialize a Repository

### Create a new repo locally
```bash
git init
```

### Clone an existing repo
```bash
git clone https://github.com/username/repo.git
cd repo
```

***

## Basic Workflow

### Check status
```bash
git status
```

### Add files to staging
```bash
git add index.html
git add .              # Add all files
```

### Commit changes
```bash
git commit -m "Add homepage structure"
```

### View history
```bash
git log
git log --oneline --graph
```

***

## Working with GitHub (Remote)

### Add remote repository
```bash
git remote add origin https://github.com/username/repo.git
```

### Verify remote
```bash
git remote -v
```

### Push to GitHub (first time)
```bash
git push -u origin main
```

### Push updates
```bash
git push
```

### Pull changes
```bash
git pull origin main
```

***

## Branching and Merging

### Create a branch
```bash
git branch feature-navbar
```

### Switch branch
```bash
git checkout feature-navbar
# or modern:
git switch feature-navbar
```

### Create and switch in one command
```bash
git checkout -b feature-navbar
# or:
git switch -c feature-navbar
```

### Merge into main
```bash
git checkout main
git merge feature-navbar
```

### Delete branch
```bash
git branch -d feature-navbar
```

***

## Undo and Fix Mistakes

### Unstage a file
```bash
git restore --staged file.txt
```

### Discard local changes
```bash
git restore file.txt
```

### Amend last commit
```bash
git commit --amend -m "Updated message"
```

***

## .gitignore Example

Create a `.gitignore` file to exclude files:

```
node_modules/
.env
*.log
build/
```

***

## Pull Requests (GitHub)

- Push your branch:
```bash
git push -u origin feature-navbar
```

- Open a Pull Request on GitHub
- Review and merge into `main`

***

## Typical Daily Workflow

```bash
git pull
git add .
git commit -m "Describe changes"
git push
```