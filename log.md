# 📜 git log

`git log` shows the **history of commits** in your Git repository.  
Each log entry includes the commit ID, author, date, and message.

---

## 🔹 Basic Usage

- bash
`git log` : This shows a list of all commits in reverse chronological order.

---

## 🔹 Example Output

commit d6e8f95d7f6c6b5a3d1a...
Author: Prapti Chavan <prapti@example.com>
Date:   Tue Jul 22 10:15:23 2025 +0530

    Add hello.txt with greeting

--- 

##🔹 Most Useful Options

| Command | 	What it Does | 
| --- | --- |
| git log --oneline | 	One line per commit (short SHA + message) | 
| git log --stat | Shows file changes and line count per commit | 
| git log -p | Shows patch (diff) with each commit | 
| git log --graph | ASCII branch tree (great for visualizing) | 
| git log --author="name" | Filter commits by author | 
| git log filename | Show only commits that changed a specific file | 

---

## 🔹 Examples
`git log --oneline --graph`
`git log -p hello.txt`
`git log --since="2 days ago"`


---

## 🧪 Practice Task
1. Make 2–3 commits in your repo
2. Run:
   `git log
    git log --oneline
    git log --graph --oneline`
3. Try filtering by file or date

---

## 🧠 Pro Tips

- Combine options: git log --oneline --graph --decorate --all
- Copy-paste commit SHA to compare or revert later

---

