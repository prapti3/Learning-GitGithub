# 🚀 git push

The `git push` command uploads your **local commits** to a **remote repository** like GitHub.

---

## 🔹 Syntax

```bash
git push <remote-name> <branch-name>

### Example:
git push origin main

```
## Common Use Case : 
1. You make local commits:
   `git commit -m "Add login feature"`

2. Then push to GitHub:
   `git push origin main`

## 🔍 Check Remote Name and Branch

- `git remote -v`       # check remote
- `git branch `         # check current branch

```
## 📌 First-Time Push (with upstream)
- If you're pushing a new branch for the first time:
`git push -u origin <branch-name>`

#### This sets the default upstream, so future pushes can be done with just:
`git push`

```

### Common Errors : 

1.  ❗ Rejected (non-fast-forward)
`error: failed to push some refs `

- Fix:
`git pull --rebase origin main`
`git push origin main`

2. ❗ Remote not set
- If Git says no upstream:
  `git push --set-upstream origin <branch>`


---

## 🧠 Pro Tip
- You can push all branches at once:
`git push --all origin `


## 📝 Summary Table

| Command | Purpose |
| --- | --- |
| git push origin main | 	Push main to origin
| git push -u origin feature | Set upstream + push | 
| git push --all origin | 	Push all local branches |
| git push | 	Push to default upstream branch |

