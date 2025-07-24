# 🌿 Feature Branch Workflow

The **Feature Branch Workflow** is a Git strategy used to develop new features in isolation from the main codebase (`main` or `master` branch). It helps teams collaborate efficiently without breaking the production-ready branch.

---
<br>

## 🔧 Why Use Feature Branches?

- Keeps `main` clean and deployable.
- Allows parallel development by multiple team members.
- Makes code reviews and testing easier.

---
<br>


## 📌 Step-by-Step Feature Branch Flow

### 1. Checkout to Main and Pull Latest Changes
```bash
git checkout main
git pull origin main
```

<br>

### 2. Create a New Feature Branch
- Use a descriptive name: `git checkout -b feature/login-form`

<br>

### 3. Work on Your Feature
- Make changes, then commit:
```
git add . 
git commit -m "Add login form component"

```
<br> 

### 4. Push Feature Branch to Remote
`git push origin feature/login-form`


---
<br> 

### 🔁 Keeping Your Branch Updated
- If other changes are merged into main while you’re working:
```
git checkout main
git pull origin main
git checkout feature/login-form
git rebase main
# OR use: git merge main

Then resolve any conflicts and continue:

`git add .`
`git rebase --continue`

```

---
<br>

### 🔄 Create a Pull Request (PR)
- Go to GitHub.
- Create a PR from feature/login-form → main.
- Add reviewers and comments.
- Wait for code review and approvals.


--- 
<br>

### ✅ Merge and Cleanup
- Once your PR is approved and merged:
```
git checkout main
git pull origin main
git branch -d feature/login-form        # delete local branch
git push origin --delete feature/login-form  # delete remote branch
```

---
<br>

### 📌 Naming Conventions

| Type     | Prefix Example           |
| -------- | ------------------------ |
| Feature  | `feature/signup-flow`    |
| Bugfix   | `bugfix/fix-null-error`  |
| Hotfix   | `hotfix/payment-crash`   |
| Refactor | `refactor/login-cleanup` |

---
<br>

### 🧠 Best Practices
- Keep feature branches short-lived.
- Sync with main regularly to avoid conflicts.
- One branch = one feature/task.
- Write clear commit messages.
- Test thoroughly before pushing.

---
<br>

### 🔚 Summary

| Step                  | Command Example                              |
| --------------------- | -------------------------------------------- |
| Create feature branch | `git checkout -b feature/name`               |
| Push to remote        | `git push origin feature/name`               |
| Update with main      | `git pull origin main` → `git rebase`        |
| Submit pull request   | On GitHub                                    |
| Cleanup               | `git branch -d` + `git push origin --delete` |


<br>

## Using feature branches helps make collaboration cleaner and more organized in every Git project! 🌱✨

