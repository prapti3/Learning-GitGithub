# 🔄 Pull Request (PR)

A **Pull Request (PR)** is a way to propose changes to a codebase. You request that your changes be reviewed and pulled (merged) into another branch — typically the `main` branch of a project.

---
<br>

## 🔧 When to Use a Pull Request?

- ✅ To contribute to **open-source projects**.
- 👨‍💻 To **collaborate with teammates** in private repos.
- 🛡️ To ensure **code review and testing** before merging.

---

<br>

## 📌 PR Workflow

> Let’s say you want to contribute to a repository:

<br>

### Step 1: Fork the Repository (if you don’t have write access)

```bash
# On GitHub
Click on "Fork" button → GitHub copies the repo to your account

```
<br>

 

### Step 2 :  Clone Your Fork
```

git clone https://github.com/your-username/repo-name.git
cd repo-name

```

<br>

### Step 3 : Create a New Branch
```
git checkout -b feature/my-changes
```

<br>

### Step 4: Make Your Changes Locally

- Edit files
- Add new features/fixes

<br>

### Step 5: Add and Commit Your Changes

```
git add .
git commit -m "✨ Added feature XYZ"
```

### Step 6: Push to Your Fork

```
git push origin feature/my-changes
```

<br>

### Step 7: Create a Pull Request (PR)
- Go to your fork on GitHub.
- You’ll see a prompt to "Compare & pull request".
- Add:
  - Title and description
  - Reviewers (if needed)
- Click Create Pull Request.


<br>

### ✅ What Happens Next?

- Code reviewers check your PR.
- You may get feedback or approval.
- Once approved, it’s merged into the target branch (main, dev, etc.)


### 🔁 Example PR Titles
##### 🐛 Fix: Typo in README
##### ✨ Feature: Added login validation
##### 🧪 Test: Added unit tests for user model


<br>

### 📢 Tips for Great PRs

- Keep it small and focused.
-Write a clear title and meaningful description.
- Always pull the latest code before pushing your PR.

<br>

### 🧠 Summary


| Term              | Meaning                                    |
| ----------------- | ------------------------------------------ |
| Fork              | Copy of repo under your GitHub account     |
| Clone             | Copy of repo on your local system          |
| Branch            | Isolated line of development               |
| PR (Pull Request) | Proposal to merge code into another branch |





