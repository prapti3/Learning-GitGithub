# 🔄 git reset

`git reset` is used to **undo changes** by moving the current HEAD and optionally changing the staging area or working directory.

---

## 🔹 Types of Reset

| Type       | Affects Commit | Affects Staging | Affects Working Dir |
|------------|----------------|------------------|----------------------|
| `--soft`   | ✅              | ❌                | ❌                    |
| `--mixed`  | ✅              | ✅                | ❌                    |
| `--hard`   | ✅              | ✅                | ✅                    |

---

## ✅ Common Use Cases

### 1. Undo last commit but keep changes staged
- bash
`git reset --soft HEAD~1`

- 🔸 Moves HEAD back, but your changes stay in staging.
  
---

## 2. Unstage changes (keep changes in working dir)

`git reset --mixed HEAD` : Removes from staging, but doesn't delete your changes.

---

## 3. Completely undo everything (careful!)

`git reset --hard HEAD~1` : ⚠️ Permanently deletes last commit + all uncommitted changes.

---

## 🧪 Example Flow

a) echo "hello" >> demo.txt
b) git add .
c) git commit -m "Add demo"

# Now undo:
1. git reset --soft HEAD~1   # Keep changes staged
2. git reset --mixed HEAD~1  # Keep changes in file, not staged
3. git reset --hard HEAD~1   # Delete everything

---

## 🔍 Reset to specific commit

`git reset --hard <commit-id>`
`git log --oneline` : You can find the commit ID from:

---

## 🧠 Tips

-- hard is dangerous! Use only if you're sure.
-- Use git reflog to recover accidentally deleted commits.
-- Prefer git restore for unstaging or discarding files (safer).





