# 🧾 git diff

`git diff` shows the exact **line-by-line differences** between:
- Modified and unstaged files
- Staged and committed files
- Commits, branches, or any two versions

It helps you **see what changed before you commit**.

---

## 🔹 Basic Usage

- bash
`git diff` - Shows unstaged changes compared to the last commit.


---

## 🔹 Example

`echo "new line" >> hello.txt`
`git diff`

⭐ Output
`+new line`

- This means a new line was added to hello.txt.
  
---

## 🔹 View Changes After Staging

`git diff commit1 commit2`

⭐ Example 

`git diff HEAD~1 HEAD`
- Shows what changed between your last commit and current one.
  
---

## 🔹 Compare Branches

`git diff main feature-branch`

---

## 🧪 Practice Task

1. Modify a file (e.g. demo.txt)
2. Run: git diff → See changes
3. Stage the file: git add demo.txt
4. Run: git diff --cached → See staged changes
5. Commit: git commit -m "Update demo.txt"

---

## 🧠 Tips
- Use git diff before committing to review your code
- Pair it with git status for better context
- + means added lines, - means removed lines
 






