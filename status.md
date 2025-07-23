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

## Output Example 

`On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
        modified:   hello.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        newfile.txt`


| File State | Meaning | 	Action Needed |
|---|---|---|
| Untracked | New file, Git isn't tracking it yet | `git add filename` |
| Modified (unstaged) | File changed but not yet staged | `git add filename` |
| Staged | File will be committed in next commit | `git commit -m "..."`
| Clean | 	No changes | Nothing to do 😊




