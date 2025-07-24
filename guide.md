## Complete Guide for Creating Folder and Structuring Git Repo.

# 🎯 Guide 
---

## ✅ Step-by-Step: Connect Local Folder to GitHub Repo

### 🔹 1. Go to your local folder using Git Bash
- cd path/to/your/folder
- cd D:/Projects/MyApp

### 🔹 2. Initialize Git inside the folder
- git init : This makes your folder a Git repository.

### 🔹 3. Add your project files to Git
- git add .

### 🔹 4. Commit the changes
- git commit -m "Initial commit"

### 🔹 5. Create a new repository on GitHub
```
1. Go to https://github.com
2. Click ➕ (top-right) → New repository
3. Don’t add README or .gitignore if you already committed locally
4. Click Create repository
```


### 🔹 6. Copy the remote repository URL
- Example (HTTPS):
     - https://github.com/your-username/your-repo-name.git


### 🔹 7. Link your local folder to the GitHub repo
- git remote add origin https://github.com/your-username/your-repo-name.git

- You can check if it's added correctly:
   - `git remote -v`


### 🔹 8. Push your code to GitHub
`git push -u origin main`

- If your branch is master, use:
`git push -u origin master`

- If push fails due to branch name mismatch, run:
`git branch -M main`
`git push -u origin main`
