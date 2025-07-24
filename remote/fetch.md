# 📥 git fetch

The `git fetch` command is used to **download commits**, files, and references from a **remote repository** into your **local repository** — but **without merging** them automatically.

---

## 🔹 Syntax

```bash
git fetch <remote-name>

Example : git fetch origin

```

## 🧠 What It Does

- Gets the latest changes from the remote.
- Updates your local remote-tracking branches (like origin/main).
- Does not modify your current working branch.
- It’s like checking the news — not acting on it yet.

## 🧪 Use Case
- You want to see what’s changed on the remote before merging it:

`git fetch origin`
`git diff main origin/main`

- This compares your local main with the remote one.

---

## 🔁 fetch vs pull

| Command | Behavior |
| --- | --- |
| git fetch | Downloads changes only |
| git pull | Downloads and merges |


## 👇 Example Workflow

- `git fetch origin`         # Get latest remote changes
- `git checkout main`        # Make sure you're on the right branch
- `git merge origin/main`    # Merge fetched changes manually



## ✅ Benefits of git fetch

- Safe: Doesn’t affect your work.
- Good for reviewing changes before updating.
- Useful for CI/CD, backups, or remote inspection.



## 📝 Summary Table

| Command |	Description | 
| --- | --- |
| git fetch | Fetches all branches from origin | 
| git fetch  origin | 	Same as above
| git fetch origin main | 	Fetch only the main branch | 
| git fetch --all | 	Fetch from all remotes


