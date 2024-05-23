You used `git init` because you started by creating a local file structure on your machine before creating a repository on GitHub. The `git init` command initializes a new Git repository in your local directory, making it a Git project. 

Here's the step-by-step process you likely followed:

1. **Create Local Project Folder**:
   - You created a folder on your local machine and added your project files.

2. **Initialize Git**:
   - You ran `git init` to create a new Git repository in that folder.

3. **Connect to GitHub Repository**:
   - You created a new repository on GitHub.
   - You connected your local repository to the GitHub repository using:
     ```sh
     git remote add origin https://github.com/YOUR-USERNAME/REPO-NAME.git
     ```

4. **Add and Commit Files**:
   - You staged your files:
     ```sh
     git add .
     ```
   - You committed your changes:
     ```sh
     git commit -m "Initial commit"
     ```

5. **Push to GitHub**:
   - You pushed your changes to the GitHub repository:
     ```sh
     git push -u origin main
     ```

In contrast, the guide provided in the README.md assumes you create the repository on GitHub first and then clone it to your local machine, which initializes the local repository automatically. Both methods are valid and depend on whether you start with a local project or a GitHub repository.