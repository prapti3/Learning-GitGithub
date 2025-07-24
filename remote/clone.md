# 📥 Git Clone

Cloning a repository means creating a local copy of a remote Git repository.

---

## 🔹 Syntax

```bash
git clone <repository-url>

```

### ✅ Example: Clone a GitHub repo
`git clone https://github.com/prapti3/Learning-GitGithub.git`

👉 This will:
- Download the full repository
- Create a folder with the repo name
- Set `origin` as the default remote

```
### 🔸 Clone into a specific folder
- git clone <repo-url> <folder-name>


### Example 
- git clone https://github.com/prapti3/Learning-GitGithub.git GitLearnings


### 🔍 Check remote URL
`git remote -v`

```

### 📝 Notes
- Cloning brings entire Git history, not just current files.
- After cloning, you can create branches, commit, push/pull, etc.
- It’s the first step in contributing to an existing project.


