# Complete Git & GitHub Guide

This document explains Git and GitHub from scratch, covering installation, configuration, daily workflow, version control concepts, branching, collaboration, and best practices.  
No prior knowledge is required.

---

## 1. Introduction

### What is Git?

Git is a distributed version control system used to track changes in files and source code over time.  
It allows developers to manage versions, revert changes, and collaborate efficiently.

Git helps you:
- Track file changes
- Maintain code history
- Work safely without data loss
- Collaborate with multiple people

---

### What is GitHub?

GitHub is a cloud-based platform that hosts Git repositories.  
It provides tools for collaboration, code sharing, and project management.

GitHub allows:
- Remote storage of repositories
- Collaboration between developers
- Issue tracking and pull requests
- Public and private projects

Git is the tool.  
GitHub is the online service.

---

## 2. Why Use Git and GitHub

- Source code version control
- Team collaboration
- Backup and recovery
- Project sharing
- Industry-standard workflow
- Open-source contribution

---

## 3. Prerequisites

- A computer (Windows, Linux, or macOS)
- Internet connection
- GitHub account
- Basic command-line knowledge (optional)

---

## 4. Installing Git

### Check if Git Is Installed

```bash
git --version

If Git is installed, the version number will be displayed.


---

Install Git on Windows

1. Download Git from https://git-scm.com


2. Run the installer


3. Use default settings


4. Complete the installation




---

Install Git on Linux

sudo apt update
sudo apt install git


---

Install Git on macOS

brew install git


---

5. Initial Git Configuration

Configure Git once after installation.

Set username:

git config --global user.name "Your Name"

Set email:

git config --global user.email "youremail@example.com"

Verify configuration:

git config --list


---

6. Creating a Git Repository

Initialize a Repository

git init

This creates a .git directory that stores version history.


---

Check Repository Status

git status


---

7. Git Workflow

Git follows a three-stage workflow:

1. Working Directory


2. Staging Area


3. Repository




---

Add Files to Staging Area

Add a single file:

git add filename

Add all files:

git add .


---

Commit Changes

git commit -m "Commit message"


---

8. Working with GitHub (Remote Repositories)

Create a Repository on GitHub

1. Log in to GitHub


2. Click "New Repository"


3. Enter repository name


4. Create the repository




---

Connect Local Repository to GitHub

git remote add origin https://github.com/username/repository-name.git

Check remote:

git remote -v


---

9. Pushing Code to GitHub

git push -u origin main

The -u flag sets the upstream branch.


---

10. Pulling Code from GitHub

git pull origin main


---

11. Branching in Git

Create a Branch

git branch new-branch

Switch branch:

git checkout new-branch

Create and switch:

git checkout -b new-branch


---

Merge Branches

git checkout main
git merge new-branch


---

12. Collaboration Workflow

1. Clone repository


2. Create a branch


3. Make changes


4. Commit changes


5. Push branch


6. Create a pull request




---

Clone a Repository

git clone https://github.com/username/repository-name.git


---

13. Common Git Commands

Command	Description

git status	Show file status
git log	Show commit history
git diff	Show changes
git branch	List branches
git checkout	Switch branches
git reset	Undo changes



---

14. Using .gitignore

The .gitignore file tells Git which files to ignore.

Example:

node_modules/
.env
*.log
dist/


---

15. Best Practices

Commit small logical changes

Write meaningful commit messages

Use branches for features

Pull changes before pushing

Do not store sensitive data

Keep repositories organized



---

16. Conclusion

Git and GitHub are essential tools for modern software development.
Understanding version control improves code quality, collaboration, and project management.

Regular practice is the key to mastering Git.


---
