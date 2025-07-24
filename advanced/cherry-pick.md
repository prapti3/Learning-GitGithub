### 📄 cherry-pick.md
# 🍒 git cherry-pick – Pick Specific Commits Like a Pro

 - git cherry-pick lets you apply specific commits from one branch to another, without merging the whole branch.

  <br>

## 🔍 What Is Cherry-Picking?
```
- It’s like saying:
   - "I want just that one commit from another branch — not everything else."
- Great for:
1. Applying hotfixes from one branch to another.
2. Picking specific features from an experimental branch.
3. Avoiding full merges or rebases.

```


## ✅ Basic Command : 
`git cherry-pick <commit-hash>`
   - This takes that commit and applies it on top of your current branch.

---
<br>

## 🧠 Example Workflow
- You're on main and want to copy a commit from feature-1:
   ` git checkout main`
   ` git cherry-pick a1b2c3d`

- That’s it! 🎉
- The commit from feature-1 is now added to main.

---
<br>

## 🛠 Common Use Cases

### 🔥 Apply a Hotfix to Another Branch
```
git checkout main
git cherry-pick <bugfix-commit>
```

<br>


### 🧪 Bring One Feature Commit Without Full Merge
```
git checkout develop
git cherry-pick <feature-commit>
```

<br>

### ⚠️ Cherry-Pick Conflicts
- If conflicts occur during cherry-pick:

```
# Resolve the conflicts manually
git add .
git cherry-pick --continue
```

<br>

- To cancel:
```
git cherry-pick --abort
```

<br>

### 🚀 Multiple Commits
- You can cherry-pick a range:
`git cherry-pick A^..B`

- Where:
`A^..B means from parent of A to B (inclusive)`

---
<br>


## 🔁 Cherry-Pick vs Merge vs Rebase
| Operation       | Use Case                                 |
| --------------- | ---------------------------------------- |
| **merge**       | Bring all commits from a branch          |
| **rebase**      | Reapply all commits on a new base        |
| **cherry-pick** | Selectively apply **individual commits** |


---
<br>

### 🧠 Pro Tip
- Before cherry-picking, make sure:
- You're on the target branch.
- You’re picking from a clean and working commit.








