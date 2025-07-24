### 📄 3. `merge.md`

**🔹 Purpose:** Understand how to bring changes from one branch into another.

**✅ Contents:**

```md
# 🔀 Git Merge

Merging combines histories of two branches.

## ✨ Merge a branch into current branch

```bash
git merge <branch-name>

## ✅ Example:
# Merge 'feature/login' into current branch (main)
git merge feature/login

💡 Fast-forward vs 3-way merge
Fast-forward: Direct pointer movement.

3-way merge: Git creates a new merge commit.
