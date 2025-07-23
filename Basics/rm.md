## 🔧 git rm – Basics
✅ Purpose: Removes a file (or folder) from the Git index (staging area) and optionally from your working directory.

---

## 🧪 Usage Examples:
1. Remove a tracked file from Git and local system: `git rm filename.txt`
   ➡ Deletes from both Git and your local filesystem.
   
2. Just remove from Git, keep locally: `git rm --cached filename.txt`
   ➡ Removes from the Git repo but keeps it in your working directory
   ✅ Useful when you mistakenly added a file like .env or a large file.

3. Remove folders: `Copy code`
➡ -r is needed to delete directories recursively.

---

## 💬 Then what?
After git rm, always follow up with:
`git commit -m "Removed unnecessary file/folder"`
`git push origin main`

---

## 📝 Pro Tip:
- If you accidentally committed a file you want Git to ignore:
`git rm --cached filename`
`echo "filename" >> .gitignore`
`git commit -m "Removed and ignored filename"`  
