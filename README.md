# Git Commands
## This Gist contains all the useful commands for Git 

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Version control is a system that records changes to a file or set of files over time so that you can recall specific versions later.

If you are a developer and want to keep every version of your code/project (which you would most certainly want to), a Version Control System (VCS) is a very wise thing to use.

- All the commands used for Git
- Compatibility with GitHub
- ✨Magic ✨

## Commands

This guide defines the **standard Git workflow** for the project. Following these practices ensures a clean history, reduces conflicts, and makes collaboration easier across the team.

---

## 🛠️ Git Workflow

### 1️⃣ Clone the repository
```bash
git clone <repository_url>
```

### 2️⃣ Navigate into the project directory
```bash
cd ascendum_poc
```

### 3️⃣ Checkout the base branch  
Replace `original_branch_name` with the actual base branch (e.g., `develop` or `main`):
```bash
git checkout original_branch_name
```

### 4️⃣ Pull the latest changes
```bash
git pull origin original_branch_name
```

### 5️⃣ Create and switch to a new feature branch  
Use a clear, descriptive branch name. For example:
```bash
git checkout -b feature/order_tracking_shivam
```

### 6️⃣ View commit history (optional)
```bash
git log              # detailed log
git log --oneline    # condensed log
```

### 7️⃣ Delete a remote branch (if required)
```bash
git push origin --delete branch_name
```

---

## 🧪 Development Workflow

### Stage your changes
```bash
git add .
```

### Check the status
```bash
git status
```

### Commit with a descriptive message  
Example messages:
- "Added API for order tracking"
- "Fixed UI issue in header"
```bash
git commit -m "Your descriptive commit message"
```

### Pull latest changes from base branch to stay updated  
Replace `main_branch_name` with your branch (`main` or `develop`):
```bash
git pull origin main_branch_name
```

### Push your feature branch to remote
```bash
git push origin your_branch_name
```

---

## ✅ Git Best Practices

- 🔄 **Always pull before pushing** to avoid merge conflicts.  
- 📝 **Write clear, meaningful commit messages**.  
- 🌿 **Never commit directly to `main` or `develop`.** Always use a feature branch.  
- 📥 **Regularly rebase or pull from `main`/`develop`** to keep your branch updated.  
- 🧪 **Test your changes locally** before committing or pushing.  
- 🔍 **Pull Request (PR) Guidelines:**
  - Ensure the PR compares against the correct base branch.
  - Provide a clear **title and description** of your changes.
  - 👥 Assign at least **one reviewer** for code review.
- 🚫 **Do not merge your own PR.** Merges should be handled by reviewers/leads after approval.  

---

## 📌 Example Workflow

**✅ Correct Workflow:**
```
Base Branch: develop
Feature Branch: feature/order_tracking_system <- shivam_changes
```

**❌ Incorrect Workflow:**
```
Base Branch: main <- shivam_changes
```

---

## 👥 Team Collaboration Notes

- Use **Pull Requests (PRs)** for all code contributions.  
- **Assign reviewers** and wait for approvals before merging.  
- **Document major changes or decisions** in the PR description for clarity.  

---

