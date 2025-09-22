# Git Setup Guide

This guide will help you **install Git** on your system and configure it for the first time.  

---

## 1. Install Git

### 🖥️ Windows
- Download the latest version of Git from [git-scm.com](https://git-scm.com/download/win).  
- This will install **Git Bash**, a terminal application where you can run Git commands.  
- During installation, you can keep most settings default. Make sure:
  - ✅ "Git Bash Here" is enabled (for right-click menu).
  - ✅ Default editor is set to *VS Code* (or your preferred editor).
  - ✅ Use "main" as the default branch name.

### 🍎 macOS
- If you have **Homebrew** installed:
  ```bash
  brew install git
  ```

- Or, install **Xcode** Command Line Tools:
  ```bash
  xcode-select --install
  ```

- Alternatively, download directly from [git-scm.com](https://git-scm.com/download/win).

### 🐧 Linux (Ubuntu/Debian)
- Update packages and install Git:

  ```bash
  sudo apt update
  sudo apt install git
  ```

### 🐧 Linux (Fedora)

  ```bash
  sudo dnf install git
  ```

### ✅ Verify Installation
After installation, check your Git version:

  ```bash
  git --version
  ```

---

## 2. Configure Git (First-Time Setup)
You need to tell Git who you are (name & email). This info is used for commits.

### Set Username
  ```bash
  git config --global user.name "Your Name"
  ```

### Set Email
  ```bash
  git config --global user.email "your.email@example.com"
  ```

>⚠️ Use the same email that you registered with GitHub so commits are linked to your profile.

### Check Configuration
  ```bash
  git config --list
  ```

### Example Output
  ```bash
  user.name=John Doe
  user.email=johndoe@example.com
  ```

---

## 3. Optional but Recommended Configuration

### Set Default Branch Name to `main`
  ```bash
  git config --global init.defaultBranch main
  ```

### Set VS Code as Default Editor
  ```bash
  git config --global core.editor "code --wait"
  ```

### Enable Color in Git Output
  ```bash
  git config --global color.ui auto
  ```

---

## 4. Where is Git Config Stored?
Git saves your settings in a file on your system:
- Global config: `~/.gitconfig` (applies to all repositories)
- Local config: `.git/config` (inside a specific repository)

---

## ✅ You’re Ready!
At this point:

- Git is installed.
- Your identity is set.
- You’re ready to create repositories and start committing code.

---

> Next step → Learn the [Common terms in GitHub](https://github.com/Akshat7garg/GitSnippets/blob/main/guides/glossary.md).
