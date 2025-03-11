# Basic Bash Commands 🚀

## File and Directory Management 📂
- `ls` : Lists files and directories. Use `ls -a` to show hidden files. 👀
- `pwd` : Prints the current working directory. 📌
- `cd <directory>` : Changes to the specified directory. 🔄
  - Example: `cd project`
  - Use `cd ..` to go back to the previous directory. ⬅️
- **Absolute Path**: A full path starting from the root (`/`). 🛤️
  - Example: `/home/user/document/project/index.html`
- **Relative Path**: A path relative to the current working directory. 🔗
  - Example: `../data/file.txt`
- `mkdir <directory>` : Creates a new directory. 📁
- `rm <file>` : Removes a file. ❌
- `rmdir <directory>` : Removes an empty directory. 🚮
- `mv <source> <destination>` : Moves or renames files/directories. 🔄
- `cp <source> <destination>` : Copies files or directories. 📋

## Git Commands 🖥️
### Creating a Repository 🏗️
- `git init` : Initializes a new Git repository. 🎯
- `ls -al` : Lists all files, including hidden ones, after `git init`. 🔍
- `git clone <repository_url>` : Clones an existing repository. 🔄

### Tracking Changes 📝
- `git status` : Shows the status of changes in the repository. 🔍
- `git add <file>` : Stages a specific file for commit. 📌
- `git add .` : Stages all changes in the current directory. 📂
- `git commit -m "message"` : Commits staged changes with a message. 📝
- `git reset <file>` : Unstages a file before committing. ⏪
- `git reset --hard` : Resets all changes to the last committed state. ❌
- If prompted for user identity:
  - `git config --global user.name "Your Name"` 👤
  - `git config --global user.email "youremail@example.com"` 📧
- `git log` : Shows commit history. 📜
- `git diff` : Displays changes. Press `q` to exit. 🔄

### Synchronizing with Remote Repositories 🌍
- `git push` : Pushes local changes to the remote repository. 🚀
  - `git remote add origin <repository_url>` : Adds a remote repository. 🔗
  - `git remote -v` : Verifies remote repository. ✅
  - `git push origin master` : Pushes changes to the `master` branch. 📤
- `git pull origin master` : Pulls updates from the remote repository. 🔄
- `git fetch` : Downloads changes without merging them. 🛠️
  - `git fetch`
  - `git checkout <branch>` : Switches to the specified branch. 🔀
  - `git branch` : Lists all branches. 🌿
- Deleting a branch:
  - `git checkout master` 🏠
  - `git branch` 📜
  - `git branch -D <branch_name>` ❌

### Working with Branches 🌿
- `git branch` : Lists all branches. 📜
- `git checkout <branch>` : Switches to the specified branch. 🔀
- `git merge <branch>` : Merges a branch into the current branch. 🔄
- `git tag` : Creates a tag for a specific commit. 🏷️

### Common Workflow 🔄
```bash
# Stage all changes, commit, and push to the main branch
git add .
git commit -m "Your commit message"
git push origin main