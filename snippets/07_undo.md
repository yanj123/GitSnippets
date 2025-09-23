# Git Snippets: Undo Changes

Sometimes you make a mistake — maybe you staged the wrong file, wrote a bad commit message, or need to roll back multiple commits.  
Git provides different commands for different situations.  

---

## Case 1: Undo Staged / Added Changes (Before Commit)

You used `git add` but haven’t committed yet.

### Unstage a Specific File

  ```bash
  git reset HEAD filename.txt
  ```

### Unstage All Files

  ```bash
  git reset HEAD
  ```

✅ This removes files from the staging area, but your changes still remain in the working directory.  
You can re-add them later if needed.

---

## Case 2: Undo the Last Commit (1 Commit Only)

You committed by mistake, but haven’t pushed to GitHub yet.

### Option A: Keep Changes (but uncommit them)

  ```bash
  git reset --soft HEAD~1
  ```

- Removes the last commit.
- Changes stay staged → ready for a new commit.

### Option B: Keep Changes (unstaged)

  ```bash
  git reset --mixed HEAD~1
  ```

- Removes the last commit.
- Changes move back to unstaged.

### Option C: Delete Commit & Changes

  ```bash
  git reset --hard HEAD~1
  ```

- Completely erases the last commit and the changes.  
  ⚠️ Use with caution.

---

## Case 3: Undo Multiple Commits

### Undo Last 3 Commits (but keep changes unstaged)

  ```bash
  git reset --mixed HEAD~3
  ```

### Undo Last 3 Commits (delete commits + changes)

  ```bash
  git reset --hard HEAD~3
  ```

### Alternative: Revert Commits (Safer)

If you already pushed to GitHub and want to undo without rewriting history:

  ```bash
  git revert <commit-hash>
  ```

- Creates a **new commit** that undoes the changes from the given commit.
- Safer than reset because it keeps history intact.

### Example (undo last 3 commits safely)

  ```bash
  git revert HEAD~2..HEAD
  ```

---

## 🚀 Quick Recap

- **Unstage changes** → `git reset HEAD <file>`
- **Undo 1 commit** → `git reset --soft/mixed/hard HEAD~1`
- **Undo multiple commits** → `git reset HEAD~N`
- **Safe undo (after push)** → `git revert <commit>`

---

## ✅ Rule of thumb

- Use **reset** when working locally (before pushing).
- Use **revert** when you’ve already pushed to GitHub.

---

> Next step → Learn few more [Basic Concepts](https://github.com/Akshat7garg/GitSnippets/blob/main/snippets/08_next_basics.md).
