# 🔄 git pull

The `git pull` command is used to **fetch** and **integrate** changes from a **remote repository** into your **local branch**.

---

## 🔹 Syntax

```bash
git pull <remote-name> <branch-name>

Example :
git pull origin main

```

## 🧠 What It Does : 

- git pull = git fetch + git merge
- fetch: Gets updates from the remote.
- merge: Combines those changes with your local code.

## 🧪 Use Case
- You’re working with a team. Before pushing your changes, you want the latest code: `git pull origin main`


##⚡ With Rebase
- Instead of merging, you can rebase (for cleaner history): `git pull --rebase origin main`
  - This avoids merge commits and keeps linear history.


## 🛑 Common Errors
1. Merge conflicts during pull
  ` CONFLICT (content): Merge conflict`

- Fix:
a. Open the conflicted file.
b. Resolve the conflict manually.
c. Add the resolved file:
   `git add <file>`

2. Complete the merge: `git commit`

3. Or, if rebasing: `git rebase --continue`

## 🔁 VS git fetch
| Command | Does What |
| --- | --- |
| git fetch | Just downloads changes |
| git pull | Downloads + merges into local  |


---


## 📝 Summary Table

| Command | Purpose |
| --- | --- |
| git pull origin main | Get latest from main branch |
| git pull --rebase origin main | Rebase instead of merge |
| git fetch + git merge | Manual alternative to pull |



