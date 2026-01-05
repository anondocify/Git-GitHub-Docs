*Complete Git & GitHub Guide*

*Introduction*

*What is Git?*
Git is a *distributed version control system* used to track changes in files and source code over time. It helps developers save different versions of a project, compare changes, and safely collaborate with others.

- Track changes in files
- Maintain complete project history
- Revert to previous versions
- Work safely without losing data
- Collaborate with multiple developers

*What is GitHub?*
GitHub is an *online platform* that hosts Git repositories. It allows developers to store projects remotely and collaborate using Git.

- Remote storage for repositories
- Team collaboration
- Pull requests and code reviews
- Issue tracking
- Public and private repositories

*Git* → Version control tool
*GitHub* → Online hosting service for Git repositories

*Why Use Git and GitHub*

- Version control for source code
- Team collaboration
- Backup and recovery
- Project sharing
- Industry-standard development workflow
- Open-source contribution

*Prerequisites*

- Computer (Windows, Linux, or macOS)
- Internet connection
- GitHub account
- Basic command-line knowledge (optional)

*Installing Git*

*Check if Git Is Installed*
git --version

If Git is installed, the version number will appear.

*Install Git on Windows*
1. Download Git from https://git-scm.com
2. Run the installer
3. Use default settings
4. Finish installation

*Install Git on Linux*
sudo apt update
sudo apt install git

*Install Git on macOS*
brew install git

*Initial Git Configuration*

Configure Git once after installation.
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
git config --list

*Creating a Git Repository*

*Initialize a Repository*
git init

This creates a `.git` folder that stores the project history.

*Check Repository Status*
git status

*Git Workflow*

Git uses a three-stage workflow:

1. Working Directory
2. Staging Area
3. Repository

*Add Files to Staging Area*
Add a specific file: `git add filename`
Add all files: `git add .`

*Commit Changes*
git commit -m "Commit message"

*Working with GitHub (Remote Repositories)*

*Create a Repository on GitHub*
1. Log in to GitHub
2. Click New Repository
3. Enter repository name
4. Create the repository

*Connect Local Repository to GitHub*
git remote add origin https://github.com/username/repository-name.git
git remote -v

*Push Code to GitHub*
git push -u origin main

*Pull Code from GitHub*
git pull origin main

*Branching in Git*

*Create a new branch*
git branch new-branch

*Switch to a branch*
git checkout new-branch

*Create and switch*
git checkout -b new-branch

*Merge Branches*
git checkout main
git merge new-branch

*Collaboration Workflow*

1. Clone repository
2. Create a new branch
3. Make changes
4. Commit changes
5. Push branch
6. Create pull request

*Clone a Repository*
git clone https://github.com/username/repository-name.git

*All Common Git Commands*

*Repository Setup*
- `git init`
- `git clone <url>`

*Configuration*
- `git config --global user.name "Name"`
- `git config --global user.email "Email"`
- `git config --list`

*File Tracking*
- `git status`
- `git add <file>`
- `git add .`
- `git rm <file>`

*Commit History*
- `git commit -m "message"`
- `git log`
- `git log --oneline`

*Branching*
- `git branch`
- `git branch <name>`
- `git checkout <branch>`
- `git checkout -b <branch>`
- `git merge <branch>`

*Remote Repositories*
- `git remote`
- `git remote -v`
- `git remote add origin <url>`

*Push & Pull*
- `git push`
- `git push -u origin main`
- `git pull`

*Undo Changes*
- `git diff`
- `git reset`
- `git reset --hard`
- `git checkout -- <file>`

*Using .gitignore*

The `.gitignore` file tells Git which files or folders should not be tracked.

Example:
node_modules/
.env
*.log
dist/

*Best Practices*

- Commit small and meaningful changes
- Write clear commit messages
- Use branches for new features
- Pull changes before pushing
- Never store sensitive data
- Keep repositories clean and organized

*Conclusion*

Git and GitHub are essential tools for modern development. They improve code quality, collaboration, and project management. Consistent practice is the key to mastering Git.