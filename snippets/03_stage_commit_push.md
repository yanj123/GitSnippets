# Git Snippets: Add, Commit, and Push

These are the most important Git commands to save and upload your work.

---

## 1. Stage Changes (git add)

Tell Git which files you want to include in your next commit.

### Add a single file

  ```bash
  git add filename.txt
  ```

### Add all files in the folder

  ```bash
  git add .
  ```

✅ After this, the files are in the **staging area** (ready to be committed).

---

## 2. Commit Changes (git commit)

Save a snapshot of your staged files in the local repository.

  ```bash
  git commit -m "Your descriptive commit message"
  ```

Example:

  ```bash
  git commit -m "Added homepage layout"
  ```

✅ A commit is like a checkpoint you can return to later.

---

## 3. Push Changes to GitHub (git push)

Upload your commits from local → remote (GitHub).

  ```bash
  git push origin main
  ```

- `origin` = the name of your remote repository.
- `main` = the branch you’re pushing to.

✅ After the first push (with `-u`), you can simply use:

  ```bash
  git push
  ```

---

## Quick Example Workflow

  ```bash
  git add index.html
  git commit -m "Updated homepage content"
  git push origin main
  ```

---

## 🚀 Recap

- `git add` → Stage your changes.
- `git commit` → Save changes locally.
- `git push` → Upload changes to GitHub.

---

> Next step → Learn the [File States](https://github.com/Akshat7garg/GitSnippets/blob/main/snippets/04_file_states.md).
