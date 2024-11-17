# ![GIT](../img/icons8-git-48.png)
# Git

Git is a distributed version control system that allows developers to track changes, collaborate on code, and manage project versions effectively. Below are some basic functionalities of Git and their corresponding commands:

---

### **1. Setting Up Git**

- **Configure Git:**
  Set up your user information for all local repositories.
  ```bash
  git config --global user.name "Your Name"
  git config --global user.email "your.email@example.com"
  ```

- **Check Configuration:**
  View the current Git configuration.
  ```bash
  git config --list
  ```

---

### **2. Initializing a Repository**

- **Create a New Repository:**
  Initialize a Git repository in the current directory.
  ```bash
  git init
  ```

- **Clone an Existing Repository:**
  Copy a remote repository to your local machine.
  ```bash
  git clone <repository_url>
  ```

---

### **3. Basic Workflow Commands**

#### **Tracking Changes**
- **Check Repository Status:**
  View the status of files in the working directory.
  ```bash
  git status
  ```

- **Add Files to Staging Area:**
  Stage specific files or all changes.
  ```bash
  git add <file>    # Add specific file
  git add .         # Add all changes
  ```

- **Commit Changes:**
  Save staged changes to the repository with a message.
  ```bash
  git commit -m "Your commit message"
  ```

#### **Viewing History**
- **View Commit Log:**
  Display the commit history.
  ```bash
  git log
  ```

- **View Changes:**
  Show changes made in the working directory.
  ```bash
  git diff          # Changes not staged
  git diff --staged # Changes staged for commit
  ```

---

### **4. Branching and Merging**

#### **Branching**
- **Create a Branch:**
  Create a new branch to work on a feature.
  ```bash
  git branch <branch_name>
  ```

- **Switch Branch:**
  Move to another branch.
  ```bash
  git checkout <branch_name>
  ```

- **Create and Switch Branch:**
  Create a new branch and switch to it.
  ```bash
  git checkout -b <branch_name>
  ```

- **List Branches:**
  View all branches in the repository.
  ```bash
  git branch
  ```

#### **Merging**
- **Merge a Branch:**
  Combine changes from another branch into the current branch.
  ```bash
  git merge <branch_name>
  ```

---

### **5. Working with Remote Repositories**

#### **Connecting to a Remote**
- **Add a Remote:**
  Link your repository to a remote server.
  ```bash
  git remote add origin <repository_url>
  ```

- **View Remotes:**
  List all configured remotes.
  ```bash
  git remote -v
  ```

#### **Pushing and Pulling**
- **Push Changes:**
  Send local changes to a remote repository.
  ```bash
  git push origin <branch_name>
  ```

- **Pull Changes:**
  Fetch and merge changes from a remote repository.
  ```bash
  git pull
  ```

- **Fetch Changes:**
  Fetch changes from a remote repository without merging.
  ```bash
  git fetch
  ```

---

### **6. Undoing Changes**

#### **Undo Local Changes**
- **Unstage a File:**
  Remove a file from the staging area.
  ```bash
  git reset <file>
  ```

- **Discard Changes:**
  Revert changes in the working directory.
  ```bash
  git checkout -- <file>
  ```

#### **Undo Commits**
- **Amend a Commit:**
  Modify the most recent commit (e.g., to change the message).
  ```bash
  git commit --amend
  ```

- **Revert a Commit:**
  Create a new commit that undoes a previous commit.
  ```bash
  git revert <commit_hash>
  ```

- **Reset to a Previous Commit:**
  Reset the repository to a specific commit.
  ```bash
  git reset --soft <commit_hash>  # Keep changes staged
  git reset --mixed <commit_hash> # Keep changes in working directory
  git reset --hard <commit_hash>  # Discard all changes
  ```

---

### **7. Collaboration**

#### **Working with Pull Requests**
- **Create a Pull Request:**
  Push your branch and open a pull request on the remote platform (e.g., GitHub, GitLab).

#### **Stashing Changes**
- **Stash Changes:**
  Save changes temporarily without committing them.
  ```bash
  git stash
  ```

- **Apply Stash:**
  Apply stashed changes back to the working directory.
  ```bash
  git stash apply
  ```

---

### **8. Additional Useful Commands**

- **View File History:**
  View changes made to a specific file.
  ```bash
  git log -- <file>
  ```

- **Delete a Branch:**
  Delete a local or remote branch.
  ```bash
  git branch -d <branch_name>  # Delete local branch
  git push origin --delete <branch_name> # Delete remote branch
  ```

- **View Remote Changes:**
  Check differences between local and remote branches.
  ```bash
  git diff <branch_name> origin/<branch_name>
  ```

---

### **Summary**
Git is essential for source code management, and understanding its basic commands enables efficient workflows. Over time, you can learn more advanced commands and workflows to suit your project needs.