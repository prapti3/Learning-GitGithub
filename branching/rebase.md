

### 📄 5. `rebase.md`

**🔹 Purpose:** Learn about rebasing to maintain clean commit history.

**✅ Contents:**

```md
# 🔁 Git Rebase

Rebase moves your branch commits onto another branch’s latest commit.

## 💡 Why Rebase?

- Keep linear history
- Avoid merge commits

## 🔧 Basic Syntax

```bash
git rebase <base-branch>


```

## Example : 
`git checkout feature/cart`
`git rebase main`

## ⚠️ Use with care : 
- Never rebase shared/public branches


---

### 📄 6. `branch-delete.md`

**🔹 Purpose:** Safely delete unwanted branches (local and remote).

**✅ Contents:**

```md
# 🗑️ Deleting Git Branches

## 🧹 Delete a local branch

```bash
git branch -d <branch-name>

Use -D for force delete


```

## ❌ Delete a remote branch : `git push origin --delete <branch-name>`

## ✅ Example: `git push origin --delete feature/login`

## 💡 Tip:
- Only delete branches after confirming they are merged or no longer needed.





