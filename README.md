## 📌 Table of Contents

- [Git & GitHub — Learning Basics](#git--github--learning-basics)
- [What is Git?](#what-is-git)
  - [Commit](#commit)
  - [Branching](#branching)
  - [Push vs Pull](#push-vs-pull)
  - [Git Init](#git-init)
  - [Common Git Commands](#common-git-commands)
- [What is GitHub?](#what-is-github)
  - [Why Use GitHub?](#why-use-github)
- [Push From Git To GitHub](#push-from-git-to-github)
- [Summary](#summary)
---

# Git & GitHub — Learning Basics

## What is Git?
**Git** is a version control system used to **track changes made in the codebase**.

---

### Commit
- A **commit** acts as a **checkpoint** in our code.
- We can commit changes for different parts of a project such as *header*, *body*, *footer*, *payment gateway*, etc.
- A commit can be understood as a **snapshot/screenshot of the current state of the code**.
- We can **go back to any previous state** of the code from the time it was committed.

---

## Branching
A **branch** is a separate line of development in Git.

### Why Use Branches?
- Allows developers to **work on features independently**
- Helps avoid **breaking the main code**
- Makes team collaboration safer and cleaner

- Default branch is usually:
  - **main**
  - **master**
    
### Common Branch Commands
- *git branch* → List all branches  
- *git branch feature-login* → Create a new branch  
- *git checkout feature-login* → Switch to the branch
- *git checkout -b new_branch_name* -> creates new branch
- *git checkout -d X* -> deletes branch X (possible only when we are not not in X)

---

## Merging

A **merge** is the process of combining changes from one branch into another in Git.

### Why Use Merging?
- Brings completed features into the **main** branch  
- Combines work from multiple developers  
- Keeps project history organized  
- Integrates tested code into production  

### How Merging Works
When you merge:
- Git takes the changes from one branch  
- Combines them with the current branch  
- Creates a **merge commit** (if needed)  

Example workflow:
1. Create a feature branch  
2. Work on it  
3. Switch back to main  
4. Merge the feature branch  

### Common Merge Commands
- *git checkout main* → Switch to main branch  
- *git merge feature-login* → Merge feature-login into main  
- *git merge --no-ff branch_name* → Force a merge commit  
- *git branch -d branch_name* → Delete branch after merging  

### Types of Merge
1. **Fast-Forward Merge**
   - Happens when there are no new commits in main  
   - Git simply moves the pointer forward  
   - No merge commit is created  

2. **Three-Way Merge**
   - Happens when both branches have new commits  
   - Git creates a merge commit  
   - Keeps full history visible  

### Merge Conflicts
A **merge conflict** happens when:
- Two branches modify the same line of code  
- Git cannot automatically decide which change to keep  

To resolve:
1. Open the conflicted file  
2. Edit and fix the conflict  
3. *git add file_name*  
4. *git commit*  

---


## Push vs Pull

### git push
- Used to **upload local commits** to GitHub
- Sends your changes from **local system → remote repository**

### git pull
- Used to **download latest changes** from GitHub

---

## git init
- To initialize a new folder as git folder on our local system, we use `GIT INIT`.
CODE:
```
- git init
- git remote add origin githubLink
- git push origin main / git push -u origin main
# Extra:
  1. git remote -v (verify remote)
  2. git branch (check branch)
  3. git branch -M newName (rename a branch name to newName/or anything written here)
  4. -u: upstreaming, then from next time just write git push
```
---

## Common Git Commands
- *git clone <url>* → Download a repository from the internet  
- *ls -a* → Show all files including hidden files  
- *git status* → Shows whether any files are updated and need to be committed.

---

## What is GitHub?
**GitHub** is a centralized platform where code is stored using Git.

### Why Use GitHub?
- Acts as a **centralized system** for storing code
- Makes it easy to **store and share** code
- Can be used as:
  - **Personal code storage**
  - A **collaboration tool in companies**, where developers can download and work on code changes committed by others
We can cllaborate with other developers here and write codes in parallel working on different features.

---

# Push From Git To GitHub:
1. Get git repo on the system
   - git clone "repo-link"
2. Move to that folder using termial cd ...
2. Make changes in the downloaded folder (update/delete), then do following steps while being in the same folder
3. Check git status to make sure changes are done:
   - git status

4. Add all changes into git
   - git add .

5. Commit changes
   - git commit -m "Message for the update"

6. Update to GitHub (Local to Repo)
   - git push origin main

- Brings updates from **remote repository → local system**

---
# Summary
- **Git** helps track changes and manage different versions of code efficiently
- **Commits** act as checkpoints, allowing developers to revert to previous stable states
- **Branching** enables parallel development and safer feature implementation without affecting the main codebase
- **GitHub** serves as a centralized platform to store, share, and collaborate on Git repositories
- **Push and Pull operations** help keep local and remote repositories in sync
- Together, **Git and GitHub** improve code reliability, team collaboration, and overall development workflow
- To merge different branches, we use merge keyword
