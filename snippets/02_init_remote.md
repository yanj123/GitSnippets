# Git Snippets: Initialize and Connect to Remote

When you create a new project on your computer, you can connect it to a GitHub repository so changes can be pushed online.

---

## 1. Initialize a Local Repository

If your project folder is not yet a Git repo, run:

  ```bash
  git init
  ```

This creates a hidden `.git` folder and starts tracking your project with Git.

---

## 2. Add a Remote Repository

Tell Git where your GitHub repository is located:

  ```bash
  git remote add origin <repository-url>
  ```

Example:

  ```bash
  git remote add origin https://github.com/username/my-project.git
  ```

- `origin` is the default name for your remote repository.
- `<repository-url>` is the HTTPS or SSH link you get from GitHub.

---

## 3. Verify Remote Connection

Check if the remote was added successfully:

  ```bash
  git remote -v
  ```

Example output:

  ```bash
  origin  https://github.com/username/my-project.git (fetch)
  origin  https://github.com/username/my-project.git (push)
  ```

---

## 4. Push Code to GitHub

If this is your first push, use:

  ```bash
  git branch -M main
  git push -u origin main
  ```

- `git branch -M main` → renames your branch to main (standard default).
- `-u` sets `origin main` as the default, so later you can just use git push without extra options.

---

## 🚀 Quick Recap

- `git init` → Start Git in your project.
- `git remote add origin <url>` → Link local repo to GitHub.
- `git push -u origin main` → Upload your project to GitHub.

---

> Next step → Learn the [add, commit and push code commands](https://github.com/Akshat7garg/GitSnippets/blob/main/snippets/03_stage_commit_push.md).
