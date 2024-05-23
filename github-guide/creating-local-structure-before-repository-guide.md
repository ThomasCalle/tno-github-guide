# 📖 Creating Local Structures Before Creating a GitHub Repository Guide

This guide provides a comprehensive, step-by-step solution for creating a local project structure before setting up a repository on GitHub. Starting with a local setup can offer more flexibility and control over your initial project environment. Using the `git init` command, you can convert your local folder into a Git repository and seamlessly link it to GitHub. This approach ensures that your local developments are well-organized before being shared on a remote platform.

## Step-by-Step Process

### Step 1: Create Local Project Folder

1. **Create a Local Folder**:
   - On your local machine, create a new folder for your project using your file manager or command line. This folder will contain all your project files and directories.

   Example:
   ```sh
   mkdir my-project
   cd my-project
   # At this point, you would typically add your project files to the folder
   ```

### Step 2: Initialize Git

1. **Navigate to Your Project Folder**:
   - Use the command:
     ```sh
     cd my-project
     ```

2. **Initialize the Git Repository**:
   - Run the command:
     ```sh
     git init
     ```
   - This command initializes a new Git repository in the current directory, allowing Git to start tracking changes.

### Step 3: Connect to GitHub Repository

1. **Create a New Repository on GitHub**:
   - Go to [GitHub](https://github.com/) and sign in.
   - Click the "+" icon in the upper right corner and select "New repository."
   - Name your repository (e.g., `my-project`), choose "Public" or "Private," and click "Create repository."
   - **Do not initialize with a README** to avoid conflicts.

2. **Link Local Repository to GitHub**:
   - Connect your local repository to the GitHub repository using:
     ```sh
     git remote add origin https://github.com/YOUR-USERNAME/REPO-NAME.git
     ```
   - Replace `YOUR-USERNAME` and `REPO-NAME` with your GitHub username and the repository name.

### Step 4: Add and Commit Files

1. **Stage Your Files**:
   - Add all your project files to the staging area using:
     ```sh
     git add .
     ```
   - This command stages all changes in your project directory for the next commit.

2. **Commit Your Changes**:
   - Commit the staged files with a descriptive message:
     ```sh
     git commit -m "Initial commit"
     ```

### Step 5: Push to GitHub

1. **Push Your Changes**:
   - Push your local commits to the GitHub repository:
     ```sh
     git push -u origin main
     ```
   - The `-u` flag sets the upstream branch, making future pushes simpler. Ensure you're pushing to the correct branch name (usually `main`).

## Common Issues and Troubleshooting

### Issue: Git is not recognized as an internal or external command
- **Solution**: Ensure Git is installed correctly and added to your system's PATH.

### Issue: Permission denied (publickey)
- **Solution**: Ensure your SSH key is added to your GitHub account. Generate an SSH key using `ssh-keygen` and add the public key to GitHub.

### Issue: Merge conflicts
- **Solution**: Review conflicting files and merge changes manually. Use `git status` to identify conflicts.

## Key Commands

- `git init`: Initialize a new Git repository.
- `git remote add origin <URL>`: Link your local repository to a remote GitHub repository.
- `git add .`: Stage all changes in the current directory.
- `git commit -m "message"`: Commit the staged changes with a message.
- `git push -u origin main`: Push commits to the remote repository and set the upstream branch.

## Glossary of Terms

- **Repository**: A storage space for your project's files and history.
- **Clone**: Creating a local copy of a repository from a remote server.
- **Commit**: Recording changes to the repository.
- **Branch**: A separate line of development in a project.
- **Merge**: Combining changes from different branches into a single branch.
- **Pull**: Fetching and integrating changes from a remote repository to your local repository.
- **Push**: Sending your local repository changes to the remote repository.

---

This guide ensures efficient personal project management in 2024 using GitHub and VSCode on both Windows and macOS.

A special thank you to all the mentors and volunteers who made this TNO Community possible and accessible to all participants.

© 2024 Thomas Calle. Confidential and Proprietary. All Rights Reserved.