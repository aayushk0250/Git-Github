# Git & GitHub — Learning Basics

## What is Git?
**Git** is a version control system used to **track changes made in the codebase**.

### Commit
- A **commit** acts as a **checkpoint** in our code.
- We can commit changes for different parts of a project such as *header*, *body*, *footer*, *payment gateway*, etc.
- A commit can be understood as a **snapshot/screenshot of the current state of the code**.
- We can **go back to any previous state** of the code from the time it was committed.

---

## Common Git Commands
- *git clone <url>* → Download a repository from the internet  
- *ls -a* → Show all files including hidden files  
- *git status* → Shows whether any files are updated and need to be committed  

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
3. Check git status to make sure changes are done
   - git status

4. Add all changes into git
   - git add .

5. Commit changes
   - git commit -m "Message for the update"

6. Update to GitHub
   - git push origin main


---
## Summary
- **Git** helps track changes and manage different versions of code
- **GitHub** is like a centralized system that helps to store, share, and collaborate on Git repositories
