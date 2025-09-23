# Git Basics: Forking a Repository

Forking means creating your **own copy of someone else’s repository** on GitHub.  
It lets you freely experiment, make changes, and propose improvements via Pull Requests (PRs).  

---

## 1. What is a Fork?

- A **fork** is like a clone of a GitHub repo under **your account**.  
- You can modify it without affecting the original project.  
- Useful for **open-source contributions** and learning.  

---

## 2. How to Fork a Repo (on GitHub)

1. Go to the repository you want to fork.  
2. Click the **Fork** button (top-right of GitHub).  
3. Choose your account → GitHub creates a copy of the repo under your profile.  

---

## 3. Work on Your Fork

1. Clone your fork to your local machine:

  ```bash
  git clone https://github.com/<your-username>/<repo-name>.git
  cd <repo-name>
  ```

2. Add the original repository (upstream) for syncing:

  ```bash
  git remote add upstream https://github.com/<original-owner>/<repo-name>.git
  ```

3. Verify remotes:

  ```bash
  git remote -v
  ```

### You’ll see

  ```bash
  origin    https://github.com/<your-username>/<repo-name>.git (your fork)
  upstream  https://github.com/<original-owner>/<repo-name>.git (original repo)
  ```

---

## 4. Keep Your Fork Updated

Before making new changes, sync with the original repo:

  ```bash
  # Fetch latest changes from upstream
  git fetch upstream
  
  # Merge them into your local main branch
  git checkout main
  git merge upstream/main
  ```

Push updates to your fork:

  ```bash
  git push origin main
  ```

---

## 5. Contribute Back (Pull Request)

1. Create a feature branch in your fork:

  ```bash
  git switch -c feature-xyz
  ```

2. Make changes → commit → push:

  ```bash
  git add .
  git commit -m "Added feature xyz"
  git push origin feature-xyz
  ```

3. Go to your fork on GitHub → Click “**Compare & Pull Request**”.
4. Submit a **PR** to the original repo for review.

---

🚀 Recap

- **Fork** = Copy repo under your GitHub account.
- **Origin** = Your fork.
- **Upstream** = Original repo.
- **Sync frequently** with upstream before contributing.
- **Pull Request** = Suggest your changes back to the original project.

---

> Next step → Learn about [Merge, Rebase & Remote](https://github.com/Akshat7garg/GitSnippets/blob/main/snippets/10_merge_rebase_remote.md).
