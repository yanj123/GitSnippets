# Git Basics: Logs, Ignore Files, and Git Directory

Before diving deeper, let’s look at some essential Git concepts and commands that you’ll use frequently.

---

## 1. `git log` (View Commit History)

The `git log` command shows the history of commits in your repository.

  ```bash
  git log
  ```

Example output:

  ```bash
  commit a1b2c3d4e5f6 (HEAD -> main, origin/main)
  Author: John Doe <johndoe@example.com>
  Date:   Mon Sep 22 18:30:00 2025 +0530
  
      Added homepage layout
  ```

### Useful options

- Show a simplified one-line log:

  ```bash
  git log --oneline
  ```

### Show a graphical branch view

  ```bash
  git log --oneline --graph --all
  ```

✅ Helps you track changes and branch history.

---

## 2. `.gitignore` (Ignore Files)

A **.gitignore** file tells Git which files/folders to **ignore** (not track).

Example `.gitignore`:

  ```bash
  # Ignore OS/system files
  .DS_Store
  Thumbs.db
  
  # Ignore build artifacts
  /node_modules
  /dist
  /build
  
  # Ignore secrets
  .env
  ```

✅ Useful for excluding temporary files, large binaries, or sensitive data.

---

## 3. .git/ Directory (Hidden Git Folder)

When you run `git init`, Git creates a hidden folder called `.git/` inside your project.

This folder contains:

- **Commits and history** (`objects/`)
- **Branches and HEAD info** (`refs/`)
- **Config files** (`config`)
- **Staging information** (`index`)

⚠️ **Do not delete or edit `.git/` manually** — it’s the brain of your repository.
Deleting it will make your project “forget” all Git history.

---

## 4. `git status` (Quick Recap)

Another essential command:

  ```bash
  git status
  ```

Shows:

- Which branch you’re on.
- Which files are untracked, modified, or staged.
- What your next step should be (`git add` or `git commit`).

---

## 🚀 Recap

- `git log` → View commit history.
- `gitignore` → Tell Git what NOT to track.
- `git/ folder` → Stores repo history & config (hidden, don’t touch).
- `git status` → Check what’s going on at any moment.

---

> Next step → Learn to [Fork Repositories](https://github.com/Akshat7garg/GitSnippets/blob/main/snippets/09_fork.md).
