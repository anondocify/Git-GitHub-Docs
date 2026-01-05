# Complete Git & GitHub Guide

This guide explains **Git and GitHub from scratch**, covering installation, configuration, version control concepts, daily workflow, branching, collaboration, and best practices.  
No prior knowledge is required.

---

## 1. Introduction

### What is Git?

Git is a **distributed version control system** used to track changes in files and source code over time.  
It helps developers save different versions of a project, compare changes, and safely collaborate with others.

Git helps you to:
- Track changes in files  
- Maintain complete project history  
- Revert to previous versions  
- Work safely without losing data  
- Collaborate with multiple developers  

---

### What is GitHub?

GitHub is an **online platform** that hosts Git repositories.  
It allows developers to store projects remotely and collaborate using Git.

GitHub provides:
- Remote storage for repositories  
- Team collaboration  
- Pull requests and code reviews  
- Issue tracking  
- Public and private repositories  

**Git** → Version control tool  
**GitHub** → Online hosting service for Git repositories  

---

## 2. Why Use Git and GitHub

- Version control for source code  
- Team collaboration  
- Backup and recovery  
- Project sharing  
- Industry-standard development workflow  
- Open-source contribution  

---

## 3. Prerequisites

- Computer (Windows, Linux, or macOS)  
- Internet connection  
- GitHub account  
- Basic command-line knowledge (optional)  

---

## 4. Installing Git

Check if Git Is Installed

git --version

If Git is installed, the version number will appear.


---

Install Git on Windows

1. Download Git from https://git-scm.com


2. Run the installer


3. Use default settings


4. Finish installation




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

git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
git config --list


---

6. Creating a Git Repository

Initialize a Repository

git init

This creates a .git folder that stores the project history.


---

Check Repository Status

git status


---

7. Git Workflow

Git uses a three-stage workflow:

1. Working Directory


2. Staging Area


3. Repository




---

Add Files to Staging Area

Add a specific file:

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


2. Click New Repository


3. Enter repository name


4. Create the repository




---

Connect Local Repository to GitHub

git remote add origin https://github.com/username/repository-name.git
git remote -v


---

9. Push Code to GitHub

git push -u origin main


---

10. Pull Code from GitHub

git pull origin main


---

11. Branching in Git

Create a new branch:

git branch new-branch

Switch to a branch:

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


2. Create a new branch


3. Make changes


4. Commit changes


5. Push branch


6. Create pull request




---

Clone a Repository

git clone https://github.com/username/repository-name.git


---

13. All Common Git Commands (Separated)

Repository Setup

git init
git clone <url>

Configuration

git config --global user.name "Name"
git config --global user.email "Email"
git config --list

File Tracking

git status
git add <file>
git add .
git rm <file>

Commit History

git commit -m "message"
git log
git log --oneline

Branching

git branch
git branch <name>
git checkout <branch>
git checkout -b <branch>
git merge <branch>

Remote Repositories

git remote
git remote -v
git remote add origin <url>

Push & Pull

git push
git push -u origin main
git pull

Undo Changes

git diff
git reset
git reset --hard
git checkout -- <file>


---

14. Using .gitignore

The .gitignore file tells Git which files or folders should not be tracked.

Example:

node_modules/
.env
*.log
dist/


---

15. Best Practices

Commit small and meaningful changes

Write clear commit messages

Use branches for new features

Pull changes before pushing

Never store sensitive data

Keep repositories clean and organized



---

16. Conclusion

Git and GitHub are essential tools for modern development.
They improve code quality, collaboration, and project management.

Consistent practice is the key to mastering Git.


---