# Complete Git & GitHub Guide

This comprehensive guide covers everything you need to know to get started with Git and GitHub on Windows, Linux, and macOS.

## Table of Contents
1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
    - [Windows](#installing-git-on-windows)
    - [Linux](#installing-git-on-linux)
    - [macOS](#installing-git-on-macos)
4. [First-Time Configuration](#first-time-configuration)
5. [GitHub Setup](#github-setup)
6. [Core Git Workflow](#core-git-workflow)
7. [Using GitHub Desktop](./GITHUB_DESKTOP_GUIDE.md)
8. [Visual Reference](#visual-reference)

---

## Introduction

### What is Git?
Git is a **distributed version control system**. It tracks changes in your code, allowing you to:
- Revert to previous versions.
- Collaborate with others without overwriting their work.
- Maintain a history of your project.

### What is GitHub?
GitHub is a **cloud-based platform** that hosts Git repositories. It adds collaboration features like:
- **Pull Requests**: Review code before merging.
- **Issues**: Track bugs and tasks.
- **Actions**: Automate testing and deployment.

---

## Prerequisites
- A computer (Windows, Linux, or macOS).
- An internet connection.
- A [GitHub account](https://github.com/signup).

---

## Installation

> **Offline Installers**: This repository contains offline installers for **Git (Windows)**, **GitHub Desktop**, and **VS Code**. Please refer to [RELEASES.md](./RELEASES.md) for direct access.

### Installing Git on Windows

**Use Offline Installer (Recommended)**
1.  Open [RELEASES.md](./RELEASES.md) in this repository.
2.  Click on **Git-2.52.0-64-bit.exe** to run the installer.


**Installation Wizard Steps:**
1.  Run the installer.
2.  **Select Components**: Ensure "Git Bash Here" and "Git GUI Here" are checked.
3.  **Default Editor**: Choose Visual Studio Code (recommended) or Nano.
4.  **Path Environment**: Select "Git from the command line and also from 3rd-party software".
5.  **Line Ending**: Keep "Checkout Windows-style, commit Unix-style line endings".
6.  Click "Install".

> **Visual Aid**: Refer to the *Git Installer Mockup* generated in the chat to see what the component selection screen looks like.

### Installing Git on Linux

**Debian/Ubuntu:**
```bash
sudo apt update
sudo apt install git
```

**Fedora:**
```bash
sudo dnf install git
```

> **Note**: An offline installer for **VS Code (.deb)** is available in [RELEASES.md](./RELEASES.md).

**Verify Installation:**
```bash
git --version
```

### Installing Git on macOS

**Option 1: Using Homebrew (Recommended)**
If you don't have Homebrew, install it from [brew.sh](https://brew.sh).
```bash
brew install git
```

**Option 2: Xcode Command Line Tools**
Run this command and follow the prompts:
```bash
xcode-select --install
```

---

## First-Time Configuration

Open your terminal (Git Bash on Windows, Terminal on Mac/Linux) and run these commands. Replace the name and email with your GitHub details.

```bash
# Set your name
git config --global user.name "Your Name"

# Set your email
git config --global user.email "your.email@example.com"

# Verify configuration
git config --list
```

---

## GitHub Setup

### Creating a Repository

1.  Log in to [GitHub.com](https://github.com).
2.  Click the **+** icon in the top-right corner and select **New repository**.
3.  **Repository Name**: Enter a unique name (e.g., `my-first-project`).
4.  **Visibility**: Choose **Public** (visible to everyone) or **Private** (only you and contributors).
5.  **Initialize**: Check "Add a README file" to start with a file.
6.  Click **Create repository**.

> **Visual Aid**: Refer to the *GitHub New Repo Mockup* generated in the chat for a visual guide of this page.

### Connecting Local to Remote

If you have a local folder you want to push to GitHub:

```bash
# Navigate to your project folder
cd path/to/your/project

# Initialize Git
git init

# Add the remote origin (get this URL from your new GitHub repo)
git remote add origin https://github.com/username/repository-name.git

# Rename branch to main
git branch -M main

# Push your files
git push -u origin main
```

---

## Core Git Workflow

The basic cycle of using Git involves three steps: **Add**, **Commit**, **Push**.

### 1. Check Status
See which files have changed.
```bash
git status
```

### 2. Add Changes (Staging)
Prepare files to be saved.
```bash
# Add a specific file
git add filename.txt

# Add all changes
git add .
```

### 3. Commit Changes (Saving)
Save the snapshot of your files with a message.
```bash
git commit -m "Added a new feature"
```

### 4. Push to GitHub
Upload your commits to the cloud.
```bash
git push
```

### 5. Pull Changes
Download changes made by others.
```bash
git pull
```

---

## Using VS Code with Git

Visual Studio Code has built-in Git support that makes this process visual.

1.  **Open Source Control**: Click the icon that looks like a branching path (Ctrl+Shift+G).
2.  **View Changes**: You will see a list of changed files. Clicking one shows a "Diff" (comparison) of what changed.
3.  **Stage**: Click the **+** icon next to a file to stage it (`git add`).
4.  **Commit**: Type a message in the box at the top and press **Commit** (Checkmark icon).
5.  **Sync**: Click the **Sync Changes** button (arrows icon) in the status bar to Pull and Push.

> **Visual Aid**: Refer to the *VS Code Git Mockup* generated in the chat to see the Source Control interface.

---

## Visual Reference

Since I cannot embed live screenshots from the web directly into this file, I have generated high-quality visual aids for you in our chat session. Please refer to them for:

1.  **Git Installation Wizard (Windows)**: Shows the component selection step.
2.  **GitHub New Repository Page**: Shows the form for creating a repo.
3.  **VS Code Git Interface**: Shows how changes and commits look in the editor.

For additional official screenshots, you can visit:
- [Git SCM Book - Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [GitHub Docs - Creating a Repo](https://docs.github.com/en/get-started/quickstart/create-a-repo)
- [VS Code Version Control](https://code.visualstudio.com/docs/sourcecontrol/overview)