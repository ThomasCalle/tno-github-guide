# Solo Project Setup Guide

This guide provides instructions for creating a repository on GitHub, cloning it to your local machine using Visual Studio Code (VSCode), and managing push and pull operations. The instructions are applicable for both Windows and macOS.

## Step 1: Create a Repository on GitHub

1. **Sign in to GitHub:**
   - Go to [GitHub](https://github.com/) and sign in.

2. **Create a New Repository:**
   - Click the "+" icon in the upper right corner, select "New repository."
   - Name your repository (e.g., `personal-project`).
   - Choose "Public" or "Private."
   - Check "Initialize this repository with a README."
   - Click "Create repository."

## Step 2: Clone the Repository to Your Local Machine Using VSCode

### Windows and macOS

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

## Step 3: Push and Pull to the Repository

1. **Configure Git:**
   - In the terminal, run:
     ```sh
     git config --global user.name "Your Name"
     git config --global user.email "your-email@example.com"
     ```

2. **Branching (Optional):**
   - Create a branch:
     ```sh
     git checkout -b feature-branch
     ```

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
   - To pull changes:
     ```sh
     git pull origin main
     ```

5. **Merging Branches:**
   - Switch to the main branch and merge:
     ```sh
     git checkout main
     git pull origin main
     git merge feature-branch
     git push origin main
     ```

## Summary of Key Commands

- `git clone https://github.com/YOUR-USERNAME/personal-project.git`
- `git checkout -b feature-branch`
- `git add .`
- `git commit -m "Your commit message"`
- `git push origin feature-branch`
- `git pull origin main`
- `git merge feature-branch`

---

This guide ensures efficient personal project management in 2024 using GitHub and VSCode on both Windows and macOS.

A special thank you to all the mentors and volunteers who made this TNO Community possible and accessible to all participants.

© 2024 Thomas Calle. Confidential and Proprietary. All Rights Reserved.