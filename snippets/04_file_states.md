# Git Snippets: File States in Git

In Git, every file in your project goes through **4 main states**.  
Understanding these states is key to using Git effectively.  

---

## 1. Untracked (Unstaged)

- Files that are new and not yet tracked by Git.  
- Git does not include them in commits until you **stage** them.  

Check status:

  ```bash
  git status
  ```

Example output:

  ```bash
  Untracked files:
    newfile.txt
  ```

Move to staged state:

  ```bash
  git add newfile.txt
  ```

---

## 2. Staged

- Files that have been marked to be included in the next commit.
- They are ready to be saved.

Example:

  ```bash
  git add file.txt
  ```

Check status:

  ```bash
  git status
  ```

Output:

  ```bash
  Changes to be committed:
    new file: file.txt
  ```

---

## 3. Modified

- Files that are tracked by Git but have changes **not yet staged**.
- Git knows they’ve been changed, but they won’t be included in the next commit until you add them.

Example workflow:

  ```bash
  # Edit file.txt
  git status
  ```

Output:

  ```bash
  Changes not staged for commit:
    modified: file.txt
  ```

To stage it:

  ```bash
  git add file.txt
  ```

---

## 4. Unmodified (Clean)

- Files that are tracked and have **no changes** compared to the last commit.
- The working directory is “clean.”

Check:

  ```bash
  git status
  ```

Output:

  ```bash
  nothing to commit, working tree clean
  ```

---

## 🚀 Quick Recap

- `Untracked` → New file, not added yet.
- `Staged` → Ready to be committed.
- `Modified` → Changed, but not staged.
- `Unmodified` → No changes since last commit.

---

> Next step → Explore [Branches](https://github.com/Akshat7garg/GitSnippets/blob/main/snippets/05_branches.md).
