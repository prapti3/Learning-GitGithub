
---

### 📄 7. `branch-rename.md`

**🔹 Purpose:** Rename branches locally and remotely.

**✅ Contents:**

```md
# ✏️ Renaming Git Branches

## 🔄 Rename current branch

```bash
git branch -m <new-name>

```

#### ✅ Example:
`git branch -m main production`

#### 🌍 Rename remote branch
`git push origin <new-name>`
`git push origin --delete <old-name>`


#### 🔁 Update tracking
`git branch --unset-upstream`
`git branch -u origin/<new-name>`

