# Git & GitHub Glossary

A beginner-friendly glossary of commonly used Git and GitHub terms.  

---

## A

**Add**  
Command to stage files for the next commit. Example:  

  ```bash
  git add file.txt
  ```

**Branch**  
A separate line of development. Lets you work on new features without affecting the main code.

**Clone**  
Copy a remote repository from GitHub to your local machine.

  ```bash
  git clone <repo-url>
  ```

---

## C

**Commit**  
A snapshot of your changes in the repository. Each commit has a unique ID (hash).

**Conflict (Merge Conflict)**  
Happens when two people make changes to the same part of a file and Git doesn’t know which to keep. Must be resolved manually.

---

## F

**Fork**  
A personal copy of someone else’s GitHub repository. Common in open-source contributions.

**Fetch**  
Downloads changes from a remote repository but does not merge them automatically.

  ```bash
  git fetch
  ```

---

## G

**Git**  
A distributed version control system that tracks changes in your code.

**GitHub**  
A cloud-based platform for hosting and collaborating on Git repositories.

---

## L

**Local Repository**  
A repository stored on your personal computer.

---

## M

**Main (or Master)**  
The default primary branch in a Git repository.

**Merge**  
Combines changes from one branch into another.

---

## P

**Pull**  
Downloads and merges changes from a remote repository to your local repo.

  ```bash
  git pull
  ```

**Push**  
Uploads your local commits to a remote repository (e.g., GitHub).

  ```bash
  git push
  ```

**Pull Request (PR)**  
A GitHub feature where you propose changes to be reviewed and merged into the main branch.

---

## R

**Remote**  
A version of your project that is hosted on GitHub (or another server).

**Repository (Repo)**  
A project folder that Git tracks. It can be local or hosted on GitHub.

**Revert**  
Undo a commit by creating a new commit that reverses the changes.

  ```bash
  git revert <commit-hash>
  ```

**Reset**  
Moves the repository back to a previous state. ⚠️ Can be destructive if used incorrectly.

---

## S

**Stage (Staging Area / Index)**  
A place where Git collects changes before committing them.

---

## T

**Tag**  
A label that marks specific commits, often used for version releases.

**Terminal / Shell**  
A command-line interface where you run Git commands.

---

> ✅ This glossary will keep expanding as you learn more commands and concepts.

> Next step → Explore [Git Snippets](https://github.com/Akshat7garg/GitSnippets/blob/main/snippets/01_create_repository.md).
