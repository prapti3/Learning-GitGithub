# 🔗 git remote add

The `git remote add` command connects your local repository to a remote one — like GitHub — so you can push or pull code.

---

## 🔹 Syntax

```bash
git remote add <remote-name> <remote-url>

```

### Example 
```git remote add origin https://github.com/prapti3/Learning-GitGithub.git```

- origin: a common default name for the remote.
- After this, you can push using:
  `git push origin main`

### 🔍 Verify the remote : 
`git remote -v`

### Expected Output :
- origin  https://github.com/prapti3/Learning-GitGithub.git (fetch)
- origin  https://github.com/prapti3/Learning-GitGithub.git (push)

### ⚠️ Common Error
- If a remote already exists and you try to add it again:
`fatal: remote origin already exists.`

### Fix it using : 
` git remote remove origin`
` git remote add origin <remote-url>`

### 🔁 Other Useful Remote Commands

| Command | Use | 
| --- | --- |
| git remote -v | View Remotes | 
| git remote remove <name> | Remove a remote | 
| git remote rename <old><new> | Rename a remote |


### 📝 Notes
- You only need to run this once per repo.
- After setting a remote, you're ready to push your commits to GitHub.




