# Git Snippets: Merging Code

Merging means combining changes from one branch into another.  
There are **two common ways to merge**: via **Pull Requests (PRs)** on GitHub, or by merging branches directly in your local repo.  

---

## 1. Merging with Pull Requests (PRs)

Pull Requests are the **recommended way** to merge in collaborative projects.  
They allow code review, discussion, and approval before merging.  

### Steps

1. Create a new branch and push it to GitHub:

  ```bash
  git switch -c feature-xyz
  # make changes
  git add .
  git commit -m "Added feature xyz"
  git push -u origin feature-xyz
  ```

2. Go to your repository on GitHub → you’ll see a “**Compare & Pull Request**” button.

3. Open a Pull Request:

- Choose the base branch (usually `main`) and compare it with your feature branch.
- Add a description of your changes.
- Submit the PR.

4. Teammates review, comment, and approve.

5. Merge the PR (via **Merge**, **Squash**, or **Rebase** options GitHub provides).

---

## 2. Merging Branches Locally (Same Repo)

If you’re working alone or want to merge directly without a PR:

Example:

1. Switch to the branch you want to merge into (usually main):

  ```bash
  git switch main
  ```

2. Merge the feature branch:

  ```bash
  git merge feature-xyz
  ```

3. If no conflicts → Git automatically merges.  
   If conflicts → you must resolve them manually, then commit.

4. Push the updated main branch back to GitHub:

  ```bash
  git push origin main
  ```

---

## 3. Visual Overview

  ```bash
  # Pull Request Workflow
  feature-branch → GitHub PR → Review → Merge → main
  
  # Local Merge Workflow
  git switch main → git merge feature-branch → git push
  ```

---

## 🚀 Quick Recap

- **Pull Requests (PRs)** → Best for teams, allows review and collaboration.
- **Local Merge** → Faster, good for solo projects or simple merges.

---

> Next step → Learn to [Undo Changes](https://github.com/Akshat7garg/GitSnippets/blob/main/snippets/07_undo.md).
