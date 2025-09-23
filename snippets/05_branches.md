# Git Snippets: Working with Branches

Branches let you **work on features or fixes** without touching the `main` code.  
They are like separate “timelines” of your project that you can merge later.

---

## 1. View Branches

List all branches:

  ```bash
  git branch
  ```

List branches with remote ones:

  ```bash
  git branch -a
  ```

Show current branch:

  ```bash
  git status
  ```

---

## 2. Create a Branch

Create a new branch:

  ```bash
  git branch feature-xyz
  ```

Create and switch in one step (recommended):

  ```bash
  git switch -c feature-xyz
  ```

---

## 3. Switch Between Branches

Switch to an existing branch:

  ```bash
  git switch feature-xyz
  ```

Older syntax (still works):

  ```bash
  git checkout feature-xyz
  ```

---

## 4. Rename a Branch

Rename the current branch:

  ```bash
  git branch -m new-branch-name
  ```

---

## 5. Delete a Branch

Delete a local branch (after merging):

  ```bash
  git branch -d branch-name
  ```

Force delete (⚠️ even if not merged):

  ```bash
  git branch -D branch-name
  ```

Delete a remote branch:

  ```bash
  git push origin --delete branch-name
  ```

---

## 6. Push Branch to GitHub

If it’s the first time pushing the branch:

  ```bash
  git push -u origin branch-name
  ```

After that, just:

  ```bash
  git push
  ```

---

## 7. Merge Branches

Switch to the branch you want to merge into (usually `main`):

  ```bash
  git switch main
  ```

Merge another branch into it:

  ```bash
  git merge feature-xyz
  ```

---

## 8. Resolve Merge Conflicts (If Any)

If Git can’t auto-merge, it will mark conflicts inside files like this:

  ```bash
  <<<<<<< HEAD
  Code from main

  =======
  
  Code from feature-xyz
  >>>>>>> feature-xyz
  ```

Steps:

- Edit the file and choose the correct code.
- Stage it again:

  ```bash
  git add conflicted-file.txt
  ```

- Complete the merge:

  ```bash
  git commit
  ```

---

## 🚀 Quick Recap

- `git branch` → list branches
- `git switch -c new-branch` → create & switch
- `git merge` → combine branches
- `git push -u origin branch-name` → share branch on GitHub
- `git branch -d branch-name` → delete a branch

---

> ✅ Branches make teamwork easy: each person can work on features safely, then merge into the main project when ready.

> Next step → Learn to [Merge Codes](https://github.com/Akshat7garg/GitSnippets/blob/main/snippets/06_merging.md).
