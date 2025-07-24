# 🔀 Resolve Merge Conflicts in Git

Merge conflicts happen when Git can't automatically combine changes from two branches. This typically occurs when:
- Two people edit the same line in a file.
- One person edits a file while another deletes it.
- Changes are made on both sides before merging or rebasing.

---
<br>

## 🚨 What a Conflict Looks Like

In your file, you'll see something like this:

```diff
<<<<<<< HEAD
console.log("Hello from main");
=======
console.log("Hello from feature");
>>>>>>> feature/login

```

## 🛠 Steps to Resolve a Merge Conflict

### 1. Identify Conflicted Files
- git status
- Output : `both modified:   src/app.js`

---
<br>

### 2. Open and Manually Edit Conflicts

- In each conflict block:
- Remove the markers: <<<<<<<, =======, and >>>>>>>
- Keep the version you want (or combine both appropriately)

#### Example : 
- // ✅ Final version
- console.log("Hello from feature and main");
  
---
<br>


---
<br> 

### 3. Add the Resolved Files
`git add src/app.js`

<br> 

### 4. Complete the Merge or Rebase
- If you're merging: `git commit`
- If you're rebasing: `git rebase --continue`


<br> 


### 💡 Conflict Resolution Tips

- Use a merge tool: `git mergetool`
- Use a good diff editor like VSCode, IntelliJ, or Beyond Compare.
- Communicate with your team if you're unsure what changes to keep.
- Commit frequently to avoid large, hard-to-merge changes.

### Example : 
```
# You are on main
git pull origin main

# Start feature work
git checkout -b feature/cart
# ...make changes...
git commit -am "Updated cart logic"

# Try to merge main
git checkout main
git pull origin main
git merge feature/cart
# ❌ Merge conflict occurs!
```
##### Now resolve conflicts, add files, and complete the merge.

<br> 

### 📦 Summary Table:
| Command                     | Description                       |
| --------------------------- | --------------------------------- |
| `git status`                | Shows which files have conflicts  |
| `git add <file>`            | Mark a file as resolved           |
| `git commit` / `--continue` | Finalize merge or rebase          |
| `git merge --abort`         | Cancel the merge (if needed)      |
| `git mergetool`             | Use GUI tool to resolve conflicts |


--- 
<br> 


### ✅ Best Practices
- Pull often to minimize conflicts.
- Break large PRs into smaller ones.
- Clearly comment your changes.
- Use topic branches to isolate work.


### Conflicts are a natural part of collaboration. Don’t panic — resolve and move forward! 🚀



  



