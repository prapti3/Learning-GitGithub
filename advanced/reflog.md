# 📄 reflog.md

## 🧭 git reflog – Your Git Time Machine

- git reflog lets you view the history of all your local Git actions, even those that don’t show up in git log—like commits that were lost after a reset, rebase, or amend.

<br>

## 🚀 Why Use git reflog?
- Recover lost commits.
- See the history of all branch changes.
- Undo a reset, rebase, or commit --amend.
- Help debug "where did my commit go?" situations.


--- 
<br>

### 🔍 Basic Command
`git reflog`

- Example
  ```
  a12b3cd HEAD@{0}: reset: moving to HEAD~1
  d34e5fg HEAD@{1}: commit: Added login form
  c78d9ef HEAD@{2}: rebase finished
  ```
- This tells you what happened at each step and lets you "go back in time."

---
<br>

## 🛠 Common Use Cases

### 🔙 Undo a Reset
```
git reflog
git checkout <commit_hash>
```

- Then, optionally create a new branch from it:
`git checkout -b recovery-branch`



###  🔄 Go Back to a Previous State
`git reset --hard HEAD@{2}`
- Takes your branch back to how it was at that point.

### 💡 Check Branch Movements
`git reflog show main`
- See how the main branch has moved over time.

---
<br>

## 🔧 Real World Example

1. Oops! You ran: `git reset --hard HEAD~1`
- But you realize you lost a commit.
2. ✅ Use git reflog to find it: `git reflog`
3. Find the lost commit hash and recover it: `git checkout <hash>`

---
<br>

### 🧠 Quick Tips
- git log shows project history.
- git reflog shows HEAD movement, including checkout, reset, merge, etc.
- Use reflog to fix mistakes — it’s like Git undo history.









