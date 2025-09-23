# Git Snippets: Create Repo, Clone, and Status

These are the first Git commands you’ll need when starting with a project.  

---

## 1. Create a New Repository (Local)

If you’re starting a brand-new project:  

  ```bash
  git init
  ```

- Creates a hidden `.git` folder inside your project.
-This is what makes Git start tracking your files.

✅ Run this **only once per project**.

---

## 2. Clone an Existing Repository (From GitHub)

If you want to copy a project from GitHub to your computer:

  ```bash
  git clone <repository-url>
  ```

Example:

  ```bash
  git clone https://github.com/octocat/Hello-World.git
  ```

- Creates a new folder named after the repo.
- Contains the project files + Git history.

✅ Use this when you **join a project** or want to **practice with a sample repo**.

---

## 3. Check Repository Status

To see what’s happening inside your repo:

  ```bash
  git status
  ```

It shows:

- ✅ Which branch you’re on
- ✅ Which files have changes
- ✅ Which files are staged (ready to commit)
- ✅ Which files are not tracked yet

Example output:

  ```bash
  On branch main
  Your branch is up to date with 'origin/main'.
  
  Changes not staged for commit:
    modified: index.html
  ```

---

## 🚀 Quick Recap

- `git init` → Start tracking a new project.
- `git clone` → Copy a repo from GitHub.
- `git status` → See what’s going on in your repo.

---

> Next step → Learn the [init + remote connection commands](https://github.com/Akshat7garg/GitSnippets/blob/main/snippets/02_init_remote.md).
