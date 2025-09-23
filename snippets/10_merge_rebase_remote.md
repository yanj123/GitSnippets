# Git Snippets: Merge, Rebase & Remote

This file explains two big areas:  

1. How to combine changes → `merge` vs `rebase`  
2. How to work with remote repositories → `git remote add`, `git push`, `git pull`  

---

## 1. Merge vs Rebase

### 🟢 `git merge`

- Combines changes from one branch into another.  
- Creates a **new commit** called a *merge commit*.  
- Preserves branch history.  

Example:

  ```bash
  git switch main
  git merge feature-xyz
  ```

✅ Easy to use, good for teamwork.  
⚠️ History can get “messy” with many merge commits.

---

## 🟡 git rebase

- **Moves** (or reapplies) commits from one branch onto another.
- **Creates a clean, linear history** (no merge commits).

Example:

  ```bash
  git switch feature-xyz
  git rebase main
  ```

✅ Cleaner history.
⚠️ Can be confusing; avoid rebasing shared branches (use on local branches).

---

## 🔄 Visual Difference

  ```bash
  Merge:              Rebase:
  A---B---C main      A---B---C main
         \                \
          D---E feature     D'--E' feature
  ```

---

## 2. Working with Remotes

Remotes are links to repositories hosted online (like GitHub).

### List Remotes

  ```bash
  git remote -v
  ```

### Add a Remote

  ```bash
  git remote add origin https://github.com/<user>/<repo>.git
  ```

### Remove a Remote

  ```bash
  git remote remove origin
  ```

### Rename a Remote

  ```bash
  git remote rename origin upstream
  ```

---

3. Push & Pull

### Push (Local → Remote)

  ```bash
  git push origin main
  ```

Uploads local commits to the `origin` remote, `main` branch.

First-time push with tracking:

  ```bash
  git push -u origin main
  ```

### Pull (Remote → Local)

  ```bash
  git pull origin main
  ```

This = `git fetch` + `git merge`.  
It updates your local branch with the latest changes from GitHub.

---

## Fetch (Remote → Local without merge)

  ```bash
  git fetch origin
  ```

Downloads new commits from remote but doesn’t merge them.

---

## 🚀 Recap

- **Merge** = Keeps history, adds merge commit.
- **Rebase** = Cleaner history, rewrites commits.
- **Remote** = Link to GitHub repo (`origin`, `upstream`).
- **Push** = Upload local → remote.
- **Pull** = Download + merge remote → local.
- **Fetch** = Just download, no merge.

---

> Next step → you can also explore [Printed Cheatsheet](https://github.com/Akshat7garg/GitSnippets/blob/main/CHEATSHEET.md).
