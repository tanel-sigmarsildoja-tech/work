# GitHowTo Learning Notes & Workflow Guide

Summary on completing the [GitHowTo](https://githowto.com/) interactive tutorial. This is its progress and notes in a repository made for coursework.

---

## What I Learned

Throughout this project, I gained hands-on experience with fundamental version control concepts:

* **Repository Initialization, Tracking Changes:** Understanding how Git tracks file changes in a local directory.
* **Staging Area Mechanics:** Preparing specific file changes before committing them to history.
* **Commit History Navigation:** Inspecting, filtering, and rolling back previous commits safely.
* **Branching and Merging:** Working on isolated features and combining them back into the main codebase.
* **Conflict Resolution:** Managing and resolving code conflicts during merge operations.
* **Working with an External Repository:** Pushing changes into an external repository like GitHub.
---

## Core Git Commands and Workflow

### 1. Workflow

```bash
# Status of working directory and staging area
git status

# Stage changes for the next commit
git add file.txt     (one file)
git add .     (all files)

# Save staged changes into the project history with a comment
git commit -m "New feature description"

# Make the changes in an external repository in the main branch of repository repo
git push -uf repo main
```

### 2. History


```bash
# Display detailed commit logs
git log

# Display one-line commit log
git log --oneline --graph
```

### 3. Branching and Merging
Isolating new work using branches prevents breaking the main codebase:

```bash
# Create and switch to a new style branch
git switch -c style      (-c is for create)

# Switch back to the main branch
git switch main

# Merge the style branch into main
git switch style     (if not yet on style, check with git status)
git merge main
! git rebase x applies active on top the x branch, git merge x applies or tries to apply x on top active branch
```

---

## Checklist

- [x] Complete GitHowTo basic exercises
- [x] Staging and committing changes
- [x] Branching and switching between branches
- [x] Perform successful branch merge operations including merge failures and how to fix them
- [x] Create documentation in README.md
- [x] Push it all onto GitHub

---
