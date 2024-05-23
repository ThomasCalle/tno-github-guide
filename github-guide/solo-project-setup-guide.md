# Solo Project Setup Guide

This guide provides instructions for creating a repository on GitHub, cloning it to your local machine using Visual Studio Code (VSCode), and managing push and pull operations. The instructions are applicable for both Windows and macOS.

## For New Users

### Step 1: Create a Repository on GitHub

1. **Sign in to GitHub:**
   - Go to [GitHub](https://github.com/) and sign in.

2. **Create a New Repository:**
   - Click the "+" icon in the upper right corner, select "New repository."
   - Name your repository (e.g., `personal-project`).
   - Choose "Public" or "Private."
   - Check "Initialize this repository with a README."
   - Click "Create repository."

### Step 2: Clone the Repository to Your Local Machine Using VSCode

#### Windows and macOS

1. **Install Git:**
   - Download and install Git from [git-scm.com](https://git-scm.com/) (Windows) or use Homebrew (`brew install git`) on macOS.

2. **Open VSCode and Clone Repository:**
   - Open VSCode.
   - Open the terminal (`Ctrl + ` or `View > Terminal`).
   - Run:
     ```sh
     git clone https://github.com/YOUR-USERNAME/personal-project.git
     ```
   - Replace `YOUR-USERNAME` and `personal-project` with your GitHub username and repo name.

3. **Open Cloned Repository:**
   - In VSCode, go to `File > Open Folder` and select the cloned folder.

### Step 3: Push and Pull to the Repository

1. **Configure Git:**
   - In the terminal, run:
     ```sh
     git config --global user.name "Your Name"
     git config --global user.email "your-email@example.com"
     ```
   - This configuration is important because it helps Git track changes and identify the contributors.

2. **Branching (Optional):**
   - Branching allows you to work on different features or fixes without affecting the main codebase. This is especially useful for collaborative work. If you are working alone, you may not need separate branches and can work directly on the main branch. However, using branches can help keep your work organized.
   - Create a new branch for your feature:
     ```sh
     git checkout -b feature-branch
     ```
   - If you are working alone and choose to use branches, remember to merge them back into the main branch once your feature or fix is complete.

3. **Make Changes, Commit, and Push:**
   - Stage changes:
     ```sh
     git add .
     ```
   - Commit changes:
     ```sh
     git commit -m "Your commit message"
     ```
   - Push changes:
     ```sh
     git push origin feature-branch
     ```

4. **Pull Latest Changes:**
   - To pull changes from the remote repository:
     ```sh
     git pull origin main
     ```

5. **Merging Branches:**
   - Switch to the main branch and merge changes from your feature branch:
     ```sh
     git checkout main
     git pull origin main
     git merge feature-branch
     git push origin main
     ```
   - If you are working alone, you might not need to create and merge branches frequently. Working directly on the main branch is usually sufficient.


# For Experienced Users

### Step 1: Create a Repository on GitHub

1. **Sign in to GitHub:**
   - Go to [GitHub](https://github.com/) and sign in.

2. **Create a New Repository:**
   - Click the "+" icon in the upper right corner, select "New repository."
   - Name your repository.
   - Choose "Public" or "Private."
   - Optionally, initialize with a README.
   - Click "Create repository."

### Step 2: Clone the Repository to Your Local Machine

1. **Open VSCode and Clone Repository:**
   - Open VSCode.
   - Open the terminal.
   - Run:
     ```sh
     git clone https://github.com/YOUR-USERNAME/REPO-NAME.git
     ```
   - Replace `YOUR-USERNAME` and `REPO-NAME` with your GitHub username and repo name.

2. **Open Cloned Repository:**
   - In VSCode, go to `File > Open Folder` and select the cloned folder.

### Step 3: Push and Pull to the Repository

1. **Configure Git (if not already configured)**:
   - This step can be skipped if Git is already configured on your machine.

2. **Branching (Optional):**
   - Branching allows you to work on different features or fixes without affecting the main codebase. Create a new branch for your feature:
     ```sh
     git checkout -b feature-branch
     ```
   - For solo projects, branching is not always necessary. You can work directly on the main branch. However, branches can help keep different features or fixes organized.

3. **Make Changes, Commit, and Push:**
   - Stage changes:
     ```sh
     git add .
     ```
   - Commit changes:
     ```sh
     git commit -m "Your commit message"
     ```
   - Push changes:
     ```sh
     git push origin feature-branch
     ```
   - If working directly on the main branch, replace `feature-branch` with `main` in the above command.

4. **Pull Latest Changes:**
   - To pull changes from the remote repository:
     ```sh
     git pull origin main
     ```

5. **Merging Branches:**
   - Switch to the main branch and merge changes from your feature branch:
     ```sh
     git checkout main
     git pull origin main
     git merge feature-branch
     git push origin main
     ```
   - If working alone, you may often push changes directly to the main branch without needing to merge other branches.

## Summary of Key Commands

- `git clone https://github.com/YOUR-USERNAME/personal-project.git`
- `git checkout -b feature-branch`
- `git add .`
- `git commit -m "Your commit message"`
- `git push origin feature-branch`
- `git pull origin main`
- `git merge feature-branch`

## Common Issues and Troubleshooting

### Issue: Git is not recognized as an internal or external command
- **Solution**: Ensure Git is installed correctly and added to your system's PATH.

### Issue: Permission denied (publickey)
- **Solution**: Ensure your SSH key is added to your GitHub account. You can generate an SSH key using the command `ssh-keygen` and add the public key to GitHub.

### Issue: Merge conflicts
- **Solution**: Carefully review the conflicting files and decide how to merge changes manually. Use `git status` to see which files have conflicts and resolve them.

## Glossary of Terms

- **Repository**: A storage space where your project's files and their histories are stored.
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