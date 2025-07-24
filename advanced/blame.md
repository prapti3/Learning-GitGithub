## 📄 blame.md
# 👀 git blame – See Who Changed What, When, and Why
- git blame lets you track the history of each line in a file — who changed it, when, and in which commit.

---
<br>

### 🧠 Why Use git blame?
- Debug a specific line of code
- Find the author of a change
- Understand the context or purpose of a change
- Investigate when a bug was introduced

---
<br>

### 🔧 Syntax
- `git blame <file>`
- You can also specify a line range:
   - `git blame -L 20,40 <file>`
   - This shows blame info only for lines 20 to 40.

---
<br>


### 📌 Example Output

```
e2f9a3f1 (Alice 2023-07-14 12:21:00 +0530) function calculateTotal(price, tax) {
a9c2d8e9 (Bob   2023-07-10 09:33:12 +0530)   return price + tax;
e2f9a3f1 (Alice 2023-07-14 12:21:00 +0530) }
```

- Each line shows:
   - Commit hash
   - Author name
   - Date/time
   - Line of code


---
<br>

### 🧰 Useful Options
| Option                  | Description                                    |
| ----------------------- | ---------------------------------------------- |
| `-L <start>,<end>`      | Limit blame to specific line numbers           |
| `--since="2 weeks ago"` | Show blame only for commits after a time       |
| `--author=<name>`       | Blame only lines modified by a specific author |
| `--reverse`             | Show oldest commits first (less common)        |


---
<br>

### 🛠 Pro Tip: View in GUI
- If you're using GitHub, you can:
  1. Open a file in your repo.
  2. Click on the blame button near the top.
- It gives a line-by-line history with clickable commits.

---
<br>

### 🎯 Summary

| Command                            | Purpose                         |
| ---------------------------------- | ------------------------------- |
| `git blame <file>`                 | See who last changed each line  |
| `git blame -L 10,20 <file>`        | Blame for a specific line range |
| `git blame --author=Alice`         | Show only Alice’s changes       |
| `git blame --since="3 months ago"` | Filter recent changes           |


















