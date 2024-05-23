# 📖 Group Project Setup Guide

This guide provides instructions for creating a group repository on GitHub, cloning it to your local machine using Visual Studio Code (VSCode), and managing push and pull operations with your group members. The instructions are applicable for both Windows and macOS.

## For New Users

### Step 1: Create a Group Repository on GitHub

1. **Sign in to GitHub:**
   - Go to [GitHub](https://github.com/) and sign in.

2. **Create a New Repository:**
   - Click the "+" icon in the upper right corner, select "New repository."
   - Name your repository (e.g., `group-project`).
   - Choose "Public" or "Private."
   - Check "Initialize this repository with a README."
   - Click "Create repository."

3. **Add Collaborators:**
   - Go to the repository page, click "Settings."
   - In the left sidebar, click "Manage access."
   - Click "Invite a collaborator" and enter the usernames or emails of your group members.

### Step 2: Clone the Repository to Your Local Machine Using VSCode

#### Windows and macOS

1. **Install Git:**
   - Download and install Git from [git-scm.com](https://git-scm.com/) (Windows) or use Homebrew (`brew install git`) on macOS.

2. **Open VSCode and Clone Repository:**
   - Open VSCode.
   - Open the terminal (`Ctrl + ` or `View > Terminal`).
   - Run:
     ```sh
     git clone https://github.com/YOUR-USERNAME/group-project.git
     ```
   - Replace `YOUR-USERNAME` and `group-project` with your GitHub username and repo name.

3. **Open Cloned Repository:**
   - In VSCode, go to `File > Open Folder` and select the cloned folder.

### Step 3: Push and Pull to the Repository with Group Members

1. **Configure Git:**
   - In the terminal, run:
     ```sh
     git config --global user.name "Your Name"
     git config --global user.email "your-email@example.com"
     ```
   - This configuration is important because it helps Git track changes and identify the contributors.

2. **Branching (Recommended for Collaboration):**
   - Branching allows each group member to work on different features or fixes without affecting the main codebase. This is especially useful for collaborative work. Always create a new branch for your feature or fix:
     ```sh
     git checkout -b feature-branch
     ```
   - Remember to merge your branch back into the main branch once your feature or fix is complete. This ensures all changes are integrated and conflicts are minimized.

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

### Step 4: Using GitHub Project Boards for Workflow Management

1. **Create a Project Board:**
   - Navigate to your repository on GitHub.
   - Click on the "Projects" tab.
   - Click "Create a project" and name your project (e.g., "Group Project Workflow").
   - Choose a template (e.g., "Basic Kanban").

2. **Add Columns and Cards:**
   - Create columns such as "To Do," "In Progress," and "Done."
   - Add cards (tasks) to these columns by clicking "Add a card" and entering the task details.

3. **Assign Tasks:**
   - Assign tasks to team members by clicking on a card, then clicking "Assignees" and selecting the team member.

4. **Track Progress:**
   - Move cards across columns as tasks progress, providing a clear visual overview of the project status.

## For Experienced Users

### Step 1: Create a Repository on GitHub

1. **Sign in to GitHub:**
   - Go to [GitHub](https://github.com/) and sign in.

2. **Create a New Repository:**
   - Click the "+" icon in the upper right corner, select "New repository."
   - Name your repository.
   - Choose "Public" or "Private."
   - Optionally, initialize with a README.
   - Click "Create repository."

3. **Add Collaborators:**
   - Go to the repository page, click "Settings."
   - In the left sidebar, click "Manage access."
   - Click "Invite a collaborator" and enter the usernames or emails of your group members.

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

2. **Branching (Recommended for Collaboration):**
   - Branching allows each group member to work on different features or fixes without affecting the main codebase. Create a new branch for your feature:
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

### Step 4: Using GitHub Project Boards for Workflow Management

1. **Create a Project Board:**
   - Navigate to your repository on GitHub.
   - Click on the "Projects" tab.
   - Click "Create a project" and name your project (e.g., "Group Project Workflow").
   - Choose a template (e.g., "Basic Kanban").

2. **Add Columns and Cards:**
   - Create columns such as "To Do," "In Progress," and "Done."
   - Add cards (tasks) to these columns by clicking "Add a card" and entering the task details.

3. **Assign Tasks:**
   - Assign tasks to team members by clicking on a card, then clicking "Assignees" and selecting the team member.

4. **Track Progress:**
   - Move cards across columns as tasks progress, providing a clear visual overview of the project status.

## Summary of Key Commands

- `git clone https://github.com/YOUR-USERNAME/group-project.git`
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

This guide ensures efficient group project collaboration in 2024 using GitHub and VSCode on both Windows and macOS.

A special thank you to all the mentors and volunteers who made this TNO Community possible and accessible to all participants.

© 2024 Thomas Calle. Confidential and Proprietary. All Rights Reserved.