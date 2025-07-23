# 📌 git status

The `git status` command shows the **current state of your working directory** and **staging area**.

It tells you:
- Which files are staged for commit
- Which files are modified but unstaged
- Which files are untracked

---

## 🔹 Syntax

- bash
`git status`

---

## 🔹 Output Example 

`On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
        modified:   hello.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        newfile.txt`

## 🔹 Common Scenarios 

| File State | Meaning | 	Action Needed |
|---|---|---|
| Untracked | New file, Git isn't tracking it yet | `git add filename` |
| Modified (unstaged) | File changed but not yet staged | `git add filename` |
| Staged | File will be committed in next commit | `git commit -m "..."`
| Clean | 	No changes | Nothing to do 😊 |

---

## 🧪 Practice Task

1. Create a file: touch test.txt
2. Run: git status → See it under "Untracked files"
3. Add it: git add test.txt
4. Run: git status again → Now it’s staged!
5. Commit it: git commit -m "Add test.txt"
6. Run: git status → Working tree should now be clean



