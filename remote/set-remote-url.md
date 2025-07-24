# 🔄 How to Set or Change a Remote URL in Git

Sometimes you need to update your remote URL — for example, if:
- You changed your Git hosting from HTTPS to SSH.
- You renamed or moved your GitHub repo.
- You cloned from the wrong URL and want to fix it.

---

## 🔹 View Current Remote URLs

Use this to see what your remotes are set to:

```bash
git remote -v

Example :
- origin  https://github.com/your-username/repo.git (fetch)
- origin  https://github.com/your-username/repo.git (push)

```

## 🔹 Set (or Change) the Remote URL
- To change the origin remote:

`git remote set-url origin <new-url>`

## ✅ Example 1: Switching to SSH
`git remote set-url origin git@github.com:your-username/repo.git`

## ✅ Example 2: Changing HTTPS URL
`git remote set-url origin https://github.com/your-username/new-repo-name.git`

##🔹 Verify the Change
 - After updating, confirm the new URL:
`git remote -v`


##🔹 Add a New Remote Instead
- If you want to add a new remote (not replace):
`git remote add <name> <url>`


## Example:
`git remote add upstream https://github.com/original-owner/repo.git`


## 🔹 Remove a Remote (Optional)
`git remote remove <name>`

Example : 
`git remote remove upstream`


## 📝 Summary

| Action | 	Command Example
| --- | --- | 
| View current remotes | 	git remote -v
| Change origin URL | 	git remote set-url origin <new-url> | 
| Add new remote | 	git remote add upstream <url> | 
| Remove remote	 | git remote remove upstream | 


## 🚀 Tip
 - Use SSH URLs (git@...) to avoid entering your username/password every time.



