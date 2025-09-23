# Introduction to Git & GitHub

## What is Git?

Git is a **distributed version control system (DVCS)** created by Linus Torvalds in 2005.  
It helps developers **track changes in code**, **collaborate with others**, and **manage different versions** of a project.  

### Key features of Git

- Tracks every change in your project (version history).
- Works offline (local repositories on your machine).
- Supports branching and merging for parallel development.
- Reliable and widely used in the software industry.

---

## What is GitHub?

[GitHub](https://github.com) is a **cloud-based hosting service** for Git repositories.  
It provides a platform for **collaboration, code sharing, and project management**.  

Think of Git as the **tool** and GitHub as the **platform** where you can publish, share, and work together with others.  

### Why GitHub?

- Store and share your Git repositories online.
- Collaborate with teams across the world.
- Manage projects with issues, pull requests, and discussions.
- Showcase your work (open-source contributions, portfolios).
- Integrates with CI/CD tools, project boards, and wikis.

---

## Use Cases of Git & GitHub

- **Team Collaboration** → Developers can work on the same project without conflicts.
- **Open-Source Contributions** → Contribute to global projects like Linux, React, or TensorFlow.
- **Backup & Remote Access** → Your code is safe in the cloud and accessible anywhere.
- **Version Tracking** → Roll back to earlier versions of your code if something breaks.
- **Portfolio Building** → Display your projects to recruiters or collaborators.

---

## Basic GitHub Workflow (Simplified)

Here’s the typical flow when working with Git and GitHub:

1. **Create / Clone a Repository**
   - Start a new project with `git init` or download an existing one with `git clone`.

2. **Make Changes Locally**
   - Edit files on your machine.

3. **Stage & Commit**
   - Stage changes:  

     ```bash
     git add <file-name>
     ```

   - Save a snapshot:  

     ```bash
     git commit -m "Your message"
     ```

4. **Push to GitHub**
   - Upload your local commits to GitHub:  

     ```bash
     git push origin main
     ```

5. **Collaborate**
   - Teammates create branches, commit changes, and push them.
   - Changes are reviewed via **Pull Requests** before merging into the main branch.

6. **Update Your Copy**
   - Keep your repo in sync with the remote:  

     ```bash
     git pull origin main
     ```

---

## Visual Overview of GitHub Flow

Local Work → Commit → Push → Pull Request → Review → Merge → Update

---

> ✅ Now you understand **what Git is**, **what GitHub is**, **why they’re important**, and the **workflow to use them effectively**.

> Next step → Learn the [Installation & Setup](https://github.com/Akshat7garg/GitSnippets/blob/main/guides/02_setup.md).
