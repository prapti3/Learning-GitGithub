## 📘 faq.md – Frequently Asked Questions (Git & GitHub)

❓ Q1: What is the difference between git add and git commit?
- ✅ A:
`git add` : Stages changes (prepares them).
`git commit` : Saves staged changes to the repository history.


❓ Q2: Why is my folder not visible on GitHub?
- ✅ A: Git tracks files, not empty folders. Use a .gitkeep file to keep empty folders.


❓ Q3: What does fatal: not a git repository mean?
- ✅ A: It means you're trying to run Git commands outside a Git-initialized folder. Run git init or move to the correct folder.


❓ Q4: How can I undo a commit?
- ✅ A:
`git reset --soft HEAD~1` : Undo commit, keep changes staged.
`git reset --mixed HEAD~1` : Undo commit, keep changes in working directory.
`git reset --hard HEAD~1`: Discard commit and changes.


❓ Q5: What is the difference between git pull and git fetch?
- ✅ A:
`git pull` : Fetches changes and merges them.
`git fetch` : Only downloads changes (no merge).


❓ Q6: How do I resolve merge conflicts?
- ✅ A:
Edit conflicted files manually.
Mark them as resolved: git add <file>
Finish with git commit or git merge --continue.


❓ Q7: Why does git push fail with non-fast-forward error?
- ✅ A:
Your local branch is behind the remote. Run `git pull --rebase` first, then `git push`.


❓ Q8: How do I rename a file or folder in Git?
- ✅ A:
Use: git mv oldname newname


❓ Q9: How do I delete a file or folder from the repo?
- ✅ A:
Use: git rm filename then git commit -m "Remove file"


❓ Q10: How can I ignore certain files in my repo?
- ✅ A:
Create a .gitignore file and add file/folder names you want to exclude.

