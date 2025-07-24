#📄 stash.md

##🧳 Git Stash
- Git stash is used to temporarily save changes in your working directory that you don't want to commit immediately. It's like putting your work in a drawer to come back to later.

<br>

## 📌 Why Use Git Stash?

- You want to switch branches but have uncommitted changes.
- You’re in the middle of a task but need to fix something urgent on another branch.
- You want to test something without committing incomplete work.

---
<br>

### 🧪 Basic Commands
- #### ➕ Save Your Changes : `git stash`

Saves all uncommitted changes (staged + unstaged) and reverts to the last commit.

- #### ➕ Save with a Message
`git stash save "WIP: added login UI"`


<br>

### 🧾 View All Stashed Changes

`git stash list`
  - Output
      - stash@{0}: WIP on main: abc123 Added login form
      - stash@{1}: WIP on feature-x: def456 Initial signup UI

<br>

### 📥 Apply Latest Stash

`git stash apply` : Keeps the stash in the list after applying.


<br>

### 📥 Apply Specific Stash

`git stash apply stash@{1}` 

<br>

### 🧹 Apply and Remove from Stash List
`git stash pop`

<br>


### ❌ Drop Specific Stash

`git stash drop stash@{1}`

<br>

### ❌ Clear All Stashes

`git stash clear`

<br>

### 📂 Stashing Specific Files
`git stash push -m "Save only login.js" login.js`

<br>

### 🔍 Show Stash Content
`git stash show stash@{0}`

- To see full diff:
`git stash show -p stash@{0}`

---
<br>


### 🧠 Pro Tip
- You can stash untracked files too: `git stash push -u`


---
<br>

### 📌 Real-World Use Case
- You’re halfway through a feature when QA finds a critical bug on main.
-  Run:
  ```
git stash
git checkout main
```

- Fix the bug, then:
```
git checkout feature-branch
git stash pop
```





  
