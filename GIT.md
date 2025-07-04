# Git & GitHub Cheatsheet

## 🔧 What is Git?

Git is a Version Control System. It is:
- ✅ Popular
- ✅ Free & Open Source
- ✅ Fast & Scalable

Git helps:
- 🕓 Track changes in code (Version Control)
- 🤝 Collaborate with others

---

## 🌐 What is GitHub?

GitHub is a website that allows developers to **store and manage their code** using Git.

- Folders are called **Repositories** (or **Repos**)

---

## 🧠 Basic Commands

### Check Git Version

git --version

##Terminal Basics

ls        # List files
clear     # Clear screen
pwd       # Print working directory
cd        # Change directory

### 📥 Clone a Repository

git clone <project-link>

### Check Repo Status

git status

Status types:

untracked – new files
modified – changed
staged – ready to commit
unmodified – unchanged

### ➕ Stage & Commit

git add filename
git add .             # stage all changes
git commit -m "msg"

### Push to GitHub

git push origin main

### 🏗️ Initialize New Repo

git init
git remote add origin <repo-url>
git remote -v           # verify
git branch -M main
git push origin main

### 🌿 Branching

git branch              # list branches
git branch -M main      # rename branch
git checkout <branch>   # switch
git checkout -b <new>   # create + switch
git branch -d <name>    # delete branch

### 🔀 Merge Code
## In VS Code Terminal

git diff <branch>      # show differences
git merge <branch>

## On GitHub

Create a Pull Request (PR)

### ⚠️ Merge Conflicts
When Git can't auto-merge two branches, you'll manually resolve code conflicts.

### 🔄 Undo Changes
## 1. Staged changes

git reset filename
git reset              # all files
## 2. Last commit

git reset HEAD~1
## 3. Specific commit

git reset <commit-hash>
git reset --hard <hash>

### 📜 Log History

git log
# Press `q` to quit

### 🍴 Fork
A fork is a copy of a repo under your account. It shares history with the upstream repo.
