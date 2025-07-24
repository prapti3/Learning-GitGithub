

### 📄 4. `conflicts.md`

**🔹 Purpose:** Handle and resolve merge conflicts during collaboration.

**✅ Contents:**

```md
# ⚔️ Merge Conflicts in Git

Merge conflicts happen when Git can't automatically combine changes.

## 🛠️ What to do:

1. Git will mark conflict areas like this:

```diff
<<<<<<< HEAD
your changes
=======
incoming changes
>>>>>>> feature/login

2. Manually fix the conflict in the file.
3. Then run:
  `git add <conflicted-file>`
  `git commit`

```

## ✅ Tips to Avoid Conflicts
- Always pull latest changes before merge.
- Communicate with your team.

  



