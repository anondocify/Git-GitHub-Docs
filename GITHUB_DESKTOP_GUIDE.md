# GitHub Desktop Guide

This guide explains how to use **GitHub Desktop**, a graphical app that makes using Git and GitHub easy.

## 1. Installation

If you haven't installed it yet:
1.  Open [RELEASES.md](./RELEASES.md).
2.  Run the **GitHubDesktopSetup-x64.exe** installer.
3.  Sign in with your GitHub account when prompted.

## 2. Cloning a Repository (Downloading)

To work on a project from GitHub:
1.  Open GitHub Desktop.
2.  Click **File** > **Clone repository...**
3.  Choose the **GitHub.com** tab.
4.  Select your repository from the list OR click **URL** and paste the link.
5.  Choose a **Local Path** (where to save it on your computer).
6.  Click **Clone**.

## 3. Making & Committing Changes

When you edit files in your project folder, GitHub Desktop detects them automatically.

### Step 1: View Changes
*   On the left sidebar, you will see a list of changed files.
*   Click a file to see the **Diff** (changes) on the right.
    *   **Green**: Added lines.
    *   **Red**: Deleted lines.

### Step 2: Commit Changes
1.  Look at the bottom-left corner.
2.  **Summary**: Type a short title for your change (e.g., "Fix login bug").
3.  **Description**: (Optional) Add more details.
4.  Click the blue **Commit to main** button.

## 4. Syncing (Push & Pull)

### Pushing (Uploading)
After committing, your changes are saved *locally*. To send them to GitHub:
1.  Look at the top toolbar.
2.  Click the **Push origin** button.
3.  Wait for the loading bar to finish.

### Pulling (Downloading Updates)
To get changes made by others:
1.  Click the **Fetch origin** button at the top.
2.  If there are new changes, the button will change to **Pull origin**.
3.  Click **Pull origin** to download them.

## 5. Creating a New Repository

1.  Click **File** > **New repository...**
2.  **Name**: Give your project a name.
3.  **Local Path**: Choose where to save it.
4.  **Git Ignore**: Select "Node", "Python", or "None" depending on your project.
5.  Click **Create repository**.
6.  Click **Publish repository** at the top to send it to GitHub.
